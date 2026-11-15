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
[Overworld](/smp/realms#overworld)
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
Since version 0.24.0 cities grow through tiers instead of bought capacity. There is no upkeep any more. Older cities are all in the tier system now too, see [Claims 2.0](/smp/cities#claims-20).
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

Strongholds belong to everyone. Nothing can be claimed on a stronghold or the chunk around it, neither a camp nor a city or an outpost. If your land was already there, it was released and the price you paid was refunded. Built blocks stay and become wilderness.

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

Inside the city the server protects your builds. TNT and PvP are off until the city turns them on. While the [dragon egg](/smp/dragon-egg#open-egg) is open in the city, PvP is on for everyone there. When protection refuses an action, the message names the reason, for example "Missing right: {right} in {area}."

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

It is paid right when you claim. See [Outposts](/smp/cities/outposts). The founder pays the founding price personally, see [Found a city](/smp/cities#found-a-city).

Cities pay no upkeep. Your tier rises through play time and [tier projects](/smp/cities/tiers), not through Silver.

### Treasury history

Under **Management**, **Treasury** and **Treasury history** you see every city treasury booking, newest first, 8 per page.

- Each line names the amount, currency and reason, plus the date and time.
- If there is another party, it is shown, for example the player who deposited.
- This needs the right **View treasury history**. The head always has it, councillors from the start.

### Bought plots

Sold plots stay protected for their owners, even when the city is frozen.

### Dissolve a city

The head can dissolve the city.

## Frozen cities

When no member has been active for a longer time, the city freezes. Members with a linked Discord get two warnings by direct message before that, with the date.

- The city stays **frozen and protected**. Land, treasury, tier, members and sold plots are kept.
- City actions, rents and the tier project pause.
- When a member is active again, the city thaws for free.

::callout{type="info"}
For now, abandoned cities stay frozen and protected, without ruin, decay or takeover. This may change.
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

Version 0.24.0 brought **Claims 2.0**: since then cities grow through [tiers](/smp/cities/tiers) instead of bought capacity and upkeep. At first, older cities could choose whether to switch. The old system is gone now. Every city that had not switched yet was moved into the tier system automatically.

::callout{type="info" title="What the automatic switch did"}

- **Free of charge:** The city treasury paid nothing and got nothing back, even if it could not have covered the old price difference. Outstanding arrears were dropped.
- **Tier:** Each city landed on the tier its current members earned with their active SMP play time since they joined it. The Metropolis still needs 15 members. From the switch on you collect new city hours.
- **What stays:** all your land, even above your tier's limit, every plot, sale and rent contract, plot co-residents, the treasury and the city form. If your land is above the limit, you can claim again once you are below it or rise a tier.
- **What starts over:** Custom ranks are deleted. Head, resident and guest have their default rights, and in a council the councillor too. Every member except the head is a resident. Set up your ranks again under [Government & ranks](/smp/cities/government).
  ::

::callout{type="info" title="Frozen cities, ruins and caretaker governments"}
Cities that the old rules had frozen or turned into a ruin, and cities run by a caretaker government, entered the tier system frozen. They stay [frozen and protected](#frozen-cities), just like abandoned cities in the tier system. As soon as a member is active again, the city thaws for free. A ruin has no members left, so it stays frozen. Ruins can no longer be taken over.
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
