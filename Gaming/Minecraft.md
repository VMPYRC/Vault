---
created: 2025-07-16
modified: 2025-07-17
description: PC - Mojang Studios
aliases: 
tags:
  - Gaming
---

# Version Stuff

> [!important] Minecraft Version
>
> - Java Edition
> - 1.21.7
> - Fabric

## Files to Transfer

- Specifically for creating new profiles on Modrinth
- `AppData\Roaming\ModrinthApp\profiles\fabric`
    - hotbar.nbt
    - options.txt

# Favourite Seeds

- https://www.mcseeder.com/
- https://www.chunkbase.com/apps/seed-map

|         Seed         |    Start     |                                  Nearby                                   | Safe Coordinate | Good Chunk? |              Note              |
| :------------------: | :----------: | :-----------------------------------------------------------------------: | :-------------: | :---------: | :----------------------------: |
| -3346229368945056716 |    Plains    |                  Meadow - Village x3<br>Forest<br>River                   |     0-70-0      |     yes     | 3 Villages within 350 blocks!! |
|       1000087        | Birch Forest | Pale Garden<br>Cherry Grove<br>Dark Forest<br>Dripstone Caves, Lush Caves |     0-70-0      |     eh      |                                |

# Multiplayer Setup

1. Launch [Radmin VPN](https://www.radmin-vpn.com/)
2. `Join` or `Create` a network
3. Log in to [Minecraft](https://www.minecraft.net/)

## For Host

1. Single-player
2. Enter a world
3. Options
4. Open to LAN
5. Choose a port number

## For Players

1. Multiplayer
2. Join via the port number
3. If that doesn't work...
    1. On Radmin VPN, copy the IP address number
    2. On Minecraft's Server Address field, paste the `IP:PORT`
    3. Example:
        1. IP: `111.222.3.4`
        2. PORT: `9999`
        3. `111.222.3.4:9999`

# Commands

- https://minecraft.wiki/w/Commands
- https://minecraft.wiki/w/Commands/gamerule
- https://minecraft.wiki/w/Game_rule

## Disable Friendly Fire

- "main" is your team name
- @a = all players

```
/team add main
/team join main @a
/team modify main friendlyFire false
```

## Disable Server Log Admin Commands

```
/gamerule logAdminCommands false
```

## God Mode Commands

- Syntax
    - `/effect give <targets> <effect> [seconds] [amplifier] [hideParticles]`
    - `/effect clear <targets> [effect]`
- https://minecraft.wiki/w/Effect

| command                                                         |                      note                      |
| --------------------------------------------------------------- | :--------------------------------------------: |
| /effect give @s minecraft:dolphins_grace infinite 255 true      |              fast swimming speed               |
| /effect give @s minecraft:water_breathing infinite 255 true     |                  no drowning                   |
| /effect give @s minecraft:resistance infinite 255 true          |                 reduce damage                  |
| /effect give @s minecraft:strength infinite 255 true            |               high melee damage                |
| /effect give @s minecraft:luck infinite 255 true                |                   high luck                    |
| /effect give @s minecraft:hero_of_the_village infinite 255 true | discounted trades<br>free gifts from villagers |
| /effect give @s minecraft:saturation infinite 255 true          |          restores hunger, saturation           |
| //                                                              |                       //                       |
| /effect give @s minecraft:haste infinite 255 true               |           high mining + attack speed           |

# Preferred Enchantments

- [Enchanting](https://minecraft.wiki/w/Enchanting) and [Enchanting Levels](https://minecraft.wiki/w/Enchanting/Levels)
- Command
    - `/enchant <username> <enchantment name> <number>`
    - `/enchant @s minecraft:unbreaking 3`

## Armour

|   Item   |                      Mending <br>Thorns 3 <br>Unbreaking 3                      |      Armour Trim       |
| :------: | :-----------------------------------------------------------------------------: | :--------------------: |
|  Helmet  |         💧Aqua Affinity 1 <br>💥Blast Protection 4 <br>💧Respiration 3          |   Dune <br>Amethyst    |
|  Chest   |                               🔥Fire Protection 4                               |   Spire <br>Amethyst   |
| Leggings |                  🏹Projectile Protection 4 <br>👟Swift Sneak 3                  | Wayfinder <br>Amethyst |
|  Boots   | 💧Depth Strider 3 <br>🪽Feather Falling 4 <br>🛡️Protection 4 <br>👟Soul Speed 3 |   Snout <br>Amethyst   |

## Tools

|   Item    | Mending <br>Unbreaking 3 <br>Efficiency 5 | Enchantment               |
| :-------: | :---------------------------------------: | ------------------------- |
|   🪓Axe   |             Sharpness 5 <br>              | Fortune 3 =OR= Silk Touch |
| ⛏️Pickaxe |                     —                     | Fortune 3 =OR= Silk Touch |
|  Shovel   |                     —                     | Fortune 3 =OR= Silk Touch |
|    Hoe    |                     —                     | Fortune 3 =OR= Silk Touch |
|  Shears   |                     —                     | —                         |

|           Item           |   Mending <br>Unbreaking 3   |
| :----------------------: | :--------------------------: |
|          Brush           |              —               |
|   🥕Carrot on a Stick    |              —               |
|          Elytra          |              —               |
|      🎣Fishing Rod       | Luck of the Sea 3 <br>Lure 3 |
|      Flint & Steel       |              —               |
|         🛡️Shield         |              —               |
| Warped Fungus on a Stick |              —               |

## Weapons

|    Item    |                                   Enchantment                                   |      Enchantment      |
| :--------: | :-----------------------------------------------------------------------------: | :-------------------: |
|   🏹Bow    |                 Unbreaking 3<br>Flame 1 <br>Power 5 <br>Punch 2                 | Mending =OR= Infinity |
| 🏹Crossbow |            Unbreaking 3<br>Mending<br>Piercing 4 <br>Quick Charge 3             |                       |
|  ⚔️Sword   | Fire Aspect 2 <br>Knockback 2 <br>Looting 3 <br>Sharpness 5 <br>Sweeping Edge 3 |                       |
| 🔱Trident  |      Unbreaking 3<br>Mending<br>Channeling 1 <br>Impaling 5 <br>Loyalty 3       |                       |
|    Mace    |        Unbreaking 3<br>Mending<br>Breach 4<br>Density 5<br>Wind Burst 3         |                       |

# Villagers (13)

|  Job Site Block   |        Name         | Materials                                   | Added? |
| :---------------: | :-----------------: | ------------------------------------------- | ------ |
|   Blast Furnace   |     Armourer Al     | - Iron Ingot<br>- Furnace<br>- Smooth Stone | x      |
|      Smoker       |    Butcher Bill     | - Log<br>- Furnace                          | x      |
|    Stonecutter    |  Stonemason Mason   | - Iron Ingot<br>- Stone                     | x      |
|  Smithing Table   |    Toolsmith Ted    | - Iron Ingot<br>- Planks                    | x      |
|    Grindstone     |  Weaponsmith Will   | - Sticks<br>- Stone Slab<br>- Planks        | x      |
|     Cauldron      | Leatherworker Larry | - Iron Ingot                                | x      |
|   Brewing Stand   |    Cleric Cedric    | - Blaze Rod<br>- Stone-tier Block           |        |
|      Barrel       |   Fisherman Willy   | - Planks<br>- Wooden Slab                   | x      |
|     Composter     |     Farmer Fred     | - Wooden Slab                               | x      |
| Cartography Table |  Cartographer Carl  | - Paper<br>- Planks                         |        |
|      Lectern      |   Librarian Lyle    | - Wooden Slab<br>- Bookshelf                | xxxx   |
|       Loom        |    Shepherd Sal     | - Planks<br>- String                        | x      |
|  Fletching Table  |  Fletcher Fletcher  | - Flint<br>- Planks                         | x      |

# Mods

## Instructions

1. Download [Minecraft](https://www.minecraft.net/)
2. Use [Modrinth](https://modrinth.com/)

## Current Setup

- `Modrinth` app that uses `Fabric Mod Loader` to launch `Minecraft Java Edition`

|   Category   |                         Link                         |
| :----------: | :--------------------------------------------------: |
| #Mod-Manager |          [Modrinth](https://modrinth.com/)           |
|  Mod Loader  |        [Fabric Loader](https://fabricmc.net/)        |
|     Game     | [Minecraft](https://www.minecraft.net/) Java Edition |

## Other Custom Content

- [https://mcpedl.com/category/mods/](https://mcpedl.com/category/mods/)
- [https://www.9minecraft.net/category/minecraft-mods/](https://www.9minecraft.net/category/minecraft-mods/)
- [https://www.curseforge.com/minecraft/](https://www.curseforge.com/minecraft/)
- [https://www.nexusmods.com/minecraft/mods/](https://www.nexusmods.com/minecraft/mods/)
- [https://www.planetminecraft.com/mods/](https://www.planetminecraft.com/mods/)

# `June` Save Game

- https://minecraft.wiki/
- Started June 28th, 2025

```
collect...


reach end

camel
fox
frog
goat
hoglin
llama
mooshroom
ocelot
panda
rabbit
sniffer
strider
turtle


```
