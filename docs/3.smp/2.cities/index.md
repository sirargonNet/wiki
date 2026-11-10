---
verified: 0.24.0
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
Oberwelt
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
Seit Version 0.24.0 wachsen Städte über Stufen statt über gekaufte Kapazität. Es gibt keinen Upkeep mehr. Hast du schon vorher eine Stadt gegründet, lies [Claims 2.0](/smp/cities#claims-20).
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
- zu Camps: mindestens 64 Blöcke

Städte gibt es nur in der Oberwelt.

## Beitreten und verlassen

- Eine Stadt lädt dich ein. Du nimmst die Einladung in `/city` an.
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

In der Stadt schützt der Server eure Bauten. TNT und PvP sind aus, bis die Stadt sie einschaltet. Lehnt der Schutz eine Aktion ab, nennt die Meldung den Grund, zum Beispiel „Fehlendes Recht: {Recht} in {Gebiet}.“

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

Diese Preise gelten für Städte im Stufensystem. Alte Städte ohne Wechsel zahlen die alten Preise, siehe [Claims 2.0](#claims-20). Bezahlt wird direkt beim Claimen. Mehr unter [Außenposten](/smp/cities/outposts). Die Gründung bezahlt der Gründer selbst, siehe [Stadt gründen](/smp/cities#stadt-gründen).

Städte im Stufensystem zahlen keinen Upkeep. Eure Stufe steigt durch Spielzeit und [Stufenprojekte](/smp/cities/tiers), nicht durch Silber.

### Kassenverlauf

Unter **Verwaltung**, **Kasse** und **Kassenverlauf** siehst du alle Buchungen der Stadtkasse, neueste zuerst, 8 pro Seite.

- Jede Zeile nennt Betrag, Währung und Grund, dazu Datum und Uhrzeit.
- Gibt es einen Gegenpart, steht er dabei, zum Beispiel der Spieler, der eingezahlt hat.
- Dafür braucht man das Recht **Kassenverlauf ansehen**. Das Oberhaupt hat es immer, Ratsmitglieder von Anfang an.

### Gekaufte Plots

Verkaufte Plots bleiben bei ihren Besitzern geschützt, auch wenn die Stadt eingefroren ist.

### Stadt auflösen

Das Oberhaupt kann die Stadt auflösen.

### Alte Städte

Für Städte, die noch nicht ins Stufensystem gewechselt haben, ist der Upkeep ausgesetzt. Was sonst für sie gilt, steht unter [Claims 2.0](/smp/cities#claims-20).

## Eingefrorene Städte

Ist längere Zeit kein Mitglied aktiv, friert die Stadt ein. Mitglieder mit verknüpftem Discord bekommen vorher zwei Warnungen per Direktnachricht, mit dem Datum.

- Die Stadt bleibt **eingefroren und geschützt**. Land, Kasse, Stufe, Mitglieder und verkaufte Plots bleiben erhalten.
- Stadtaktionen, Mieten und das Stufenprojekt ruhen.
- Ist ein Mitglied wieder aktiv, taut die Stadt kostenlos auf.

::callout{type="info"}
Stand jetzt bleiben verlassene Städte im Stufensystem eingefroren und geschützt, ohne Ruine, Zerfall oder Übernahme. Das kann sich ändern.
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

::callout{type="info" title="Claims 2.0 für bestehende Städte"}
Mit Version 0.24.0 kam **Claims 2.0**. Städte wachsen jetzt über [Stufen](/smp/cities/tiers) statt über gekaufte Kapazität und Upkeep. Neue Städte starten direkt im Stufensystem. Bestehende Städte behalten ihre alten Regeln, bis ihr Oberhaupt wechselt.
::

::callout{type="info" title="Claims 1.x und Claims 2.0 im Vergleich"}

| Thema            | Claims 1.x (alte Städte)                                                | Claims 2.0 (Stufensystem)                                           |
| :--------------- | :---------------------------------------------------------------------- | :------------------------------------------------------------------ |
| Wachstum         | Chunk-Kapazität kaufen, 10.000 Silber für 4 Chunks                      | 8 Stufen durch Stadtstunden und Stufenprojekte                      |
| Chunk-Grenze     | Startgröße plus Kapazität, begrenzt durch die Bewohnerzahl              | fest pro Stufe, 24 bis 640 Chunks                                   |
| Neuer Chunk      | aus der gekauften Kapazität                                             | 16.000 Silber beim Claimen                                          |
| Chunks freigeben | geht nicht                                                              | geht, ohne Erstattung                                               |
| Außenposten      | alte Preise, höchstens 4 Chunks                                         | einzeln gekauft, Anzahl und Größe nach Stufe                        |
| Upkeep           | ausgesetzt                                                              | gibt es nicht                                                       |
| Ränge            | Oberhaupt, Assistent, Ehrenbürger, Bürger, Besucher; höchstens 10 Ränge | Oberhaupt, Ratsmitglied, Bewohner, Gast; dazu 5 bis 14 eigene Ränge |
| Stadtrat         | Oberhaupt direkt gewählt                                                | Rat mit 3 bis 9 Sitzen, der den Vorsitz wählt                       |
| Herrschaft       | Stadtherr, kein Aufstand                                                | Herrscher, Aufstand und Nachfolge bei Inaktivität                   |
| Inaktive Stadt   | alte Ruinen bleiben Ruinen                                              | eingefroren und geschützt, ohne Ruine oder Übernahme                |

Für **alle** Städte gelten schon jetzt: feine [Rechte](/smp/cities/rights), Stadtsperren, Umwelt- und Cosmetics-Einstellungen, Rechte für einzelne Spieler, Mitverwalter, die Stadtzone, der Kassenverlauf und Meldungen mit Grund.
::

::callout{type="info" title="Was sich für alte Städte sofort geändert hat"}

- **Upkeep:** Der Upkeep ist ausgesetzt. Offene Rückstände wurden erlassen. Eingefrorene Städte im Rückstand sind wieder aktiv, ihre Mieten laufen wieder.
- **Ruinen:** Städte, die schon eine Ruine waren, bleiben eine Ruine. Wer eine Ruine für 1.500 Silber übernimmt, bekommt eine Stadt im Stufensystem auf Stufe 1. Das Land bleibt erhalten.
- **Nationen und Allianzen** sind pausiert, siehe [Nationen und Allianzen](/smp/cities/nations). Ihre Daten und ihre Kasse bleiben erhalten.
- **Plots und Camps** haben ihre bisherigen Rechte behalten. Sie stehen jetzt als feste Einstellungen in den neuen Rechtegruppen.
  ::

::callout{type="info" title="Was alte Städte ohne Wechsel behalten"}
Wechselt ihr nicht, bleibt alles wie bisher:

- **Chunk-Kapazität kaufen:** 2.500 Silber je Chunk, also 10.000 Silber pro Erweiterung um 4 Chunks
- Es gilt die kleinere von zwei Grenzen: die gekaufte Kapazität oder die Startgröße plus 4 Chunks je 2 Bewohner.
- die alten Ränge mit höchstens zehn Stadt-Rängen
- die alten Regeln für Außenposten: ein neuer Außenposten kostet 25.000 Silber

| Bewohner | höchstens Chunks (Start 25) | höchstens Chunks (Start 16) |
| -------- | --------------------------- | --------------------------- |
| 1        | 25                          | 16                          |
| 2–3      | 29                          | 20                          |
| 4–5      | 33                          | 24                          |
| 10–11    | 45                          | 36                          |
| 20–21    | 65                          | 56                          |

Stufen, Stufenprojekte, das Freigeben einzelner Chunks, Ratssitze, Aufstand und Nachfolge gibt es nur im Stufensystem. Versuchst du es in einer alten Stadt, sagt das Spiel: „Diese Stadt muss zuerst ins Stufensystem wechseln.“
::

::callout{type="info" title="Ins Stufensystem wechseln"}
Der Wechsel ist freiwillig. Es gibt keine Frist. Er lässt sich aber nicht rückgängig machen.

1. Öffne als Oberhaupt `/city`, dann **Verwaltung** und **Wechseln**.
2. Prüfe die Vorschau:
   - „Zielstufe {Stufe}: {Name}“ und eure Stadtstunden
   - „Eigene Ränge und Stadtrechte werden zurückgesetzt.“
   - „Land und Plot-Verträge bleiben unverändert.“
   - den Preis oder „Erstattung in die Stadtkasse: {Betrag} Silber.“
3. Bestätige.

Wechseln darf nur das Oberhaupt selbst, keine kommissarische Leitung. Die Stadt darf nicht eingefroren sein.

**Auf welcher Stufe ihr landet**

Die Zielstufe richtet sich nach der aktiven Spielzeit, die eure heutigen Mitglieder im SMP gesammelt haben, seit sie in der Stadt sind. Ihr landet direkt auf dieser Stufe, ohne die Projekte der Stufen davor. Für die Metropole braucht ihr auch hier 15 Mitglieder. Nach dem Wechsel sammelt ihr neue Stadtstunden ab dem Zeitpunkt des Wechsels.

**Was der Wechsel kostet**

Das Spiel vergleicht den Wert eures Landes im Stufensystem mit dem, was eure Stadtkasse schon bezahlt hat.

- **Wert des Landes:** jeder Chunk über 16 kostet 16.000 Silber. Außenposten-Chunks zählen mit 20.000 Silber in der Oberwelt und 24.000 Silber im Nether.
- **Angerechnet** wird alles, was die Stadtkasse je für Erweiterungen und Außenposten bezahlt hat.
- Ist der Wert höher, zahlt die Stadtkasse den Unterschied. Fehlt Silber, meldet das Spiel: „Der Stadtkasse fehlen {Betrag} Silber für den Wechsel.“
- Habt ihr mehr bezahlt, bekommt die Stadtkasse den Überschuss zurück.

Im Kassenverlauf steht die Buchung als „Wechsel ins Stadtsystem“.

**Was bleibt und was neu startet**

Es bleibt:

- euer ganzes Land, auch wenn es über der Grenze eurer Stufe liegt. Dann könnt ihr erst wieder claimen, wenn ihr unter der Grenze seid oder aufsteigt.
- alle Plots, Kauf- und Mietverträge und Plot-Mitbewohner
- die Stadtkasse und die Stadtform

Es startet neu:

- Alle eigenen Ränge werden gelöscht.
- Die festen Ränge Oberhaupt, Bewohner und Gast bekommen ihre Standardrechte. Im Stadtrat kommt das Ratsmitglied dazu.
- Alle Mitglieder außer dem Oberhaupt werden Bewohner.
- Rechte, die Nationen oder Allianzen in der Stadt hatten, werden entfernt.
- Laufende Stadtwahlen werden beendet.

Legt eure eigenen Ränge danach neu an, siehe [Regierung & Ränge](/smp/cities/government).
::

::callout{type="info" title="Checkliste vor dem Wechsel"}

- [ ] Vorschau geprüft: Zielstufe und Preis
- [ ] genug Silber in der Stadtkasse
- [ ] Mitglieder vorgewarnt, dass Ränge neu starten
- [ ] eigene Ränge und ihre Rechte notiert, um sie neu anzulegen
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
