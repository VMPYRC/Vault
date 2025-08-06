---
created: 2025-02-12
modified: 2025-03-28
description: PC - KRAFTON
aliases: 
tags:
  - Gaming
---

# Mods

## Installation

1. Download [BepInEx_UnityMono_x64_6.0.0-pre.1.zip](https://github.com/BepInEx/BepInEx/releases/tag/v6.0.0-pre.1)
2. Extract the into the same folder as `Dinkum.exe`
    - `Program Files (x86)\Steam\steamapps\common\Dinkum`
3. Run the game normally to generate the files
4. Close the game
5. Get mods from [NexusMods](https://www.nexusmods.com/dinkum/mods/?BH=1)
6. Place mods in the `plugins` folder
    - `Program Files (x86)\Steam\steamapps\common\Dinkum\BepInEx\plugins`
7. Or, use [[Vortex Mod Manager]]
8. Run the game. There should be a mod dialog that pops up.

## Mods I Use

- [All Day Sucker (Auto Harvest And Vacuum)](https://www.nexusmods.com/dinkum/mods/309)
- [Beam Me Up (Teleport Anywhere On The Map)](https://www.nexusmods.com/dinkum/mods/208)
- [Belt Loop (Picked Up Items Go Into Inventory Instead Of Toolbelt)](https://www.nexusmods.com/dinkum/mods/142)
- [Dig Dug (Automatically Dig Up Buried Items While Metal Detecting)](https://www.nexusmods.com/dinkum/mods/274)
- [Museum Collection Helper Redux](https://www.nexusmods.com/dinkum/mods/308)
- [Reel Easy (Makes Fishing Much Easier And Faster)](https://www.nexusmods.com/dinkum/mods/263)
- [Simple Auto Pickup (Pick Up Dropped Items Near You Automatically)](https://www.nexusmods.com/dinkum/mods/257)
- [Six Centimeters Under (Bury Items Without Digging)](https://www.nexusmods.com/dinkum/mods/281)
- [Work Smarter Not Harder (Infinite Tools Health Stamina)](https://www.nexusmods.com/dinkum/mods/266)

# Hotkeys

|       Key        |              Action               |                                                      Mod                                                       |
| :--------------: | :-------------------------------: | :------------------------------------------------------------------------------------------------------------: |
| LeftCtrl + Space |             Teleport              |             [Beam Me Up (Teleport Anywhere On The Map)](https://www.nexusmods.com/dinkum/mods/208)             |
|        F1        | Enable/Disable Simple Auto Pickup | [Simple Auto Pickup (Pick Up Dropped Items Near You Automatically)](https://www.nexusmods.com/dinkum/mods/257) |

# Commands

1. Chat Window
2. Enable commands with `devCommandsOn`
    1. Disable with `devCommandsOff`
3. Enable the cheat menu with `cheatsOn`
    1. Hotkey for cheat menu is =

## Most Used

```
devCommandsOn
cheatsOn

giveMoney `Amount`
givePoints `Amount`
giveMilestone

nextDayChange
setTime 8

= to open and spawn all items

chunkDistance 15

hideHud

```

## Commands

| check |            Command            |                                                                Description                                                                |
| :---: | :---------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------: |
|       |         /e `Emote ID`         |                                                         Performs specified emote                                                          |
|   x   |          changeRain           |                                                                                                                                           |
|   x   |    changeSpeed `NewSpeed`     |                                                                                                                                           |
|       |           cheatsOn            |                                                     Enables the cheat menu (=) hotkey                                                     |
|   x   |    chunkDistance `Number`     |                                                 Adjust the distance of chunks you can see                                                 |
|   x   |         clearFreeCam          |                                                                                                                                           |
|   x   |          compassLock          |                                                          Locks the compass north                                                          |
|   x   |     completeNPC `NPC ID`      |                                        Completes the quest given by the NPC whose ID is specified                                         |
|   x   |        completeQuests         |                                                        Completes all active quests                                                        |
|   x   |            crocDay            |                                                                                                                                           |
|   x   |      cropsGrowAllSeasons      |                                                  Allows all crops to grow in all Seasons                                                  |
|   x   |             debug             |                                                           Activates debug mode                                                            |
|   x   |        devCommandsOff         |                                                            Turns off commands                                                             |
|   x   |         devCommandsOn         |                                                         Required to use commands                                                          |
|   x   |       dropAllFurniture        |                                           Spawns 1 of each item that is tagged as "isFurniture"                                           |
|   x   |            freeCam            |                                             Activates free camera mode. `Z` key does the same                                             |
|   x   |           fullPedia           |                                                         Unlocks all Pedia entries                                                         |
|   x   |           giveGift            |                                                             Adds 1,000 Dinks                                                              |
|   x   |         giveMilestone         |                                      Randomly progresses 1 level of Milestones or unlocks a new one                                       |
|   x   |      giveMoney `Amount`       |                                                      Adds specified amount of Dinks                                                       |
|   x   |      givePoints `Amount`      |                                                  Adds specified amount of Permit Points                                                   |
|   x   |  hairColour `Hair Color ID`   |                                                    Changes hair colour to specified ID                                                    |
|   x   |      hairStyle `Hair ID`      |                                                    Changes hair style to specified ID                                                     |
|   x   |           hideGuide           |                                                              Hides the Guide                                                              |
|   x   |            hideHud            |                                                   Hides the HUD + Good for screenshots                                                    |
|   x   |          loadFreeCam          |                                                                                                                                           |
|   x   |           makeWindy           |                                                                                                                                           |
|   x   |     maxRelation `NPC ID`      |                                            Maximizes your relationship with the specified NPC                                             |
|       |         moveAllCarry          |                                                                                                                                           |
|   x   |      moveInNPC `NPC ID`       |                                                   Moves in the specified NPC into town                                                    |
|   x   |            nextDay            |                                              Sleeping. Saves the day. Progresses to next day                                              |
|   x   |         nextDayChange         |                                            Commits changes of the day without skipping the day                                            |
|   x   |            noClip             |                                                           Invisible character.                                                            |
|   x   |        noClipNoFollow         |                                               Can move character. Does not follow character                                               |
|   x   |         npcPhoto `ID`         |                                                                                                                                           |
|   x   |      placeItem `Item ID`      |                        Places a tile at the position the player is looking, use -1 to remove existing placed tiles                        |
|   x   |    placeItemFix `Item ID`     |                                                                                                                                           |
|   x   |        randomClothing         |                                                        Changes character clothing                                                         |
|   x   |      randomiseCharacter       |                                                       Changes character appearance                                                        |
|   x   |         refreshInside         |                                                         Reset the house interior                                                          |
|   x   |      renameIsland `Name`      |                                                          Changes the island name                                                          |
|   x   |          resetHouse           |                                                         Reset the house interior                                                          |
|   x   |      resetHouseExteriors      |                                                         Reset the house exterior                                                          |
|   x   |             save              |                                                              Saves the game                                                               |
|   x   |          saveFreeCam          |                                                                                                                                           |
|   x   |            scanMap            |                                            Updates the map. Reveals the whole map in the mine.                                            |
|   x   |     setAnimalRel `Value`      |                                        Sets the value for all animal relationships - Maximum `100`                                        |
|   x   | setDate `Day Week Month Year` |                                                   Sets the calendar to a specified date                                                   |
|   x   |           setStatus           |                                                                                                                                           |
|   x   |        setTime `Hour`         |                                             Sets the time to a specified hour. 24 hour format                                             |
|   x   |          setTimeDay           |                                                          Sets the time to 10 AM                                                           |
|   x   |         setTimeNight          |                                                           Sets the time to 7 PM                                                           |
|   x   |          setTimeReal          |                                                                                                                                           |
|   x   |           setTired            |                                                            Sets stamina to -40                                                            |
|   x   |      skinTone `Skin ID`       |                                                    Sets the skin tone to a specific ID                                                    |
|   x   |           skipSong            |                                                          Skips the current song                                                           |
|   x   |    spawnAnimal `Animal ID`    |                                                          Spawns specified animal                                                          |
|   x   |           spawnBoat           |                                                        Spawns Mysterious Salesman                                                         |
|   x   |        spawnCarry `ID`        | Spawns a carriable with specified ID from [Carriable List](https://modding.wiki/en/dinkum/developers/carriable-list) at player's position |
|   x   |  spawnFarmAnimal `Animal ID`  |                                                       Spawns specified farm animal                                                        |
|   x   |       spawnNpc `NPC ID`       |                                                           Spawns specified NPC                                                            |
|   x   |          stopRandom           |                                                       Disables random cloth change                                                        |
|   x   |     strikeLightning `X Z`     |                                                   Lightning strikes at specified point                                                    |
|   x   |        teleport `X Z`         |                                                        Teleport to specified point                                                        |
|   x   |         unlockRecipes         |                                                       Unlocks all crafting recipes                                                        |

# Resources

- https://steamcommunity.com/sharedfiles/filedetails/?id=2850877983
