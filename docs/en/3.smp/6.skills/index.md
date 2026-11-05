---
verified: 0.21.0
title: 'Skills'
description: 'Skill points, commands, skill tree and mana.'
icon: lucide:sparkle
---

SMP XP raises your level and gives you skill points. You spend them in the skill tree to unlock abilities. How you collect XP and how much a level costs is under [Levels and XP](/smp/skills/levels).

::page-cards
::

## Skill tree

In the skill tree you unlock stars. Every star costs one skill point. A star needs the tier before it. Higher tiers also need points in the same category, counted over all abilities of that category:

- abilities with 5 tiers: from tier III the first number of points, from tier IV the second
- abilities with 8 tiers: from tier IV the first number of points, from tier VI the second

**Show as constellation** and **Show in columns** switch the view. The same choice is in `/settings`.

## Mana

Abilities for larger areas only trigger while sneaking and cost mana. Your mana is shown above the hotbar. `/skills` shows it too.

- Without [Mana Storage](/smp/skills/overworld) you have 50 mana. Every tier adds 25 mana, up to 250.
- Without Mana Flow your mana refills by 0.5 per second. Mana Flow makes it faster, up to 2.5 per second.
- Your mana is full again when you join the server, leave it or die.

| Ability        | Mana              |
| :------------- | :---------------- |
| Vein Miner     | 3 per extra block |
| Tunnel Borer   | 2 per block       |
| Tree Feller    | 2 per extra log   |
| Harvest Scythe | 1 per ripe crop   |
| Excavator      | 1 per block       |
| Sprint Boost   | 20                |

The mana stars of a category lower these costs by 5% per tier. If a block is protected, you get its mana back. When your mana runs out, the ability stops. The blocks broken so far stay broken.

## Good to know

- Abilities only work in Survival mode.
- Abilities are off while you fight other players.
- Territory rights apply to every single block. When an ability reaches a protected block, it stops there.
- No ability breaks blocks you placed yourself.
- When your tool has 5 durability or less left, you only break single blocks. That way it does not break.
- An ability runs as long as you sneak and hold the same tool in the same slot. If you let go or switch, it stops.
- Every block must be at most 32 blocks away from you and loaded. Otherwise the ability stops.
- If you trigger an ability while another one runs, the new one waits. At most 4 wait at the same time. If you stop the running one yourself, the waiting ones are dropped.
- Use `/skills toggle` to turn off an ability that gets in your way.

## Commands

`<…>` and `[…]` are placeholders; `[…]` is optional, `a|b` means one of them.

- `/skills`: abilities and mana
- `/skills tree` or `/skilltree`: skill tree
- `/skills toggle <ability>`: turn an ability on or off
- `/skills reset`: reset stars

### Resetting

`/skills reset` resets all stars. You keep your XP and skill points.

Your first reset is free. After that, every further reset costs 2,000 Silver more: 2,000, 4,000, 6,000 Silver and so on. You see the price before you confirm.

When we change skill values, you may reset once for free. After that, the prices start from the beginning.
