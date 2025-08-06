---
created: 2025-07-22
modified: 2025-07-22
description: A guide on how to publish your Obsidian notes online using Quartz, GitHub Desktop, and GitHub Pages
aliases:
  - How to Publish Your Obsidian Notes Online, Using Quartz, GitHub Desktop, and GitHub Pages
tags:
  - Digital
---

# Tools Overview

|  #  |         Type          |     Title      |
| :-: | :-------------------: | :------------: |
|  1  |        Source         |  [[Obsidian]]  |
|  2  | Static Site Generator |     Quartz     |
|  3  |    Version Control    | GitHub Desktop |
|  4  |        Hosting        |  GitHub Pages  |

# Setup Instructions

> [!note]
> Choose to either ==FORK== or ==CLONE== the repo.

|    Feature    | Fork                                                                                                                                                                                                                          | Clone                                                                                                                                                                                                                                                                                   |
| :-----------: | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|  Visibility   | - Shows up on the original repo as a fork                                                                                                                                                                                     | - Doesn't show up on the original repo                                                                                                                                                                                                                                                  |
| Personal Repo | - Creates a linked personal copy of the original                                                                                                                                                                              | - Creates a standalone local copy (not tied to the original)                                                                                                                                                                                                                            |
|    Changes    | - Changes are made in your fork, and visible as your repo                                                                                                                                                                     | - Changes are local until you push them to your own remote repo                                                                                                                                                                                                                         |
|    Syncing    | - Can easily sync with the original repo to get updates                                                                                                                                                                       | - Must manually pull changes from the original if you want updates                                                                                                                                                                                                                      |
|   Use Case    | - Maintains a connection to the original project, updates easy.                                                                                                                                                               | - Full control, manually pull updates from the original                                                                                                                                                                                                                                 |
| Prerequisites | 1. [GitHub](https://github.com/) account<br>2. [GitHub Pages](https://docs.github.com/en/pages) setup<br>3. [GitHub Desktop](https://desktop.github.com/download/) installed<br>4. [Obsidian](https://obsidian.md/) installed | 1. [NodeJS](https://nodejs.org/) - `node -v`<br>2. [NPM](https://nodejs.org/) - Included with NodeJS - `npm install -g npm` - `npm -v`<br>3. [Git](https://git-scm.com/) - `git --version`<br>4. [GitHub](https://github.com/) account<br>5. [Obsidian](https://obsidian.md/) installed |
|    Amount     | - 1 fork per repo                                                                                                                                                                                                             | - Multiple clones per repo                                                                                                                                                                                                                                                              |

## Fork (Easy)

1. Sign in to [GitHub](https://github.com/)
2. Fork this repository: https://github.com/jackyzha0/quartz
3. Rename repo
4. Rewrite description
5. ✅Copy the v4 branch only
6. Edit your repository details
7. Go to your repo webpage (Example: `https://github.com/username/repoName`)
8. Click the ⚙️ gear icon next to the right section that has the About, Description, Website, Readme, etc.
9. ✅ Use your GitHub Pages website
10. Add some topics like: `obsidian-vault`, `quartz`, `github-pages`, `digital-garden`, `notes`)
11. Include in the home page
12. ❌ Releases
13. ❌ Packages
14. ✅ Deployments
15. Save changes
16. Add / Create the file: `.github/workflows/deploy.yml`
17. Paste [this](https://quartz.jzhao.xyz/hosting#github-pages) into `deploy.yml`
18. Commit changes
19. On your repo webpage, go to Settings, then Pages (Example: `https://github.com/username/repoName/settings/pages`)
20. Build and Deployment
21. Source
22. Change the dropdown to GitHub Actions
23. Refresh the page
24. "Your site is live at …"
25. Visit the link
26. Clone locally
27. Go to your repo webpage (Example: `https://github.com/username/repoName`)
28. Green button `< > Code`
29. Open with [GitHub Desktop](https://desktop.github.com/download/)
30. Select the local path
31. Clone the repository
32. How are you planning to use this fork? — `For my own purposes`
33. Continue
34. Fetch origin
35. Show in Explorer (Leave this window open if you need the path)
36. Launch [Obsidian](https://obsidian.md/)
37. Open folder as vault: `content` (this is where your posts go)
38. Customize your vault
39. Transfer your settings and plugins into the `.obsidian` folder
40. Build locally before publishing your notes publicly! (next 2 steps)
41. In the base folder of your repo, right click in the folder to `Open in Terminal`
42. `npm audit fix` and then view at http://localhost:8080
43. Add notes via Obsidian, commit via [GitHub Desktop](https://desktop.github.com/download/). Repeat this cycle.
44. Done!

## Clone (Advanced)

1. Sign in to [GitHub](https://github.com/)
2. Create a new repository
3. Repository name
4. ✅ Public repository
5. ==DO NOT== initialize with a `README.md` file
6. Create repository
7. "Quick setup — if you've done this kind of thing before"
8. Copy the line shown on the page. (Example: `https://github.com/username/repoName.git`)
9. Open with [GitHub Desktop](https://desktop.github.com/download/)
10. Select the local path
11. Clone the repository
12. Fetch origin
13. Show in Explorer
14. Right click in the folder to `Open in Terminal`
15. `git clone https://github.com/jackyzha0/quartz.git
16. `cd quartz`
17. `npm i`
18. `npm audit fix`
19. `npx quartz create`
20. `Empty Quartz`
21. How should Quartz resolve links?
22. Open your Obsidian
23. Settings
24. File and Links
25. New Link Format (What links to insert when auto-generating internal links)
26. Default: `Treat links as shortest path`
27. `cd..` to primary / base folder
28. `git remote -v`
29. `git remote rm origin`
30. `git remote add origin https://github.com/username/repoName.git`
31. `username` should be your GitHub username
32. `repoName` should be your repository name
33. `git remote -v`
34. `origin` = `your repo`
35. `upstream` = `the quartz repo` (`git remote add upstream https://github.com/jackyzha0/quartz.git`)
36. Sync your changes: `npx quartz sync --no-pull`
37. Refresh your repo webpage (Example: `https://github.com/username/repoName`)
38. Should now have many files
39. Add / Create the file: `.github/workflows/deploy.yml`
40. Paste [this](https://quartz.jzhao.xyz/hosting#github-pages) into `deploy.yml`
41. Commit changes
42. On your repo webpage, go to Settings, then Pages (Example: `https://github.com/username/repoName/settings/pages`)
43. Build and Deployment >> Source
44. Change the dropdown `Deploy from a Branch` to `GitHub Actions`
45. Back to primary page (Example: `https://github.com/username/repoName`)
46. Click the ⚙️ gear icon next to the right section that has the About, Description, Website, Readme, etc…
47. ✅ Use your GitHub Pages website
48. Add some topics like: `obsidian-vault`, `quartz`, `github-pages`, `digital-garden`)
49. Optional: Include in the home page: ❌ Releases, ❌ Packages, ✅ Deployments
50. Save changes
51. In Terminal:
52. `git fetch upstream`
53. `git merge upstream/v4` (Should say: `Already up to date`)
54. Launch [Obsidian](https://obsidian.md/)
55. Open folder as vault: `content` (this is where your posts / notes go)
56. Transfer your settings and plugins into the `content/.obsidian` folder (For easier navigation: Right-click any file >> Show in System Explorer)
57. Customize your vault, add some notes
58. index is your Front Page
59. Build locally before publishing your notes publicly! (next 2 steps)
60. In the base folder of your repo, right click in the folder to `Open in Terminal`
61. `npx quartz build --serve`
62. View at where the Terminal says: `Started a Quartz server listening at http://localhost:8080` (example)
63. Add notes via Obsidian, commit via [GitHub Desktop](https://desktop.github.com/download/) or in Terminal with `npx quartz sync --no-pull`. Repeat this cycle.
64. Optional: Customize your quartz installation (see section below)
65. Done!

# Files I Used to Customize Quartz

- Repository Name / Base Folder
    - `.gitignore`
    - `quartz.config.ts`
    - `quartz.layout.ts`
    - quartz\
        - components\
            - `ContentMeta.tsx`
            - `Date.tsx`
            - styles\
                - `explorer.scss`
                - `graph.scss`
                - `search.scss`
        - styles\
            - `base.scss`
            - `callouts.scss`
            - `variables.scss`

# Quick Commands

- Run `Terminal` locally in the `quartz` directory / folder

| Command                            | Note                                                                                                                                                                      |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `npx quartz --help`                | - Help, Commands<br>- Examples: `npx quartz sync --help` and `npx quartz build --help`                                                                                    |
| `npx quartz build --serve`         | - Run a local server to live-preview your Quartz                                                                                                                          |
| `npx quartz build --serve --watch` | - Watches for changes and rebuilds automatically                                                                                                                          |
| `npx quartz sync`                  | - Syncs your local Quartz content with GitHub (pushes changes and updates local content)                                                                                  |
| `npx quartz sync --no-pull`        | - Syncs local Quartz content with GitHub without pulling remote updates                                                                                                   |
| `git remote -v`                    | - Shows the remote repos linked to your local Git repo<br>- `origin` is your fork / copy of the repo<br>- `upstream` is the original repo you forked from                 |
| `git pull origin v4`               | - Pulls the latest changes from your forked GitHub repo<br>- `v4` is your main branch<br>- `origin` is your fork / copy of the repo                                       |
| `git push origin v4`               | - Pushes your updates to your forked GitHub repo<br>- `v4` is your main branch<br>- `origin` is your fork / copy of the repo                                              |
| `git merge upstream/v4`            | - Merges the latest changes from the `v4` branch of the original Quartz repo (`upstream`) into your current branch (`origin`)                                             |
| `npm i`                            | - Installs all dependencies listed in `package.json`<br>- Run this when setting up Quartz for the first time or after pulling updates                                     |
| `npm audit fix`                    | - Automatically fixes vulnerabilities in your project's dependencies. <br>- Recommended to run after installing new dependencies or after `npm audit` reports any issues. |

# Keyboard Shortcuts on Web

|                    Command                    |          Action           |
| :-------------------------------------------: | :-----------------------: |
|           `⌘` + `K`<br>`Ctrl` + `K`           |      Search content       |
| `⌘` + `Shift` + `K`<br>`Ctrl` + `Shift` + `K` | Search content by tag (#) |
|           `ArrowUp`<br>`ArrowDown`            |  Navigate search results  |
|                     `Tab`                     |       Cycle forward       |
|                `Shift` + `Tab`                |      Cycle backward       |

# Resources

- [GitHub Desktop Documentation](https://docs.github.com/en/desktop)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [How to publish Obsidian notes with Quartz on GitHub Pages](https://notes.nicolevanderhoeven.com/How+to+publish+Obsidian+notes+with+Quartz+on+GitHub+Pages)
- [Obsidian Documentation](https://help.obsidian.md/Home)
- [Quartz Documentation](https://quartz.jzhao.xyz/)
- [Quartz Source Code on GitHub](https://github.com/jackyzha0/quartz)
