---
verified: 0.27.0
title: 'Quests'
description: 'Daily and weekly quests in the Overworld and the Nether, rewards and delivering.'
icon: lucide:scroll-text
categories: ['SMP']
---

::infobox{title="Quests"}

:::infobox-row{label="Command" key="command"}
`/quests`
:::

:::infobox-row{label="Realm" key="realm"}
[Overworld](/smp/realms#overworld), [Nether](/smp/realms#nether)
:::

::

Quests are daily and weekly tasks that earn you silver. Every player has the same quests. `/quests` shows them, and each [realm](/smp/realms) has its own row. On top comes the shared [World Quest](/smp/quests/world-quest).

::page-cards
::

## Quest menu

`/quests` shows your daily and weekly quests. Daily quests are on the left, weekly quests on the right. Each [realm](/smp/realms) has its own row. The colour of the slots shows the realm: green for the Overworld, red for the Nether.

Each quest shows its difficulty, its goal, your progress, the reward and the time until it ends.

After you join SMP, the game loads your quests, milestones and the World Quest in the background. Once they are ready, `/quests` and `/milestones` open immediately with the complete menu. If you open it earlier, the menu waits for the running request. Changes refresh in the background. If loading fails, you get the message **Your quests are currently unavailable.**

## How quests are drawn

- All players have the same quests.
- Daily quests arrive every day at midnight (German time).
- Weekly quests arrive every Monday at midnight.
- Each kind of quest, for example wood or combat, appears only once per day and realm where possible.
- Two quests never share the same goal.
- The same daily quest usually returns only after a week. The same weekly quest usually returns only after four weeks.

| Realm                              | Daily quests                | Weekly quests               |
| :--------------------------------- | :-------------------------- | :-------------------------- |
| [Overworld](/smp/quests#overworld) | 5: 2 easy, 2 medium, 1 hard | 3: 1 easy, 1 medium, 1 hard |
| [Nether](/smp/quests#nether)       | 3: 1 easy, 1 medium, 1 hard | 3: 1 easy, 1 medium, 1 hard |

## Nether quests

You get the Nether quests on top of your Overworld quests. You see them once you have entered the Nether for the first time. You then get the message **You entered the Nether: new Nether quests are now unlocked.** From then on, `/quests` has a row for the Nether.

Your actions count only towards quests in the matching realm. For example, an action in the Nether does not advance an Overworld quest.

## Target of the day

Some quests pick a target of the day, for example a certain kind of wood. The quest shows it as **Today: …**. How many you need depends on the target.

## Kills

In kill quests, a mob counts for the player who dealt it the most damage. On a tie, it counts for the one who hit last. That way kills count when you fight together too.

## Rewards

| Quest  |         Easy |       Medium |          Hard |
| :----- | -----------: | -----------: | ------------: |
| daily  | 1,000 Silver | 2,000 Silver |  3,000 Silver |
| weekly | 3,000 Silver | 6,000 Silver | 12,000 Silver |

Since 6 November 2026, daily quests pay at least these amounts. If you got less for a daily quest from that day on, the game pays the difference later. You then get the message **Daily quest back pay**.

Quests in the Nether pay 25% more:

| Nether quest |         Easy |       Medium |          Hard |
| :----------- | -----------: | -----------: | ------------: |
| daily        | 1,250 Silver | 2,500 Silver |  3,750 Silver |
| weekly       | 3,750 Silver | 7,500 Silver | 15,000 Silver |

## Delivering

Some quests ask you to turn in items, for example bread or iron ingots.

1. Open `/quests`.
2. Click **Select to turn in** on the quest.
3. Click matching items in your inventory. They are used up.

## World Quest

There is also a shared **World Quest**. Open `/quests`. The **World Quest** area sits directly below your personal quests. Everyone helps by donating raw materials. See the [instructions and rewards](/smp/quests/world-quest).

## Overworld

Here you find every quest that can appear in the Overworld. 5 of them arrive each day, 3 each week. How they are drawn is explained under [How quests are drawn](/smp/quests#how-quests-are-drawn).

The number under **Target** is also shown in the menu. For a target of the day, the number depends on what was drawn today.

- Wood only counts from natural logs.
- Crops only count when ripe.
- Combat counts hostile mobs unless something else is named.
- Smelting counts when you take items out of a furnace, blast furnace or smoker yourself. Items a hopper pulls out do not count. After a partial take, the rest only counts once the furnace has smelted something new.
- Chunks only count if you have never visited them.

### Daily, easy

Reward: 1,000 Silver.

| Quest            | Task                                                  | Target                          |
| :--------------- | :---------------------------------------------------- | :------------------------------ |
| Lumberjack       | fell logs                                             | 80                              |
| Wood of the day  | fell one kind of wood: oak, birch, spruce or dark oak | 8                               |
| Harvest time     | harvest crops                                         | 112                             |
| Crop of the day  | harvest one crop                                      | wheat 24, carrots 4, potatoes 2 |
| Night watch      | defeat hostile mobs                                   | 12                              |
| Mob of the day   | defeat one mob: zombie, skeleton, spider or creeper   | 6                               |
| Farm Animal Hunt | hunt cows, pigs, sheep, chickens or rabbits           | 4                               |
| Ore seeker       | mine iron or copper ore                               | 24                              |
| Coal shaft       | mine coal ore                                         | 48                              |
| Stone Quarry     | mine stone or deepslate                               | 96                              |
| Smelting furnace | take smelted items out of a furnace                   | 80                              |
| Wanderer         | enter new chunks                                      | 50                              |
| Five Biomes      | visit different biome types today                     | 5                               |
| Bakery           | turn in bread                                         | 64                              |

### Daily, medium

Reward: 2,000 Silver.

| Quest               | Task                                                | Target                                   |
| :------------------ | :-------------------------------------------------- | :--------------------------------------- |
| Forest work         | fell logs                                           | 256                                      |
| Wood of the day     | fell one kind of wood                               | oak 24, birch 24, spruce 40, dark oak 40 |
| Great harvest       | harvest crops                                       | 192                                      |
| Crop of the day     | harvest one crop                                    | wheat 112, carrots 24, potatoes 8        |
| Clean-up            | defeat hostile mobs                                 | 36                                       |
| Mob of the day      | defeat one mob: zombie, skeleton, spider or creeper | 18                                       |
| Stronger together   | defeat mobs with at least two active players nearby | 12                                       |
| Dig deeper          | mine iron or copper ore                             | 64                                       |
| Redstone Supply     | mine redstone ore                                   | 16                                       |
| Lapis Lazuli Supply | mine lapis lazuli ore                               | 8                                        |
| Smelting Furnace    | take smelted items out of a furnace                 | 112                                      |
| New Paths           | enter new chunks                                    | 150                                      |
| New land            | visit different biome types today                   | 7                                        |
| Tannery             | turn in leather                                     | 16                                       |

### Daily, hard

Reward: 3,000 Silver.

| Quest                | Task                                                            | Target                                                     |
| :------------------- | :-------------------------------------------------------------- | :--------------------------------------------------------- |
| Clear-cut            | fell logs                                                       | 128                                                        |
| Wood of the day      | fell one kind of wood                                           | oak 104, birch 56, spruce 128, dark oak 128                |
| Rare wood of the day | fell one rare kind of wood                                      | cherry 72, jungle 112, pale oak 80, acacia 16, mangrove 40 |
| Crop of the day      | harvest one crop                                                | wheat 240, carrots 64, potatoes 32                         |
| Rare crop of the day | harvest one rare crop                                           | pumpkin 16, beetroot 8, melon 5, cocoa 32                  |
| Monster hunt         | defeat hostile mobs                                             | 108                                                        |
| Mob of the day       | defeat one mob: zombie, skeleton, spider or creeper             | 36                                                         |
| Ore vein             | mine ores, including at least 3 diamond ores                    | 208                                                        |
| Cartographer         | visit different biome types today                               | 19                                                         |
| Pantry               | turn in cooked meat: steak, porkchop, chicken, mutton or rabbit | 64                                                         |

### Weekly, easy

Reward: 3,000 Silver.

| Quest          | Task                                | Target |
| :------------- | :---------------------------------- | -----: |
| Weekly wood    | fell logs                           |    704 |
| Weekly harvest | harvest crops                       |    256 |
| Weekly watch   | defeat hostile mobs                 |    120 |
| Coal week      | mine coal ore                       |    144 |
| Furnace week   | take smelted items out of a furnace |    448 |
| Trail finder   | enter new chunks                    |    300 |

### Weekly, medium

Reward: 6,000 Silver.

| Quest          | Task                                        | Target |
| :------------- | :------------------------------------------ | -----: |
| Great hunt     | defeat hostile mobs                         |    300 |
| Mine           | mine iron or copper ore                     |    256 |
| Trail finder   | enter new chunks                            |    450 |
| Globetrotter   | discover new biome types                    |      3 |
| Neighbourhood  | play near another active player, in seconds |  2,848 |
| Smith delivery | turn in iron ingots                         |     96 |

### Weekly, hard

Reward: 12,000 Silver.

| Quest          | Task                                | Target |
| :------------- | :---------------------------------- | -----: |
| Battlefield    | defeat hostile mobs                 |    700 |
| Diamond fever  | mine diamond ore                    |     80 |
| Master smelter | take smelted items out of a furnace |  1,024 |
| Explorer       | discover new structure types        |      3 |
| Repel a raid   | win a raid                          |      1 |
| Gold reserve   | turn in gold ingots                 |    128 |

For ores, the deepslate variant counts too.

## Nether

Here you find every quest that can appear in the Nether. 3 of them arrive each day, 3 each week. You get them on top of your [Overworld quests](/smp/quests#overworld). How they are drawn is explained under [How quests are drawn](/smp/quests#how-quests-are-drawn).

You see Nether quests once you have entered the Nether for the first time. They pay 25% more silver than Overworld quests.

The number under **Target** is also shown in the menu.

### Daily, easy

Reward: 1,250 Silver.

| Quest              | Task                                                              | Target |
| :----------------- | :---------------------------------------------------------------- | -----: |
| Nether Watch       | defeat piglins, zombified piglins, hoglins, magma cubes or ghasts |      7 |
| Hoglin hunt        | defeat hoglins                                                    |      2 |
| Nether Timber      | fell crimson or warped stems                                      |     32 |
| Quartz Shards      | mine nether quartz ore                                            |     24 |
| Basalt quarry      | mine basalt                                                       |     16 |
| Glowstone gatherer | mine glowstone                                                    |      8 |
| Soul ground        | mine soul sand or soul soil                                       |      8 |

### Daily, medium

Reward: 2,500 Silver.

| Quest             | Task                         | Target |
| :---------------- | :--------------------------- | -----: |
| Embers and ash    | defeat magma cubes or blazes |     24 |
| Magma hunt        | defeat magma cubes           |     18 |
| Blaze hunt        | defeat blazes                |      8 |
| Wart Harvest      | harvest ripe nether wart     |     48 |
| Nether stems      | fell crimson or warped stems |     24 |
| Nether Gold       | mine nether gold ore         |     48 |
| Blackstone quarry | mine blackstone              |     24 |

### Daily, hard

Reward: 3,750 Silver.

| Quest                | Task                                          | Target |
| :------------------- | :-------------------------------------------- | -----: |
| Ghast Hunt           | defeat ghasts                                 |      5 |
| Fortress assault     | defeat wither skeletons                       |     13 |
| Wither skeleton hunt | defeat wither skeletons                       |     12 |
| Piglin brutes        | defeat piglin brutes                          |     20 |
| Hoglin hunter        | defeat hoglins                                |      4 |
| Scrap Seeker         | mine ancient debris                           |     11 |
| Five Nether biomes   | visit five different Nether biome types today |      5 |

### Weekly, easy

Reward: 3,750 Silver.

| Quest               | Task                               | Target |
| :------------------ | :--------------------------------- | -----: |
| Nether Journey      | visit different Nether biome types |      2 |
| Nether Forester     | fell crimson or warped stems       |    112 |
| Quartz Quarry       | mine nether quartz ore             |    160 |
| Glowstone stockpile | mine glowstone                     |     16 |

### Weekly, medium

Reward: 7,500 Silver.

| Quest                    | Task                                  | Target |
| :----------------------- | :------------------------------------ | -----: |
| Nether Campaign          | defeat hostile Nether mobs            |    120 |
| Wither skeleton campaign | defeat wither skeletons               |     24 |
| Wart Fields              | harvest ripe nether wart              |    208 |
| Nether expedition        | enter a Nether fortress and a bastion |      2 |

Nether Campaign counts piglins, zombified piglins, hoglins, magma cubes, ghasts, blazes, wither skeletons and piglin brutes.

### Weekly, hard

Reward: 15,000 Silver.

| Quest           | Task                                                                        | Target |
| :-------------- | :-------------------------------------------------------------------------- | -----: |
| Ghast campaign  | defeat ghasts                                                               |      8 |
| Netherite Fever | mine ancient debris                                                         |     16 |
| Nether Explorer | enter different special Nether buildings, such as castles, villages or labs |      3 |
| Blaze hunter    | turn in blaze rods                                                          |    208 |

## Commands

- `/quests`: quests

## Frequently asked questions

### Why do I not see any Nether quests?

Nether quests, milestones and the Nether skill tree appear once you have entered the Nether. Before that, `/quests`, `/milestones` and the skill tree do not show the Nether. When you first enter it, the chat tells you what is now unlocked. More under [Realms](/smp/realms).

::navbox{category="SMP"}
::
