# Source: https://mintlify.com/docs/editor/git-essentials

Git lets you control and track changes to files. It’s the version control system behind branch-based workflows, where you manage content the same way you would any other codebase. The web editor handles Git operations for you. Understanding a few key concepts helps you get the most out of the editor and collaborate effectively with your team.

## 

[​](https://mintlify.com/#what-git-does-for-your-content)

What Git does for your content

Git tracks every change made to your content. It records what changed, who changed it, when they changed it, and why. This means you can:

- See the full history of any page.
- Undo changes by reverting to a previous version.
- Work on updates without affecting your live site.
- Review changes before they go live.

Your repository is the collection of files and their history that makes up your site. The editor connects to this repository to sync and publish your content.

## 

[​](https://mintlify.com/#key-concepts)

Key concepts

These are the Git concepts you’ll encounter most often when using the web editor.

Commit

A saved snapshot of your changes at a specific point in time. Each commit includes a message describing what changed and creates a permanent record in your project history.When you publish changes, the web editor creates a commit in your Git repository.

Branch

A separate line of work in your repository. Sometimes called a **feature branch**.Your live site builds from a **deployment branch**, usually called `main`. Other branches let you work on changes independently without affecting your live site. Nothing on a branch goes live until you merge it into your deployment branch with a pull request.Switch between branches using the branch dropdown in the editor toolbar. If you have unpublished changes, the editor lets you bring them to the new branch or leave them on your current branch.

Deployment branch

The branch that builds your live site, typically called `main`. Changes merged into this branch automatically deploy to your site.

Pull request

A proposal to merge changes from one branch into another. Pull requests let your team review and discuss changes before they go live.When you publish changes on a feature branch (or when your repository requires pull requests), the web editor creates a pull request. Your team reviews and merges the pull request in your Git provider (GitHub or GitLab).

Merge

Combining changes from one branch into another. After your team reviews and approves a pull request, merging the branch incorporates your changes into the deployment branch and publishes them.

Conflict

Occurs when two branches have incompatible changes to the same files. The editor helps you resolve conflicts when they occur.

Diff

A comparison showing the differences between two versions of a file. The editor shows a visual diff of your pending changes before you publish so you can review exactly what gets committed.

## 

[​](https://mintlify.com/#how-the-editor-maps-to-git)

How the editor maps to Git

Every action in the web editor corresponds to a Git operation. Here is the full reference:

| Action in the editor | Git operation |
| --- | --- |
| Edit a page | Changes auto-save to Mintlify servers. No Git commit yet. |
| Publish on your deployment branch | `git commit` and `git push`. Triggers a deployment. |
| Save in branch | `git commit` to the current feature branch. |
| Create pull request | `git push` and opens a pull request against your deployment branch. |
| Merge and publish | Merges the pull request and triggers a deployment. |
| Create a branch | `git checkout -b <branch-name>` |
| Switch branches | `git checkout <branch-name>` |
| External push or CLI update | Incoming changes sync into the editor automatically using a three-way merge. |

Related topics

[Editor overview](https://mintlify.com/docs/editor/index) [Branching and publishing](https://mintlify.com/docs/editor/branching-and-publishing) [Git concepts for documentation](https://mintlify.com/docs/guides/git-concepts)

[How to use the editor\\ \\ Previous](https://mintlify.com/docs/editor/tutorial) [Create and edit pages\\ \\ Next](https://mintlify.com/docs/editor/pages)

⌘I