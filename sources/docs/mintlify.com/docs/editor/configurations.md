# Source: https://mintlify.com/docs/editor/configurations

Configure your site’s branding, appearance, and features from the **Site configurations** panel in the web editor. Configuration changes sync in real time with other editors on the same branch, so your team always sees the latest settings. To open the panel, click the configurations icon in the editor toolbar.

![Configurations menu in the editor.](https://mintcdn.com/mintlify/yLHAwTnwTq05X1uS/images/editor/configurations-light.png?fit=max&auto=format&n=yLHAwTnwTq05X1uS&q=85&s=8d3d37dc337b15b533426bb4b9c24445)![Configurations menu in the editor.](https://mintcdn.com/mintlify/yLHAwTnwTq05X1uS/images/editor/configurations-dark.png?fit=max&auto=format&n=yLHAwTnwTq05X1uS&q=85&s=01aba3d30c86ab77a959a7672098b905)

The panel groups settings into sections that map to the top-level properties in your [`docs.json`](https://mintlify.com/docs/organize/settings).

## 

[​](https://mintlify.com/#general)

General

Set your site’s identity and how it appears to visitors.

- **Name**: The name of your project. Appears in browser tabs and search results.
- **Description**: Brief overview of your project. Used for SEO and AEO.

## 

[​](https://mintlify.com/#branding)

Branding

Upload the marks that identify your site.

- **Logo**: Your brand logo. Upload PNG or JPG files. Set separate light and dark versions and an optional click-through URL. To use an SVG logo, add the file to your repository and reference its path in your [`docs.json`](https://mintlify.com/docs/organize/settings-appearance#logos).
- **Favicon**: Small icon that appears in browser tabs. Upload ICO, PNG, GIF, or JPG files. Set separate light and dark versions if needed.

## 

[​](https://mintlify.com/#styling)

Styling

Control your site’s visual identity and color scheme.

- **Theme**: Choose a [theme](https://mintlify.com/docs/customize/themes) for your site’s overall appearance.
- **Primary color**: The main accent color used throughout your site for links, buttons, and highlights.
- **Light color**: Accent color used in dark mode. How themes apply this varies by theme.
- **Dark color**: Accent color used in light mode. How themes apply this varies by theme.
- **Background color**: Custom background colors for light and dark modes.
- **Icon library**: Icon library used for all icon properties. Defaults to `fontawesome`.
- **Strict appearance**: Lock the site to a single appearance mode and hide the theme toggle.
- **Default appearance**: Whether your site loads in `system`, `light`, or `dark` mode by default.
- **Background decoration**: Apply a visual style (`gradient`, `grid`, or `windows`) to your background.
- **Background image**: Optional background image. Set a single image or separate light and dark versions.

## 

[​](https://mintlify.com/#typography)

Typography

Replace default fonts with your brand’s typography.

- **Font family**: Any [Google Fonts](https://fonts.google.com/) family works out of the box. For a self-hosted font, provide a source URL and format (`woff` or `woff2`).
- **Weight**: Typically `400` for regular and `700` for bold. Variable fonts support precise weights like `550`.
- **Heading font**: Optional override applied to all headings (`h1` through `h6`).
- **Body font**: Optional override applied to body text and the remainder of the page.

## 

[​](https://mintlify.com/#navbar)

Navbar

Add navigation elements to the top of your site.

- **Primary button**: The main call-to-action in your header. Set the type, label, and destination URL.
- **Navbar links**: Additional navigation links in your header. Each link includes text and a URL.

## 

[​](https://mintlify.com/#footer)

Footer

Add links and social media handles to your site footer.

- **Social links**: Profiles on platforms like GitHub, X, LinkedIn, Discord, YouTube, and Slack.
- **Footer columns**: Enable to organize footer links into up to four columns with custom headings.

## 

[​](https://mintlify.com/#banner)

Banner

Display an announcement bar across the top of every page.

- **Content**: The banner text. Supports basic MDX formatting like links, bold, and italic. Custom components are not supported.
- **Dismissible**: Show a dismiss button on the right side of the banner.
- **Type**: Visual style. `info` uses the primary brand color, `warning` uses an amber background, and `critical` uses a red background. Defaults to `info`.
- **Color**: Override the banner background color with a custom hex color. Set separate light and dark values for theme-aware colors.

## 

[​](https://mintlify.com/#thumbnail)

Thumbnail

Customize page thumbnails and social previews.

- **Background**: Custom background image for thumbnails.
- **Appearance**: Render thumbnails in `light` or `dark` mode. When unset, thumbnails are auto-generated from your theme colors.
- **Font**: Custom font for text in thumbnails.

## 

[​](https://mintlify.com/#content)

Content

Customize how content appears on your site.

- **Page eyebrow**: Show small labels preceding page titles. Choose `section` or `breadcrumbs`.
- **Timestamps**: Show the date the content was last modified on all pages.
- **LaTeX**: Load LaTeX (KaTeX) stylesheets for mathematical notation rendering.

## 

[​](https://mintlify.com/#code-blocks)

Code blocks

Configure syntax highlighting and code block behavior.

- **Code block theme**: Match the site light/dark mode with `system`, always use a dark theme with `dark`, or pick a custom [Shiki](https://shiki.style/) theme.
- **Custom code languages**: Register additional syntax highlighting languages.

## 

[​](https://mintlify.com/#context-menu)

Context menu

Configure the quick actions surfaced in the page context menu.

- **Options**: Multi-select dropdown of actions like `copy`, `view`, and opening the page in `chatgpt`, `claude`, `cursor`, and other AI assistants.
- **Display**: Where to display the options. `header` (default) shows them in the top-of-page context menu; `toc` shows them in the table of contents sidebar.

## 

[​](https://mintlify.com/#navigation)

Navigation

Tune navigation behavior across your site.

- **Drilldown**: Auto-navigate to the first page when a user clicks a navigation group.

## 

[​](https://mintlify.com/#search)

Search

Customize the search experience and feedback.

- **Search placeholder**: The text that appears in the search box before users type. Default is `Search or ask`.
- **Feedback**: Show thumbs-up and thumbs-down buttons or a “Suggest edits” link on every page.

## 

[​](https://mintlify.com/#api-reference)

API reference

Document your API endpoints.

- **OpenAPI specs**: Add OpenAPI specification files to generate API reference pages.
- **AsyncAPI specs**: Add AsyncAPI specification files to generate API reference pages.
- **MDX server**: Custom MDX server endpoints for the API playground.
- **Playground display**: Show the interactive API playground, the simple API playground, or no API playground.
- **Proxy server**: Enable or disable the proxy server for API requests.
- **MDX schema**: Whether to render the schema section on API reference pages.

## 

[​](https://mintlify.com/#redirects)

Redirects

Use the **Redirects** section to add, edit, search, and remove redirects without manually editing your `docs.json` file. Redirects send users from old URLs to new ones, which is useful when you rename pages or restructure your site. For more information, see [Redirects](https://mintlify.com/docs/create/redirects). Each redirect has the following fields:

- **Source**: The path to redirect from, like `/old-path`. Supports wildcards.
- **Destination**: The path to redirect to, like `/new-path`. Supports wildcards.
- **Status**: The HTTP status code for the redirect.
 - `308`: Permanent redirect. Use this for content that has moved permanently. This is the default status.
 - `307`: Temporary redirect. Use this when the move is temporary.

![Redirects menu in the editor.](https://mintcdn.com/mintlify/De7VVdLQKy1YZcUm/images/editor/redirects-light.png?fit=max&auto=format&n=De7VVdLQKy1YZcUm&q=85&s=ab5f397d74f04d07f3ab1b4f3149763a)![Redirects menu in the editor.](https://mintcdn.com/mintlify/De7VVdLQKy1YZcUm/images/editor/redirects-dark.png?fit=max&auto=format&n=De7VVdLQKy1YZcUm&q=85&s=2ca09783d35e3ed01cea7b2975e623f6)

To add a redirect:

1. Click **Add redirect**.
2. Enter the source and destination.
3. Click **Save**.

To edit or remove an existing redirect, hover over the row and use the inline edit icon or the **X** to remove it.

## 

[​](https://mintlify.com/#seo)

SEO

Configure metatags and indexing for search engines.

- **Metatags**: Custom `<meta>` tags applied across your site. Add key-value pairs for tags like `og:image` or `twitter:card`.
- **Indexing**: Choose whether to index hidden pages.

## 

[​](https://mintlify.com/#analytics)

Analytics

Connect analytics platforms to track visitor behavior. Supported providers include Amplitude, Mixpanel, Heap, Google Analytics, Google Tag Manager, PostHog, Plausible, Fathom, Segment, Hightouch, Hotjar, LogRocket, Microsoft Clarity, Intercom, Clearbit, and more. Each entry renders as an inline row. Use the **X** icon to remove an integration.

## 

[​](https://mintlify.com/#404-page)

404 page

Customize the experience when a user lands on a missing page.

- **Redirect to home**: When on, missing pages redirect to your home page. When off, the site shows a 404 page and you can customize the title and description below.
- **Title**: Heading shown on the 404 page.
- **Description**: Subheading shown on the 404 page.

## 

[​](https://mintlify.com/#variables)

Variables

Define custom variables that can be re-used throughout your content. Each variable is a key-value pair. Use the **X** icon to remove a variable.

Related topics

[CI checks](https://mintlify.com/docs/deploy/ci) [Content Security Policy (CSP) configuration](https://mintlify.com/docs/deploy/csp-configuration) [Global settings](https://mintlify.com/docs/organize/settings)

[Ask agent\\ \\ Previous](https://mintlify.com/docs/editor/agent) [Editor settings for AI and publishing\\ \\ Next](https://mintlify.com/docs/editor/settings)

⌘I