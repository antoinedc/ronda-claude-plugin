# ronda for Claude

ronda lets Claude change an existing web app from a GitHub repository. It runs an isolated copy of your site in a sandbox, shows you a live preview, lets you review each change, and opens a pull request when you say so. Nothing reaches your repository until you ask for a pull request, and ronda never merges or deploys anything.

## How to use it

1. Add the ronda plugin in Claude.
2. Open the plugin's Connectors tab, connect the ronda connector and sign in to your ronda account. If you do not have one yet, you can create it during sign-in. You will also be asked to connect GitHub.
3. Ask Claude to change something in one of your repositories, for example "Shorten the headline on my homepage" or "Fix the mobile menu so it does not cover the logo".
4. Open the preview link Claude shares, review the changes on the card, and ask for a pull request when you are happy.

The first time you start a project, the sandbox takes a minute or two to boot.

## What data it sends

- Your requests and the tool results go to `mcp.useronda.com`, the ronda connector.
- To edit a repository, ronda clones the GitHub repositories you connect into isolated sandboxes. It stores your sessions, the diffs of your changes and the sandbox logs.
- Pull requests are opened with your own GitHub connection, so they appear under your GitHub account.
- Privacy policy: https://useronda.com/privacy
- Terms: https://useronda.com/terms
- Support: https://useronda.com/support

## Limitations

- Works with web apps that run as a single container, such as Next.js, Vite or similar projects with a start script.
- Starting a sandbox takes a minute or two.
- ronda never merges pull requests and never deploys your app.
- Usage limits depend on your ronda workspace.
