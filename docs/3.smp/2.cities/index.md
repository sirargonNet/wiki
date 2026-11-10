---
verified: 0.25.0
title: 'Städte'
description: 'Gemeinsam bauen, verwalten und über acht Stufen wachsen.'
icon: lucide:castle
categories: ['SMP']
---

Eine Stadt ist ein gemeinsames Gebiet aus ganzen Chunks. Ihr verwaltet sie zusammen, vergebt Ränge, haltet Wahlen ab und könnt Plots verkaufen oder vermieten. Mit eurer Spielzeit steigt die Stadt über acht [Stufen](/smp/cities/tiers) auf, von der Lichtung bis zur Metropole.

::callout{type="info" title="Claims 2.0"}
Seit Version 0.24.0 wachsen Städte über Stufen statt über gekaufte Kapazität. Es gibt keinen Upkeep mehr. Hast du schon vorher eine Stadt gegründet, lies [Claims 2.0 für bestehende Städte](/smp/cities/claims-2).
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

Stadt-Ränge legen fest, wer was darf, zum Beispiel bauen, Plots verwalten, Bewohner einladen oder die Kasse nutzen. Mehr unter [Regierung und Ränge](/smp/cities/government) und [Rechte und Gebietseinstellungen](/smp/cities/rights).

In der Stadt schützt der Server eure Bauten. TNT und PvP sind aus, bis die Stadt sie einschaltet. Lehnt der Schutz eine Aktion ab, nennt die Meldung den Grund, zum Beispiel „Fehlendes Recht: {Recht} in {Gebiet}.“

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

## Befehle

`<…>` und `[…]` sind Platzhalter; `[…]` ist optional, `a|b` heißt: eins davon.

- `/city`: Stadt öffnen
- `/city plot`: Plot, auf dem du stehst
- `/city plots`: freie Plots
- `/city outpost`: Außenposten
- `/unstuck`: dich von fremdem Land befreien

Bei `/city`:

- `view`: Grenzen zeigen
- `off`: Grenzen ausblenden
- `retry`: Änderung mit unklarem Ergebnis wiederholen

::page-cards
::

::navbox{category="SMP"}
::
