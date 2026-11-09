---
verified: 0.24.0
title: 'Cities'
description: 'Build, manage and rise through eight tiers together.'
icon: lucide:castle
---

A city is a shared territory made of whole chunks. You manage it together, assign ranks, hold elections and can sell or rent out plots. Through your play time the city rises through eight [tiers](/smp/cities/tiers), from Clearing to Metropolis.

::callout{type="info" title="Claims 2.0"}
Since version 0.24.0 cities grow through tiers instead of bought capacity. There is no upkeep any more. If you founded a city before, read [Claims 2.0 for existing cities](/smp/cities/claims-2).
::

## Found a city

Founding a city needs network level 5 and 100,000 Silver. You pay this yourself. `/city` shows what you are missing. You always see the costs before you confirm.

- The price includes the first 16 chunks, for example 4 × 4 chunks, so 64 × 64 blocks.
- Every new city starts at tier 1, the **Clearing**.
- You can only live in one city.
- When you found a city, the whole server hears about it: "{player} founded the city {city}."

### From your camp

If you have a [camp](/smp/camps), you can turn it straight into a city. Choose **Found city** in `/camp`.

- The camp chunks become the city. The city gets only these chunks, no extra 16.
- Silver you paid for camp expansions counts towards the founding price. At most what the expansions of your current camp are worth. The price never drops below 0.
- The camp is gone afterwards. Residents and rights are not carried over. The city starts with default settings.
- You must not be in a city yet and need network level 5.

## Size

A chunk is 16 × 16 blocks and covers the full height. You choose the shape. Every new chunk must share a side with a chunk of the city.

How many chunks your city may have depends on its [tier](/smp/cities/tiers): 24 as a Clearing, 640 as a Metropolis. Chunks of [outposts](/smp/cities/outposts) count too. Each confirmation adds at most 25 chunks.

The city menu shows the limit as "{occupied} / {limit} · Tier {tier} · {name}".

## Distances

Distances are measured horizontally from border to border. Chunks of your own city border each other directly.

- to spawn: at least 512 blocks
- to other cities: at least 256 blocks
- to outposts, including your own: at least 384 blocks
- to sold plots of other cities: at least 256 blocks
- to camps: at least 64 blocks

Cities exist only in the Overworld.

## Join and leave

- A city invites you. You accept the invitation in `/city`.
- In `/city` choose **Leave city**.

## Add land

**Add current chunk** adds the chunk you stand in. Every new chunk costs 16,000 Silver from the city treasury. It is paid right when you claim it. Under **Land management** you can check the chunks before you confirm.

When your tier's limit is reached, the game says: "Your city has reached its tier's chunk limit." Only the next tier helps then.

## Release land

Under **Land management**, **Release chunk** gives up the chunk you stand in. You need the right **Expand city**, for outposts **Manage outposts**.

- There is no refund. New land costs the full price again.
- A chunk containing a plot cannot be released.
- The city must not split into two parts.
- You cannot release the city's last chunk. Use **Dissolve city** instead.
- If spawners stand in the chunk, the confirmation lists them.

## Rights and protection

City ranks decide who may do what, for example build, manage plots, invite residents or use the treasury. See [Government and ranks](/smp/cities/government) and [Rights and area settings](/smp/cities/rights).

Inside the city the server protects your builds. TNT and PvP are off until the city turns them on. When protection refuses an action, the message names the reason, for example "Missing right: {right} in {area}."

## Frozen cities

When no member has been active for a longer time, the city freezes. Members with a linked Discord get two warnings by direct message before that, with the date.

- The city stays **frozen and protected**. Land, treasury, tier, members and sold plots are kept.
- City actions, rents and the tier project pause.
- When a member is active again, the city thaws for free.

::callout{type="info"}
For now, abandoned tier cities stay frozen and protected, without ruin, decay or takeover. This may change.
::

## Stuck

If you are stuck on someone else's land, `/unstuck` helps:

1. Enter `/unstuck`.
2. Stand still for five seconds. If you move or take damage, it is cancelled.
3. The game moves you to the nearest safe block outside protected areas.

- This only works on someone else's land, not on your own camp, plot or city land and not in the wilderness.
- Only in Survival mode and not in combat.
- You can only free yourself once every ten minutes.

## Commands

`<…>` and `[…]` are placeholders; `[…]` is optional, `a|b` means one of them.

- `/city`: open your city
- `/city plot`: the plot you stand on
- `/city plots`: free plots
- `/city outpost`: outposts
- `/unstuck`: free yourself from someone else's land

With `/city`:

- `view`: show borders
- `off`: hide borders
- `retry`: repeat a change with an unclear result

::page-cards
::
