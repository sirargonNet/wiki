---
verified: 0.29.0
title: 'Cities'
description: 'Build, manage and rise through eight tiers together, with treasury and Claims 2.0.'
icon: lucide:castle
categories: ['SMP', 'Commands', 'Economy']
---

::infobox{title="Cities"}

:::infobox-row{label="Command" key="command"}
`/city`
:::

:::infobox-row{label="Realm" key="realm"}
[Overworld](/smp/realms#overworld)
:::

:::infobox-row{label="Cost" key="cost"}
100,000 Silver
:::

:::infobox-row{label="Unlock" key="unlock"}
Network level 5
:::

::

A city is a shared territory made of whole chunks in the Overworld. You run it together, hand out ranks, hold elections and can sell or rent out plots. As you play, your city rises through eight [tiers](/smp/cities/tiers), from Clearing to Metropolis.

::callout{type="info" title="Claims 2.0"}
Since version 0.24.0, cities grow through tiers instead of bought capacity, and there is no upkeep any more. Older cities have all moved into the tier system by now, and [Claims 2.0](/smp/cities#claims-20) explains what happened to them.
::

## Found a city

To found a city you need network level 5 and 100,000 Silver, which you pay yourself. `/city` shows you what you are still missing, and you always see the cost before you confirm.

- The price includes the first 16 chunks, for example 4 × 4 chunks, which is 64 × 64 blocks.
- Every new city starts at tier 1, the **Clearing**.
- You can only live in one city.
- When you found a city, the whole server hears about it: "{player} founded the city {city}."

### From your camp

If you have a [camp](/smp/camps), you can turn it straight into a city. Choose **Found city** in `/camp`. You need network level 5 and must not be in a city yet.

- The camp chunks become the city. The city gets only these chunks, not an extra 16.
- Silver you paid for camp expansions counts towards the founding price, but at most what the expansions of your current camp are worth. The price never drops below 0.
- The camp is gone afterwards. Residents and rights are not carried over, and the city starts with default settings.

## Size

A chunk is 16 × 16 blocks and covers the full height. You decide the shape of your city, as long as every new chunk shares a side with a chunk of the city.

How many chunks your city may have depends on its [tier](/smp/cities/tiers): 24 as a Clearing, 640 as a Metropolis. Chunks of [outposts](/smp/cities/outposts) count too. Each confirmation adds at most 25 chunks.

The city menu shows the limit as "{occupied} / {limit} · Tier {tier} · {name}".

## Distances

Distances are measured horizontally from border to border. Chunks of your own city border each other directly.

- to spawn: at least 512 blocks
- to other cities: at least 256 blocks
- to outposts, including your own: at least 384 blocks
- to sold plots of other cities: at least 256 blocks
- to camps: at least 64 blocks

Strongholds belong to everyone. Nothing can be claimed on a stronghold or the chunk around it: not a camp, not a city and not an outpost. If your land was already there, it was released and the price you paid was refunded. Anything built there stays standing and is now wilderness.

Cities exist only in the Overworld.

## Join and leave

- A city invites you, and you accept the invitation in `/city` with **Join city**.
- To leave, choose **Leave city** in `/city`.

## Add land

**Add current chunk** adds the chunk you are standing in. Every new chunk costs 16,000 Silver from the city treasury, paid the moment you claim it. Under **Land management** you can look at the chunks before you confirm.

Once your tier's limit is reached, the game says: "Your city has reached its tier’s chunk limit." From then on, only the next tier gets you more land.

## Release land

Under **Land management**, **Release chunk** gives up the chunk you are standing in. You need the right **Expand city**, or **Manage outposts** for outposts.

- You get nothing back, and new land costs the full price again.
- You cannot release a chunk with a plot in it.
- The city must not split into two parts.
- You cannot release the city's last chunk. Use **Dissolve city** instead.
- If there are spawners in the chunk, the confirmation lists them.

## Rights and protection

City ranks decide who may do what, for example build, manage plots, invite residents or use the treasury. [Government & ranks](/smp/cities/government) and [Rights & plots](/smp/cities/rights) explain how that works in detail.

Inside the city, the server protects your builds. TNT and PvP stay off until the city turns them on. While the [dragon egg](/smp/dragon-egg#open-egg) is open in the city, PvP is on for everyone there. When protection blocks something, the message tells you why, for example "Missing right: {right} in {area}."

## Treasury

Every city has a treasury. Anyone with the right can deposit or withdraw Silver. The treasury only pays for city purchases once you confirm them.

### What the city pays for

| Purchase                         | Price from the treasury |
| :------------------------------- | ----------------------: |
| new city chunk                   |           16,000 Silver |
| new outpost in the Overworld     |           80,000 Silver |
| new outpost in the Nether        |           96,000 Silver |
| further outpost chunk, Overworld |           20,000 Silver |
| further outpost chunk, Nether    |           24,000 Silver |

You always pay the moment you claim. [Outposts](/smp/cities/outposts) lists what outposts cost. The founder pays the founding price personally, see [Found a city](/smp/cities#found-a-city).

Cities pay no upkeep. Their tier rises through play time and [tier projects](/smp/cities/tiers), not through Silver.

### Treasury history

Under **Management**, **Treasury** and **Treasury history** you see every booking of the city treasury, newest first, 8 per page.

- Each line shows the amount, currency and reason, plus the date and time.
- If someone else was involved, they are shown too, for example the player who made a deposit.
- You need the right **View treasury history**. The head always has it, and councillors have it from the start.

### Bought plots

Sold plots stay protected for their owners, even when the city is frozen.

### Dissolve a city

The head can dissolve the city.

## Frozen cities

If no member has been active for a longer time, the city freezes. Before that, members with a linked Discord get two warnings by direct message, which include the date.

- The city stays **frozen and protected**. Land, treasury, tier, members and sold plots are kept.
- City actions, rents and the tier project pause in the meantime.
- As soon as a member is active again, the city thaws for free.

::callout{type="info"}
For now, abandoned cities stay frozen and protected. They do not turn into ruins, decay or get taken over. This may change.
::

## Stuck

If you are stuck on someone else's land, `/unstuck` gets you out:

1. Enter `/unstuck`.
2. Stand still for five seconds. If you move or take damage, it is cancelled.
3. The game then moves you to the nearest safe block outside protected areas.

- This only works on someone else's land, so not on your own camp, plot or city land, and not in the wilderness.
- It only works in Survival mode and not in combat.
- It does not work on a mount or in bed.
- You can only free yourself once every ten minutes.
- If it does not work, the message tells you why, for example because the game is still loading the territories or your inventory is busy for a moment.

## Claims 2.0

Version 0.24.0 brought **Claims 2.0**. Since then, cities grow through [tiers](/smp/cities/tiers) instead of bought capacity and upkeep. At first, older cities could choose for themselves when to migrate. The old system is gone now, and every city that had not migrated by then was moved into the tier system automatically.

That move was free. The city treasury paid nothing and got nothing back, even if it would have been short of Silver for the old migration price, and any outstanding arrears were dropped.

Your city landed on the tier its current members earned with their active SMP play time since they joined it. A Metropolis still needs 15 members, though. From the move onwards, you collect new city hours.

You kept all your land, even the part above your tier's limit. In that case you can only claim again once you are below the limit or rise a tier. You also kept every plot with its purchase and rental contracts and plot residents, the city treasury and the city form.

The ranks, on the other hand, started over:

- Your custom ranks were deleted. Set them up again under [Government & ranks](/smp/cities/government).
- Head, Resident and Guest have their default rights again, and so does the Councillor in a city council.
- Every member except the head is now a Resident.
- Running city elections were ended.

## Commands

`<…>` and `[…]` are placeholders; `[…]` is optional, `a|b` means one of them.

- `/city`: open your city
- `/city plot`: the plot you are standing on
- `/city plots`: free plots
- `/city outpost`: outposts
- `/city view`: show borders
- `/city off`: hide borders
- `/city retry`: repeat a change with an unclear result
- `/unstuck`: free yourself from someone else's land

## Frequently asked questions

### Why is my old city frozen after the move?

If the old rules had already frozen it or turned it into a ruin, or a caretaker was leading it, it entered the tier system frozen. It then stays [frozen and protected](#frozen-cities) like any abandoned city, and thaws for free as soon as a member is active again.

### Can I still take over a ruin?

No. A ruin has no members left, so it stays frozen and protected.

::page-cards
::

::navbox{category="SMP"}
::
