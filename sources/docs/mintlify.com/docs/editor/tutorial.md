# Source: https://mintlify.com/docs/editor/tutorial

This tutorial walks you through a complete content update using the editor. You’ll create a branch, make a change, share a preview for review, and publish your changes.

1

Create a branch

A branch is a temporary copy of your content. It’s where you make your changes without affecting your live site.Think of branches like drafts. You can merge them into your live site or safely discard them if you choose not to make the changes.Working on a branch keeps your edits separate from your live site until you’re ready to share the content with your users.

1. In the editor toolbar, click the branch name (usually `main`).
 
 ![Branch name emphasized in the editor toolbar.](https://mintcdn.com/mintlify/yLHAwTnwTq05X1uS/images/editor/create-branch-light.png?fit=max&auto=format&n=yLHAwTnwTq05X1uS&q=85&s=87ae81c20f8d4b1899eae7f61f8ed8af)![Branch name emphasized in the editor toolbar.](https://mintcdn.com/mintlify/yLHAwTnwTq05X1uS/images/editor/create-branch-dark.png?fit=max&auto=format&n=yLHAwTnwTq05X1uS&q=85&s=07ad9f42f4beafd2ca2d383b732dbafe)
 
2. Click **Create new branch**.
3. Enter a name that describes your change, like `update-quickstart`.
4. Click **Create branch**.

The editor switches to your new branch. Any changes you make are only on the branch. They only appear on your live site if you complete the publishing process.

2

Make your changes

Edit an existing page or create a new one.**To edit a page**: Click the page name in the navigation sidebar to open it. Type directly in the editor to add content. Press / to insert components, images, or other content.**To create a page**: Click the plus button next to the navigation group where you want to add the page, then click **Add a page** and enter a filename.

![The add page menu opened beside a group in the editor.](https://mintcdn.com/mintlify/i7HF0rh5FCMSySpX/images/editor/add-page-light.png?fit=max&auto=format&n=i7HF0rh5FCMSySpX&q=85&s=5283f9de897cbf3cf87a3cac7dca935b)![The add page menu opened beside a group in the editor.](https://mintcdn.com/mintlify/i7HF0rh5FCMSySpX/images/editor/add-page-dark.png?fit=max&auto=format&n=i7HF0rh5FCMSySpX&q=85&s=8a2766dfd62e1f7cfc82fbcfb2fb601f)

3

Publish your branch

When you’re ready for review, create a pull request from your branch. A pull request is a proposal to merge your changes into the branch that builds your live site. Your changes only go live after someone approves and merges the pull request.

1. Click **Publish** in the toolbar to open the publish menu.
 
 ![The publish menu opened in the editor toolbar.](https://mintcdn.com/mintlify/i7HF0rh5FCMSySpX/images/editor/publish-menu-light.png?fit=max&auto=format&n=i7HF0rh5FCMSySpX&q=85&s=b1b35fa88340dae93b38647a18933229)![The publish menu opened in the editor toolbar.](https://mintcdn.com/mintlify/i7HF0rh5FCMSySpX/images/editor/publish-menu-dark.png?fit=max&auto=format&n=i7HF0rh5FCMSySpX&q=85&s=e2eab84933b03b41e2a88a911ecdd31a)
 
2. Optionally, click any changed file in the list to view and compare your edits against the published version.
3. Click **Create pull request**. Add a title and description, then click **Publish pull request**.

You can also click **Save in branch** to commit your changes without opening a pull request yet. This is useful if you want to keep editing before requesting review.

After the pull request is created, a preview deployment builds automatically. The publish menu shows the preview URL, a temporary link where your changes render exactly as they would on your live site. Share this URL with your reviewers.

4

Get your pull request approved

Share the pull request with your team. Reviewers can open the pull request in GitHub or GitLab to leave comments, request changes, or approve it.If a reviewer requests changes, make the edits in the editor on the same branch. Your updates push to the existing pull request automatically. You don’t need to create a new one.When all required reviewers have approved, the pull request is ready to merge.

5

Merge and publish

With the pull request approved, click **Publish** in the toolbar to reopen the publish menu. The menu now shows the pull request status and an option to merge.Click **Merge and publish**. The editor merges the pull request and switches you back to your deployment branch. Mintlify builds and deploys your changes. Your live site updates in about 30 seconds to a few minutes.

Related topics

[Git concepts for documentation](https://mintlify.com/docs/guides/git-concepts) [Git essentials for the editor](https://mintlify.com/docs/editor/git-essentials) [How to use images, screenshots, and videos in documentation](https://mintlify.com/docs/guides/media)

[Editor overview\\ \\ Previous](https://mintlify.com/docs/editor) [Git essentials for the editor\\ \\ Next](https://mintlify.com/docs/editor/git-essentials)

⌘I