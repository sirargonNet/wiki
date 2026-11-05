---
verified: 0.21.0
title: 'Skills'
description: 'Skillpunkte, Befehle, Skillbaum und Mana.'
icon: lucide:sparkle
---

Mit SMP-XP steigst du im Level und bekommst Skillpunkte. Mit ihnen schaltest du im Skillbaum Fähigkeiten frei. Wie du XP sammelst und wie viel ein Level kostet, steht unter [Level und XP](/smp/skills/levels).

::page-cards
::

## Skillbaum

Im Skillbaum schaltest du Sterne frei. Jeder Stern kostet einen Skillpunkt. Ein Stern braucht die Stufe davor. Höhere Stufen brauchen außerdem Punkte in derselben Kategorie, gezählt über alle Fähigkeiten der Kategorie:

- Fähigkeiten mit 5 Stufen: ab Stufe III die erste Punktzahl, ab Stufe IV die zweite
- Fähigkeiten mit 8 Stufen: ab Stufe IV die erste Punktzahl, ab Stufe VI die zweite

Mit **Als Sternbild zeigen** und **In Spalten zeigen** wechselst du die Ansicht. Dieselbe Wahl findest du unter `/settings`.

## Mana

Fähigkeiten für größere Flächen lösen nur beim Schleichen aus und kosten Mana. Dein Mana steht über der Hotbar. `/skills` zeigt es dir auch.

- Ohne [Mana-Speicher](/smp/skills/overworld) hast du 50 Mana. Jede Stufe gibt 25 Mana mehr, bis 250.
- Ohne Mana-Fluss lädt dein Mana 0,5 pro Sekunde nach. Mit Mana-Fluss geht es schneller, bis 2,5 pro Sekunde.
- Dein Mana ist wieder voll, wenn du den Server betrittst, ihn verlässt oder stirbst.

| Fähigkeit    | Mana                |
| :----------- | :------------------ |
| Erzader      | 3 je weiterem Block |
| Tunnelbohrer | 2 je Block          |
| Baumfäller   | 2 je weiterem Stamm |
| Ernte-Sense  | 1 je reifer Pflanze |
| Bagger       | 1 je Block          |
| Sprint-Schub | 20                  |

Die Mana-Sterne einer Kategorie senken diese Kosten, pro Stufe um 5 %. Ist ein Block geschützt, bekommst du sein Mana zurück. Reicht dein Mana nicht mehr, stoppt die Fähigkeit. Die Blöcke bis dahin bleiben abgebaut.

## Gut zu wissen

- Fähigkeiten wirken nur im Überlebensmodus.
- Im Kampf gegen Spieler sind die Fähigkeiten aus.
- Gebietsrechte gelten für jeden einzelnen Block. Trifft eine Fähigkeit einen geschützten Block, stoppt sie dort.
- Selbst gesetzte Blöcke baut keine Fähigkeit mit ab.
- Hat dein Werkzeug nur noch 5 Haltbarkeit oder weniger, baust du nur noch einzelne Blöcke ab. So geht es nicht kaputt.
- Eine Fähigkeit läuft, solange du schleichst und dasselbe Werkzeug im selben Feld hältst. Lässt du los oder wechselst du, stoppt sie.
- Jeder Block muss höchstens 32 Blöcke von dir entfernt und geladen sein. Sonst stoppt die Fähigkeit.
- Löst du eine Fähigkeit aus, während noch eine läuft, wartet die neue. Höchstens 4 warten gleichzeitig. Stoppst du die laufende selbst, fallen die wartenden weg.
- Mit `/skills toggle` schaltest du eine Fähigkeit aus, die dich gerade stört.

## Befehle

`<…>` und `[…]` sind Platzhalter; `[…]` ist optional, `a|b` heißt: eins davon.

- `/skills`: Fähigkeiten und Mana
- `/skills tree` oder `/skilltree`: Skillbaum
- `/skills toggle <Fähigkeit>`: Fähigkeit an oder aus
- `/skills reset`: Sterne zurücksetzen

### Zurücksetzen

`/skills reset` setzt alle Sterne zurück. XP und Skillpunkte behältst du.

Das erste Zurücksetzen ist kostenlos. Danach kostet jedes weitere 2.000 Silber mehr: 2.000, 4.000, 6.000 Silber und so weiter. Den Preis siehst du vor dem Bestätigen.

Ändern wir die Werte der Skills, darfst du einmal kostenlos zurücksetzen. Danach beginnt die Preisstaffel wieder von vorn.
