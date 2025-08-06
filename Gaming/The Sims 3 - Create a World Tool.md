---
created: 2025-02-12
modified: 2025-07-31
description: PC - Electronic Arts
aliases:
  - TS3 CAW
tags:
  - Gaming
---

# Setup

1. [Create A World (CAW)](http://thesims3.com/content/global/downloads/caw/worldtool.exe)
2. Custom install
3. `Documents\Electronic Arts\The Sims 3`
4. Start Menu
5. `regedit.exe`
6. `Computer\HKEY_LOCAL_MACHINE\SOFTWARE\WOW6432Node\Sims(Steam)`
7. Right Click `Sims(Steam)`
8. Export
9. Edit in text editor
10. Find: `Wow6432Node\Sims(Steam)`
11. Replace with: `Wow6432Node\Sims`
12. Save
13. File
14. Import

# How to Export a Pre-Made World into CAW

## Prerequisites

- Create A World (CAW)
- S3PE
- [[The Sims 3]] Game

## Instructions

1. Start CAW
2. File
3. New World
4. Choose any
    - Example: LargeFlatMap300, 100 Height, Lush
5. OK
6. File
7. Save As
8. Temp.world
9. Save
10. `Wait for the "Save Successful" popup`
11. OK
12. Close CAW
13. Open S3PE
14. File
15. Open
16. Go to `Documents\Electronic Arts\The Sims 3 Create A World Tool\UserToolData\Worlds`
17. Temp.world
18. Open
19. Resource
20. Import
21. From Package
22. Navigate to the world you want to edit
    - Example: Sunset Valley.world
23. Open
24. Import Files:
    - YES -- Replace Duplicates
    - YES -- Compress
    - YES -- Use Resource Name
25. Import
26. NO -- Autosave
27. On the bottom, there are checkboxes and text fields
    1. Underneath `Tag`, checkmark and write `WPID` into the text field
    2. Click the `Set` button
    3. Checkmark the `Filter Active`
    4. Delete WPID file(s)
    5. Uncheck the box under Tag
    6. Underneath `ResourceType`, checkmark and write `0x296A6258` into the text field
    7. Click the `Set` button
    8. Delete the UNKN 0x296A6258 file(s)
28. Close the program this way to see that the saving process is fully complete:
    1. Top Right RED X (Close the program)
    2. Save Now?
    3. YES
    4. Wait for the entire program (S3PE) to close
29. Open CAW
30. File
31. Open World
32. Temp.world
33. Open
34. Left Pane that says "World Layers"
35. Right click Temp.world
36. Add/Edit Description
    1. Enter the desired name
    2. Enter the desired description
    3. Select a 256x256 24-bit image
    4. Example
        1. ![[Pink_256x.png]]![[Pink_500x.png]]
    5. OK
37. ==DO NOT MAKE ANY OTHER CHANGES TO THE WORLD==
38. File
39. Save As
40. Sunset Valley Edited.world (Or whatever you want)
41. Save
42. Wait for the "Save Successful" popup
43. OK
44. Close CAW
45. Open File Explorer
46. Go to: `Documents\Electronic Arts\The Sims 3 Create A World Tool\UserToolData\Worlds`
47. Delete Temp.world & the folder
48. Continue on to the next section

## Edit World

1. Open CAW
2. File
3. Open world
4. Select a world
5. Open
6. Make any edits you want
7. ==Save frequently if you plan to make lots of changes==
8. Wait for the "Save Successful" popup
9. File
10. Select World to Export
11. Select your newly created world (Example: Sunset Valley Edited.world)
12. Open
13. `Wait for the "Success! World Export was Successful!" popup`
14. OK
15. Go to `Documents/Electronic Arts/The Sims 3/Exports`
16. Select the world
17. CTRL + X
18. Go to `Documents/Electronic Arts/The Sims 3/Downloads`
19. CTRL + V
20. Launch The Sims 3 Launcher
21. Downloads
22. CHECKMARK the world
23. Install
24. `Wait for installer`
25. OK
26. Launch [[The Sims 3]]
27. Create a new game
28. Select your world
29. Play
30. Enjoy
