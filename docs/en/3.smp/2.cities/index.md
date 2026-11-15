---
verified: 0.26.0
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
Since version 0.24.0, cities grow through tiers instead of bought capacity, and there is no upkeep any more. If you founded a city before that, read [Claims 2.0](/smp/cities#claims-20).
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

These prices apply to cities in the tier system. Older cities that have not migrated pay the old prices from [Claims 2.0](#claims-20). You always pay the moment you claim. [Outposts](/smp/cities/outposts) lists what outposts cost. The founder pays the founding price personally, see [Found a city](/smp/cities#found-a-city).

Cities in the tier system pay no upkeep. Their tier rises through play time and [tier projects](/smp/cities/tiers), not through Silver.

### Treasury history

Under **Management**, **Treasury** and **Treasury history** you see every booking of the city treasury, newest first, 8 per page.

- Each line shows the amount, currency and reason, plus the date and time.
- If someone else was involved, they are shown too, for example the player who made a deposit.
- You need the right **View treasury history**. The head always has it, and councillors have it from the start.

### Bought plots

Sold plots stay protected for their owners, even when the city is frozen.

### Dissolve a city

The head can dissolve the city.

### Older cities

For cities that have not migrated to the tier system yet, upkeep is suspended. Everything else that applies to them is under [Claims 2.0](/smp/cities#claims-20).

## Frozen cities

If no member has been active for a longer time, the city freezes. Before that, members with a linked Discord get two warnings by direct message, which include the date.

- The city stays **frozen and protected**. Land, treasury, tier, members and sold plots are kept.
- City actions, rents and the tier project pause in the meantime.
- As soon as a member is active again, the city thaws for free.

::callout{type="info"}
For now, abandoned tier cities stay frozen and protected. They do not turn into ruins, decay or get taken over. This may change.
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

::callout{type="info" title="Claims 2.0 for existing cities"}
Version 0.24.0 brought **Claims 2.0**. Since then, cities grow through [tiers](/smp/cities/tiers) instead of bought capacity and upkeep. New cities start in the tier system right away. Existing cities keep their old rules until their head moves them to the tier system.
::

::callout{type="info" title="Claims 1.x and Claims 2.0 compared"}

| Topic            | Claims 1.x (older cities)                                             | Claims 2.0 (tier system)                                     |
| :--------------- | :-------------------------------------------------------------------- | :----------------------------------------------------------- |
| Growth           | buy chunk capacity, 10,000 Silver for 4 chunks                        | 8 tiers through city hours and tier projects                 |
| Chunk limit      | starting size plus capacity, limited by the number of residents       | fixed per tier, 24 to 640 chunks                             |
| New chunk        | from bought capacity                                                  | 16,000 Silver when you claim it                              |
| Releasing chunks | not possible                                                          | possible, without refund                                     |
| Outposts         | old prices, at most 4 chunks                                          | bought one by one, number and size by tier                   |
| Upkeep           | suspended                                                             | none                                                         |
| Ranks            | Head, Assistant, Honorary citizen, Citizen, Visitor; at most 10 ranks | Head, Councillor, Resident, Guest; plus 5 to 14 custom ranks |
| City council     | head elected directly                                                 | council of 3 to 9 seats that elects its chair                |
| Dominion         | City lord, no uprising                                                | Ruler, uprising and succession on inactivity                 |
| Inactive city    | old ruins stay ruins                                                  | frozen and protected, without ruin or takeover               |

**Every** city already has: fine [rights](/smp/cities/rights), city hard locks, environment and cosmetics settings, rights for single players, co-managers, the city zone, the treasury history and messages that name the reason.
::

::callout{type="info" title="What changed for older cities right away"}

- **Upkeep:** upkeep is suspended, and outstanding arrears have been forgiven. Frozen cities in arrears are active again, and their rents run again.
- **Ruins:** cities that were already a ruin stay a ruin. Whoever takes over a ruin for 1,500 Silver gets a city in the tier system at tier 1, and the land is kept.
- **Nations and alliances** are paused, see [Nations and alliances](/smp/cities/nations). Their data and treasury are kept.
- **Plots and camps** kept their previous rights. These now appear as fixed settings in the new right groups.
  ::

::callout{type="info" title="What older cities keep without migrating"}
If you do not migrate, everything stays as it was:

- **Buy chunk capacity:** 2,500 Silver per chunk, so 10,000 Silver per expansion of 4 chunks
- The smaller of two limits applies: bought capacity, or the starting size plus 4 chunks per 2 residents.
- the old ranks with at most ten city ranks
- the old outpost rules: a new outpost costs 25,000 Silver

| Residents | max chunks (start 25) | max chunks (start 16) |
| --------- | --------------------- | --------------------- |
| 1         | 25                    | 16                    |
| 2–3       | 29                    | 20                    |
| 4–5       | 33                    | 24                    |
| 10–11     | 45                    | 36                    |
| 20–21     | 65                    | 56                    |

Tiers, tier projects, releasing single chunks, council seats, uprising and succession exist only in the tier system. If you try them in an older city, the game says: "This city must migrate to the tier system first."
::

::callout{type="info" title="Migrate to the tier system"}
Migrating is optional and has no deadline, but it cannot be undone.

1. As the head, open `/city`, then **Management** and **Migrate**.
2. Check the preview:
   - "Target tier {tier}: {name}" and your city hours
   - "Custom ranks and city rights will be reset."
   - "Land and plot contracts stay unchanged."
   - the price or "Refund to the city treasury: {amount} Silver."
3. Confirm.

Only the head may migrate, not a caretaker. The city must also not be frozen.

**Which tier you land on**

The target tier depends on the active SMP play time your current members have collected since they joined the city. You land directly on that tier and skip the projects of the tiers before it. A Metropolis still needs 15 members, though. From the moment you migrate, you start collecting new city hours.

**What migrating costs**

The game compares what your land is worth in the tier system with what your city treasury has already paid.

- **Land value:** every chunk above 16 costs 16,000 Silver. Outpost chunks count at 20,000 Silver in the Overworld and 24,000 Silver in the Nether.
- **Credited** is everything the city treasury ever paid for expansions and outposts.
- If the value is higher, the city treasury pays the difference. If there is not enough Silver, the game says: "The city treasury is missing {amount} Silver for migration."
- If you paid more, the city treasury gets the surplus back.

The treasury history lists the booking as "City tier migration".

**What stays and what starts over**

What stays:

- all your land, even above your tier's limit. You can then only claim again once you are below the limit or rise a tier.
- all plots, purchase and rental contracts and plot residents
- the city treasury and the city form

What starts over:

- All custom ranks are deleted.
- The fixed ranks Head, Resident and Guest get their default rights. With a city council, the Councillor is added.
- Every member except the head becomes a Resident.
- Rights that nations or alliances had in the city are removed.
- Running city elections are ended.

Afterwards, set up your custom ranks again as described in [Government & ranks](/smp/cities/government).
::

::callout{type="info" title="Checklist before migrating"}

- [ ] Checked the preview: target tier and price
- [ ] Enough Silver in the city treasury
- [ ] Warned members that ranks start over
- [ ] Noted custom ranks and their rights to create them again
      ::

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

::page-cards
::

::navbox{category="SMP"}
::
