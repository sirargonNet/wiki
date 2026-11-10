---
verified: 0.26.0
title: 'Cities'
description: 'Build, manage and rise through eight tiers together, with treasury and Claims 2.0.'
icon: lucide:castle
categories: ['SMP']
---

::infobox{title="Cities"}

:::infobox-row{label="Command" key="command"}
`/city`
:::

:::infobox-row{label="Realm" key="realm"}
Overworld
:::

:::infobox-row{label="Cost" key="cost"}
100,000 Silver
:::

:::infobox-row{label="Unlock" key="unlock"}
Network level 5
:::

::

A city is a shared territory made of whole chunks in the Overworld. You manage it together, assign ranks, hold elections and can sell or rent out plots. To found one, you need network level 5 and 100,000 silver. Through your play time the city rises through eight [tiers](/smp/cities/tiers), from Clearing to Metropolis.

::callout{type="info" title="Claims 2.0"}
Since version 0.24.0 cities grow through tiers instead of bought capacity. There is no upkeep any more. If you founded a city before, read [Claims 2.0](/smp/cities#claims-20).
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

- A city invites you. You accept the invitation in `/city` with **Join city**.
- In `/city` choose **Leave city**.

## Add land

**Add current chunk** adds the chunk you stand in. Every new chunk costs 16,000 Silver from the city treasury. It is paid right when you claim it. Under **Land management** you can check the chunks before you confirm.

When your tier's limit is reached, the game says: "Your city has reached its tier’s chunk limit." Only the next tier helps then.

## Release land

Under **Land management**, **Release chunk** gives up the chunk you stand in. You need the right **Expand city**, for outposts **Manage outposts**.

- There is no refund. New land costs the full price again.
- A chunk containing a plot cannot be released.
- The city must not split into two parts.
- You cannot release the city's last chunk. Use **Dissolve city** instead.
- If spawners stand in the chunk, the confirmation lists them.

## Rights and protection

City ranks decide who may do what, for example build, manage plots, invite residents or use the treasury. See [Government & ranks](/smp/cities/government) and [Rights & plots](/smp/cities/rights).

Inside the city the server protects your builds. TNT and PvP are off until the city turns them on. When protection refuses an action, the message names the reason, for example "Missing right: {right} in {area}."

## Treasury

Every city has a treasury. Anyone with the right deposits or withdraws Silver. City purchases are only paid from the treasury after confirmation.

### What the city pays for

| Purchase                         | Price from the treasury |
| :------------------------------- | ----------------------: |
| new city chunk                   |           16,000 Silver |
| new outpost in the Overworld     |           80,000 Silver |
| new outpost in the Nether        |           96,000 Silver |
| further outpost chunk, Overworld |           20,000 Silver |
| further outpost chunk, Nether    |           24,000 Silver |

These prices apply to cities in the tier system. Older cities that have not migrated pay the old prices, see [Claims 2.0](#claims-20). It is paid right when you claim. See [Outposts](/smp/cities/outposts). The founder pays the founding price personally, see [Found a city](/smp/cities#found-a-city).

Cities in the tier system pay no upkeep. Your tier rises through play time and [tier projects](/smp/cities/tiers), not through Silver.

### Treasury history

Under **Management**, **Treasury** and **Treasury history** you see every city treasury booking, newest first, 8 per page.

- Each line names the amount, currency and reason, plus the date and time.
- If there is another party, it is shown, for example the player who deposited.
- This needs the right **View treasury history**. The head always has it, councillors from the start.

### Bought plots

Sold plots stay protected for their owners, even when the city is frozen.

### Dissolve a city

The head can dissolve the city.

### Older cities

For cities that have not migrated to the tier system yet, upkeep is suspended. What else applies to them is under [Claims 2.0](/smp/cities#claims-20).

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
- Not on a mount and not in bed.
- You can only free yourself once every ten minutes.
- If it does not work, the message tells you why. For example, the game is still loading the territories or your inventory is busy for a moment.

## Claims 2.0

::callout{type="info" title="Claims 2.0 for existing cities"}
Version 0.24.0 brought **Claims 2.0**. Cities now grow through [tiers](/smp/cities/tiers) instead of bought capacity and upkeep. New cities start in the tier system right away. Existing cities keep their old rules until their head migrates.
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

- **Upkeep:** upkeep is suspended. Outstanding arrears have been forgiven. Frozen cities in arrears are active again, and their rents run again.
- **Ruins:** cities that were already a ruin stay a ruin. Whoever takes over a ruin for 1,500 Silver gets a city in the tier system at tier 1. The land is kept.
- **Nations and alliances** are paused, see [Nations and alliances](/smp/cities/nations). Their data and treasury are kept.
- **Plots and camps** kept their previous rights. They now appear as fixed settings in the new right groups.
  ::

::callout{type="info" title="What older cities keep without migrating"}
If you do not migrate, everything stays as before:

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
Migrating is optional. There is no deadline. It cannot be undone, though.

1. As the head, open `/city`, then **Management** and **Migrate**.
2. Check the preview:
   - "Target tier {tier}: {name}" and your city hours
   - "Custom ranks and city rights will be reset."
   - "Land and plot contracts stay unchanged."
   - the price or "Refund to the city treasury: {amount} Silver."
3. Confirm.

Only the head may migrate, not a caretaker. The city must not be frozen.

**Which tier you land on**

The target tier depends on the active SMP play time your current members collected since they joined the city. You land directly on that tier, without the projects of the tiers before. A Metropolis still needs 15 members. After migrating, you collect new city hours from the moment of the migration.

**What migrating costs**

The game compares the value of your land in the tier system with what your city treasury has already paid.

- **Land value:** every chunk above 16 costs 16,000 Silver. Outpost chunks count at 20,000 Silver in the Overworld and 24,000 Silver in the Nether.
- **Credited** is everything the city treasury ever paid for expansions and outposts.
- If the value is higher, the city treasury pays the difference. If Silver is missing, the game says: "The city treasury is missing {amount} Silver for migration."
- If you paid more, the city treasury gets the surplus back.

The treasury history lists the booking as "City tier migration".

**What stays and what starts over**

What stays:

- all your land, even above your tier's limit. Then you can only claim again once you are below the limit or rise a tier.
- all plots, purchase and rental contracts and plot residents
- the city treasury and the city form

What starts over:

- All custom ranks are deleted.
- The fixed ranks Head, Resident and Guest get their default rights. A city council also gets the Councillor.
- Every member except the head becomes a Resident.
- Rights that nations or alliances had in the city are removed.
- Running city elections are ended.

Create your custom ranks again afterwards, see [Government & ranks](/smp/cities/government).
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
- `/city plot`: the plot you stand on
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
