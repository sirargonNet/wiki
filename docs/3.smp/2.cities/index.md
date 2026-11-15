---
verified: 0.29.0
title: 'Städte'
description: 'Gemeinsam bauen, verwalten und über acht Stufen wachsen, mit Stadtkasse und Claims 2.0.'
icon: lucide:castle
categories: ['SMP']
---

::infobox{title="Städte"}

:::infobox-row{label="Befehl" key="command"}
`/city`
:::

:::infobox-row{label="Realm" key="realm"}
[Oberwelt](/smp/realms#oberwelt)
:::

:::infobox-row{label="Kosten" key="cost"}
100.000 Silber
:::

:::infobox-row{label="Freischaltung" key="unlock"}
Netzwerk-Level 5
:::

::

Eine Stadt ist ein gemeinsames Gebiet aus ganzen Chunks in der Oberwelt. Ihr verwaltet sie zusammen, vergebt Ränge, haltet Wahlen ab und könnt Plots verkaufen oder vermieten. Zum Gründen brauchst du Netzwerk-Level 5 und 100.000 Silber. Mit eurer Spielzeit steigt die Stadt über acht [Stufen](/smp/cities/tiers) auf, von der Lichtung bis zur Metropole.

::callout{type="info" title="Claims 2.0"}
Seit Version 0.24.0 wachsen Städte über Stufen statt über gekaufte Kapazität. Es gibt keinen Upkeep mehr. Auch ältere Städte sind inzwischen alle im Stufensystem, siehe [Claims 2.0](/smp/cities#claims-20).
::

## Stadt gründen

Zum Gründen brauchst du Netzwerk-Level 5 und 100.000 Silber. Das bezahlst du selbst. In `/city` siehst du, was dir fehlt. Die Kosten siehst du immer, bevor du bestätigst.

- Im Preis sind die ersten 16 Chunks enthalten, zum Beispiel 4 × 4 Chunks, also 64 × 64 Blöcke.
- Jede neue Stadt startet auf Stufe 1, der **Lichtung**.
- Du kannst nur in einer Stadt wohnen.
- Gründest du eine Stadt, erfährt es der ganze Server: „{player} hat die Stadt {city} gegründet.“

### Aus deinem Camp

Hast du ein [Camp](/smp/camps), kannst du es direkt zur Stadt ausbauen. Wähle in `/camp` **Stadt gründen**.

- Die Camp-Chunks werden zur Stadt. Die Stadt bekommt nur diese Chunks, keine zusätzlichen 16.
- Silber, das du für Camp-Erweiterungen bezahlt hast, wird auf den Gründungspreis angerechnet. Höchstens so viel, wie die Erweiterungen deines jetzigen Camps wert sind. Der Preis fällt nie unter 0.
- Das Camp ist danach weg. Mitbewohner und Rechte werden nicht übernommen. Die Stadt startet mit Standardeinstellungen.
- Du darfst noch in keiner Stadt sein und brauchst Netzwerk-Level 5.

## Größe

Ein Chunk ist 16 × 16 Blöcke groß und reicht über die volle Höhe. Die Form bestimmt ihr selbst. Jeder neue Chunk muss mit einer Seite an einen Chunk der Stadt grenzen.

Wie viele Chunks eure Stadt haben darf, hängt von ihrer [Stufe](/smp/cities/tiers) ab: 24 auf der Lichtung, 640 als Metropole. Chunks von [Außenposten](/smp/cities/outposts) zählen dazu. Pro Bestätigung nehmt ihr höchstens 25 Chunks dazu.

Das Stadtmenü zeigt die Grenze als „{belegt} / {Grenze} · Stufe {Stufe} · {Name}“.

## Abstände

Gemessen wird waagerecht von Grenze zu Grenze. Eigene Chunks deiner Stadt grenzen direkt aneinander.

- zum Spawn: mindestens 512 Blöcke
- zu anderen Städten: mindestens 256 Blöcke
- zu Außenposten, auch deinen eigenen: mindestens 384 Blöcke
- zu verkauften Plots anderer Städte: mindestens 256 Blöcke

Festungen gehören allen. Auf einer Festung und dem Chunk um sie herum lässt sich nichts claimen, weder ein Camp noch eine Stadt oder ein Außenposten. Lag dein Land schon dort, wurde es freigegeben und der bezahlte Preis zurückerstattet. Gebaute Blöcke bleiben stehen und gehören zur Wildnis.

- zu Camps: mindestens 64 Blöcke

Städte gibt es nur in der Oberwelt.

## Beitreten und verlassen

- Eine Stadt lädt dich ein. Du nimmst die Einladung in `/city` mit **Stadt beitreten** an.
- In `/city` wählst du **Stadt verlassen**.

## Land dazunehmen

Mit **Aktuellen Chunk hinzufügen** nehmt ihr den Chunk, in dem du stehst, dazu. Jeder neue Chunk kostet 16.000 Silber aus der Stadtkasse. Bezahlt wird direkt beim Claimen. Unter **Gebietsverwaltung** siehst du die Chunks vor der Bestätigung an.

Ist die Grenze eurer Stufe erreicht, meldet das Spiel: „Die Stadt hat die Chunk-Grenze ihrer Stufe erreicht.“ Dann hilft nur die nächste Stufe.

## Land freigeben

Unter **Gebietsverwaltung** gibt **Chunk freigeben** den Chunk an deinem Standort auf. Dafür brauchst du das Recht **Stadt erweitern**, bei Außenposten **Außenposten verwalten**.

- Es gibt keine Erstattung. Neues Land kostet wieder den vollen Preis.
- Ein Chunk mit Plot lässt sich nicht freigeben.
- Die Stadt darf dadurch nicht in zwei Teile zerfallen.
- Den letzten Chunk der Stadt gibst du nicht frei. Dafür gibt es **Stadt auflösen**.
- Stehen Spawner im Chunk, zeigt die Bestätigung sie an.

## Rechte und Schutz

Stadt-Ränge legen fest, wer was darf, zum Beispiel bauen, Plots verwalten, Bewohner einladen oder die Kasse nutzen. Mehr unter [Regierung & Ränge](/smp/cities/government) und [Rechte & Plots](/smp/cities/rights).

In der Stadt schützt der Server eure Bauten. TNT und PvP sind aus, bis die Stadt sie einschaltet. Ist das [Drachenei](/smp/dragon-egg#offenes-ei) in der Stadt offen, ist dort PvP für alle an. Lehnt der Schutz eine Aktion ab, nennt die Meldung den Grund, zum Beispiel „Fehlendes Recht: {Recht} in {Gebiet}.“

## Stadtkasse

Jede Stadt hat eine Kasse. Wer das Recht hat, zahlt Silber ein oder hebt es ab. Käufe der Stadt werden erst nach Bestätigung aus der Kasse bezahlt.

### Was die Stadt bezahlt

| Kauf                                 | Preis aus der Kasse |
| :----------------------------------- | ------------------: |
| neuer Chunk der Stadt                |       16.000 Silber |
| neuer Außenposten in der Oberwelt    |       80.000 Silber |
| neuer Außenposten im Nether          |       96.000 Silber |
| weiterer Außenposten-Chunk, Oberwelt |       20.000 Silber |
| weiterer Außenposten-Chunk, Nether   |       24.000 Silber |

Bezahlt wird direkt beim Claimen. Mehr unter [Außenposten](/smp/cities/outposts). Die Gründung bezahlt der Gründer selbst, siehe [Stadt gründen](/smp/cities#stadt-gründen).

Städte zahlen keinen Upkeep. Eure Stufe steigt durch Spielzeit und [Stufenprojekte](/smp/cities/tiers), nicht durch Silber.

### Kassenverlauf

Unter **Verwaltung**, **Kasse** und **Kassenverlauf** siehst du alle Buchungen der Stadtkasse, neueste zuerst, 8 pro Seite.

- Jede Zeile nennt Betrag, Währung und Grund, dazu Datum und Uhrzeit.
- Gibt es einen Gegenpart, steht er dabei, zum Beispiel der Spieler, der eingezahlt hat.
- Dafür braucht man das Recht **Kassenverlauf ansehen**. Das Oberhaupt hat es immer, Ratsmitglieder von Anfang an.

### Gekaufte Plots

Verkaufte Plots bleiben bei ihren Besitzern geschützt, auch wenn die Stadt eingefroren ist.

### Stadt auflösen

Das Oberhaupt kann die Stadt auflösen.

## Eingefrorene Städte

Ist längere Zeit kein Mitglied aktiv, friert die Stadt ein. Mitglieder mit verknüpftem Discord bekommen vorher zwei Warnungen per Direktnachricht, mit dem Datum.

- Die Stadt bleibt **eingefroren und geschützt**. Land, Kasse, Stufe, Mitglieder und verkaufte Plots bleiben erhalten.
- Stadtaktionen, Mieten und das Stufenprojekt ruhen.
- Ist ein Mitglied wieder aktiv, taut die Stadt kostenlos auf.

::callout{type="info"}
Stand jetzt bleiben verlassene Städte eingefroren und geschützt, ohne Ruine, Zerfall oder Übernahme. Das kann sich ändern.
::

## Feststecken

Steckst du auf fremdem Land fest, hilft dir `/unstuck`:

1. Gib `/unstuck` ein.
2. Bleib fünf Sekunden still stehen. Bewegst du dich oder bekommst du Schaden, bricht es ab.
3. Das Spiel bringt dich zum nächsten sicheren Block außerhalb geschützter Gebiete.

- Das geht nur auf fremdem Land, nicht auf deinem eigenen Camp, Plot oder Stadtgebiet und nicht in der Wildnis.
- Nur im Überlebensmodus und nicht im Kampf.
- Nicht auf einem Reittier und nicht im Bett.
- Du kannst dich nur alle zehn Minuten befreien.
- Klappt es nicht, nennt dir die Meldung den Grund. Zum Beispiel lädt das Spiel gerade die Gebiete oder dein Inventar ist kurz beschäftigt.

## Claims 2.0

Mit Version 0.24.0 kam **Claims 2.0**: Städte wachsen seitdem über [Stufen](/smp/cities/tiers) statt über gekaufte Kapazität und Upkeep. Anfangs konnten ältere Städte selbst entscheiden, ob sie wechseln. Das alte System gibt es nicht mehr. Alle Städte, die noch nicht gewechselt hatten, sind automatisch ins Stufensystem gekommen.

::callout{type="info" title="Was beim automatischen Wechsel passiert ist"}

- **Kostenlos:** Die Stadtkasse hat nichts bezahlt und nichts zurückbekommen, auch wenn Silber für den alten Aufpreis gefehlt hätte. Offene Rückstände sind weggefallen.
- **Stufe:** Jede Stadt ist auf der Stufe gelandet, die sich ihre heutigen Mitglieder mit ihrer aktiven Spielzeit im SMP verdient haben, seit sie in der Stadt sind. Für die Metropole braucht es auch hier 15 Mitglieder. Ab dem Wechsel sammelt ihr neue Stadtstunden.
- **Es bleibt:** euer ganzes Land, auch über der Grenze eurer Stufe, alle Plots, Kauf- und Mietverträge, Plot-Mitbewohner, die Stadtkasse und die Stadtform. Liegt euer Land über der Grenze, könnt ihr erst wieder claimen, wenn ihr darunter seid oder aufsteigt.
- **Es startet neu:** Eigene Ränge sind gelöscht. Oberhaupt, Bewohner und Gast haben ihre Standardrechte, im Stadtrat auch das Ratsmitglied. Alle Mitglieder außer dem Oberhaupt sind Bewohner. Legt eure Ränge unter [Regierung & Ränge](/smp/cities/government) neu an.
  ::

::callout{type="info" title="Eingefrorene Städte, Ruinen und kommissarische Leitung"}
Städte, die nach den alten Regeln eingefroren oder schon eine Ruine waren, und Städte unter kommissarischer Leitung sind eingefroren ins Stufensystem gekommen. Sie bleiben [eingefroren und geschützt](#eingefrorene-städte), wie verlassene Städte im Stufensystem. Ist ein Mitglied wieder aktiv, taut die Stadt kostenlos auf. Eine Ruine hat keine Mitglieder mehr und bleibt deshalb eingefroren. Ruinen übernehmen geht nicht mehr.
::

## Befehle

`<…>` und `[…]` sind Platzhalter; `[…]` ist optional, `a|b` heißt: eins davon.

- `/city`: Stadt öffnen
- `/city plot`: Plot, auf dem du stehst
- `/city plots`: freie Plots
- `/city outpost`: Außenposten
- `/city view`: Grenzen zeigen
- `/city off`: Grenzen ausblenden
- `/city retry`: Änderung mit unklarem Ergebnis wiederholen
- `/unstuck`: dich von fremdem Land befreien

::page-cards
::

::navbox{category="SMP"}
::
