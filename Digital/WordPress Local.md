---
created: 2025-07-22
modified: 2025-07-22
description: A guide on how to publish your WordPress Blog online using XAMPP, WordPress, Simply Static, GitHub Desktop, and GitHub Pages
aliases:
  - How to Publish Your WordPress Blog Online Using XAMPP, WordPress, Simply Static, GitHub Desktop, and GitHub Pages
tags:
  - Digital
---

# Tools Overview

|  #  |      Name      |          Type           |
| :-: | :------------: | :---------------------: |
|  1  |     XAMPP      | Local Database / Server |
|  2  |   WordPress    |    Blogging Software    |
|  3  | Simply Static  |    WordPress Plugin     |
|  4  | GitHub Desktop |   Git Version Control   |
|  5  |  GitHub Pages  | Static Website Hosting  |

# Instructions

1. Install [XAMPP](https://www.apachefriends.org/index.html)
2. Launch the XAMPP Control Panel
3. `Start` these servers
    1. Apache - web server
    2. MySQL - database server
4. Allow access from Windows Firewall
5. Should be green
6. In the `htdocs` folder of where you installed XAMPP, create a folder called `website-name` or something easily identifiable
    1. `Program Files/XAMPP/htdocs`
    2. `XAMPP/htdocs`
7. Create a [GitHub repository](https://github.com/)
8. Create a new branch: `gh-pages`
9. Settings
10. General
11. Default branch: `gh-pages`
12. On main repo page
13. Click the gear icon next to the "About" and "No description, website, or topics provided"
14. Write a description
15. ✅ Use your GitHub Pages website
16. Save changes
17. Click the link, and it should open up to something like: `username.github.io/project-name/ `
18. Clone the repo to your desktop with [GitHub Desktop](https://github.com/apps/desktop) into that folder (example: `website-name`)
19. Download and Extract [WordPress](https://wordpress.org/download/)
20. Copy and paste the `wordpress` folder CONTENTS into the project folder (example: `website-name`)
21. On your browser: `https://localhost/website-name/`
22. Should load the WordPress installation wizard
23. Choose a language
24. On your browser: `https://localhost/phpmyadmin/`
25. Databases tab
26. Create database - name your database
27. Back to the browser tab: `https://localhost/website-name/`
28. Let's go!
29. Database Name
30. Username: `root`
31. Password: none
32. Database Host: `localhost`
33. Submit
34. Run the installation
35. Site Title, Username, Password, Email
36. Install WordPress
37. Log In
38. Update the Appearance: `https://localhost/website-name/wp-admin/themes.php`
39. Add posts
40. Add the plugin: Simply Static
41. Manage the settings
42. General Section
    1. Replacing URLs
    2. Absolute URLs
    3. Scheme - https://
    4. Host - example: `username.github.io/project-name/` (should be open in your browser, from ==step 17==)
    5. Include the following in `Additional Files and Directories`
        1. Write their full path on separate lines for:
        2. `xampp/htdocs/website-name/wp-content
        3. `xampp/htdocs/website-name/wp-content/uploads`
    6. Save Settings
43. Deploy Section
    1. Deployment Method
    2. Local Directory
    3. Path: the path of your project folder
        1. Write the full path for:
        2. `xampp/htdocs/website-name/public_static/`
    4. Save Settings
44. Generate Button
45. Wait
46. Generate Static Files
47. Activity Log
    1. Check the messages for any missing files
    2. Fetched 500 of 500 pages/files
    3. Transferred 500 of 500 files
48. Diagnostics
    1. Check this for any errors
49. Open GitHub Desktop
50. Add a commit message
51. Commit files
52. Push to Origin
53. Wait for GitHub Pages to deploy
54. View website on the example: `username.github.io/project-name/ `

## For New Changes

1. Launch the XAMPP Control Panel
2. `Start` these servers
    1. Apache - web server
    2. MySQL - database server
3. Make your WordPress changes / edits / updates
4. Simply Static Plugin
5. Generate Button
6. Wait until finished
7. Add a commit message on GitHub Desktop
8. Push to origin
9. View website on the example: `username.github.io/project-name/ `
