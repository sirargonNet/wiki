---
verified: 0.20.0
title: 'Städte'
description: 'Gemeinsam bauen, verwalten und wachsen.'
icon: lucide:castle
---

Eine Stadt ist ein gemeinsames Gebiet aus ganzen Chunks. Ihr verwaltet sie zusammen, vergebt Ränge, haltet Wahlen ab und könnt Plots verkaufen oder vermieten.

## Stadt gründen

Zum Gründen brauchst du Netzwerk-Level 5 und 100.000 Silber. In `/city` siehst du, was dir fehlt. Die Kosten siehst du immer, bevor du bestätigst.

Du kannst nur in einer Stadt wohnen.

## Größe

Ein Chunk ist 16 × 16 Blöcke groß und reicht über die volle Höhe. Eine neue Stadt hat Platz für 16 Chunks, zum Beispiel 4 × 4 Chunks, also 64 × 64 Blöcke. Die Form bestimmt ihr selbst. Jeder neue Chunk muss mit einer Seite an einen Chunk der Stadt grenzen.

Wie viele Chunks eure Stadt belegen darf, hängt von zwei Grenzen ab. Es gilt die kleinere:

- **Gekaufte Kapazität:** die Startgröße, dazu 4 Chunks je Erweiterung.
- **Bewohner:** die Startgröße, dazu 4 Chunks je 2 Bewohner. Du als Gründer zählst mit.

| Bewohner | höchstens Chunks (Start 25) | höchstens Chunks (Start 16) |
| -------- | --------------------------- | --------------------------- |
| 1        | 25                          | 16                          |
| 2–3      | 29                          | 20                          |
| 4–5      | 33                          | 24                          |
| 10–11    | 45                          | 36                          |
| 20–21    | 65                          | 56                          |

Chunks von Außenposten zählen zu diesen Grenzen dazu. Pro Bestätigung nehmt ihr höchstens 25 Chunks dazu.

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

## Wachsen

Mit **Chunk-Kapazität kaufen** bekommt eure Stadt Platz für 4 weitere Chunks. Das kostet 2.500 Silber je Chunk, also 10.000 Silber pro Erweiterung. Bezahlt wird aus der Stadtkasse.

Mit **Aktuellen Chunk hinzufügen** nehmt ihr den Chunk, in dem du stehst, dazu. Unter **Gebietsverwaltung** siehst du die Chunks vor der Bestätigung an.

Gekaufte Kapazität könnt ihr erst nutzen, wenn ihr genug Bewohner habt. Mehr Chunks heißen auch mehr [Upkeep](/smp/cities/treasury).

## Rechte

Stadt-Ränge legen fest, wer was darf, zum Beispiel bauen, Plots verwalten, Bewohner einladen oder die Kasse nutzen. Mehr unter [Regierung und Ränge](/smp/cities/government).

## Schutz

In der Stadt schützt der Server eure Bauten. TNT und PvP sind aus, bis die Stadt sie einschaltet.

## Befehle

- `/city`: Stadt öffnen
- `/city plot`: Plot, auf dem du stehst
- `/city plots`: freie Plots
- `/city outpost`: Außenposten

Bei `/city`:

- `view`: Grenzen zeigen
- `off`: Grenzen ausblenden
- `retry`: Änderung mit unklarem Ergebnis wiederholen

::page-cards
::
