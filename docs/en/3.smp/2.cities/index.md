---
verified: 0.21.0
title: 'Cities'
description: 'Build, manage and grow together.'
icon: lucide:castle
---

A city is a shared territory made of whole chunks. You manage it together, assign ranks, hold elections and can sell or rent out plots.

## Found a city

Founding a city needs network level 5 and 100,000 silver. `/city` shows what you are missing. You always see the costs before you confirm.

You can live in only one city.

## Size

A chunk is 16 × 16 blocks and covers the full height. A new city has room for 16 chunks, for example 4 × 4 chunks, which is 64 × 64 blocks. You choose the shape yourselves. Every new chunk must share a side with a chunk of the city.

How many chunks your city may occupy depends on two limits. The smaller one applies:

- **Bought capacity:** the starting size, plus 4 chunks per expansion.
- **Residents:** the starting size, plus 4 chunks per 2 residents. You count as founder.

| Residents | Chunks at most (start 25) | Chunks at most (start 16) |
| --------- | ------------------------- | ------------------------- |
| 1         | 25                        | 16                        |
| 2–3       | 29                        | 20                        |
| 4–5       | 33                        | 24                        |
| 10–11     | 45                        | 36                        |
| 20–21     | 65                        | 56                        |

Outpost chunks count towards these limits. You add at most 25 chunks per confirmation.

## Distances

Measured horizontally from border to border. Your city's own chunks border each other directly.

- to spawn: at least 512 blocks
- to other cities: at least 256 blocks
- to outposts, including your own: at least 384 blocks
- to sold plots of other cities: at least 256 blocks
- to camps: at least 64 blocks

Cities only exist in the Overworld.

## Join and leave

- A city invites you. Accept the invitation in `/city`.
- In `/city` choose **Leave city**.

## Grow

**Buy chunk capacity** gives your city room for 4 more chunks. It costs 2,500 silver per chunk, so 10,000 silver per expansion. The treasury pays.

**Add current chunk** adds the chunk you stand in. Under **Land management** you look at the chunks before confirming.

You can only use bought capacity once you have enough residents. More chunks also mean more [upkeep](/smp/cities/treasury).

## Permissions

City ranks decide who may do what, for example build, manage plots, invite residents or use the treasury. More under [Government and ranks](/smp/cities/government).

## Protection

In the city the server protects your builds. TNT and PvP are off until the city turns them on.

## Commands

- `/city`: open your city
- `/city plot`: the plot you stand on
- `/city plots`: free plots
- `/city outpost`: outposts

For `/city`:

- `view`: show borders
- `off`: hide borders
- `retry`: repeat a change whose result is uncertain

::page-cards
::
