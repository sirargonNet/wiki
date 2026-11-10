---
verified: 0.21.0
title: 'Quests'
description: 'Daily and weekly quests, rewards and delivering.'
icon: lucide:scroll-text
---

`/quests` shows your daily and weekly quests. Daily quests are on the left, weekly quests on the right. Each [realm](/smp/realms) has its own row. The colour of the slots shows the realm: green for the Overworld, red for the Nether.

Each quest shows its difficulty, its goal, your progress, the reward and the time until it ends.

Your actions count towards quests in the matching realm. For example, an action in the Nether does not advance an Overworld quest.

::page-cards
::

## How quests are drawn

- All players have the same quests.
- Daily quests arrive every day at midnight (German time).
- Weekly quests arrive every Monday at midnight.
- Each kind of quest, for example wood or combat, appears only once per day and realm where possible.
- Two quests never share the same goal.
- The same daily quest usually returns only after a week. The same weekly quest usually returns only after four weeks.

| Realm                              | Daily quests                | Weekly quests               |
| :--------------------------------- | :-------------------------- | :-------------------------- |
| [Overworld](/smp/quests/overworld) | 5: 2 easy, 2 medium, 1 hard | 3: 1 easy, 1 medium, 1 hard |
| [Nether](/smp/quests/nether)       | 3: 1 easy, 1 medium, 1 hard | 3: 1 easy, 1 medium, 1 hard |

## Nether quests

You get the Nether quests on top of your Overworld quests. You see them once you have entered the Nether for the first time. You then get the message **You entered the Nether: new Nether quests are now unlocked.** From then on, `/quests` has a row for the Nether.

## Target of the day

Some quests pick a target of the day, for example a certain kind of wood. The quest shows it as **Today: …**. How many you need depends on the target.

## Kills

In kill quests, a mob counts for the player who dealt it the most damage. On a tie, it counts for the one who hit last. That way kills count when you fight together too.

## Rewards

| Quest  |         Easy |       Medium |          Hard |
| :----- | -----------: | -----------: | ------------: |
| daily  | 1,000 Silver | 2,000 Silver |  3,000 Silver |
| weekly | 3,000 Silver | 6,000 Silver | 12,000 Silver |

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

New daily quests use the rewards above from 0.21.0. Quests already drawn keep their existing terms. The change takes effect at the next daily draw or a later scheduled publication. Check your quest menu for your current rewards.

## Commands

- `/quests`: quests
