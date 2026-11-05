---
verified: 0.21.0
title: 'Quests'
description: 'Tägliche und wöchentliche Quests, Belohnungen und Abliefern.'
icon: lucide:scroll-text
---

`/quests` zeigt deine täglichen und wöchentlichen Quests. Links stehen die Tagesquests, rechts die Wochenquests. Jedes [Realm](/smp/realms) hat eine eigene Reihe. Die Farbe der Felder zeigt das Realm: grün die Oberwelt, rot der Nether.

Jede Quest zeigt ihre Schwierigkeit, ihr Ziel, deinen Fortschritt, die Belohnung und die Zeit bis zum Ende.

::page-cards
::

## So werden Quests gezogen

- Alle Spieler haben dieselben Quests.
- Tagesquests kommen jeden Tag um Mitternacht (deutsche Zeit).
- Wochenquests kommen jeden Montag um Mitternacht.
- Jede Art von Quest, zum Beispiel Holz oder Kampf, kommt pro Tag und Realm möglichst nur einmal vor.
- Zwei Quests haben nie dasselbe Ziel.
- Dieselbe Tagesquest kommt in der Regel erst nach einer Woche wieder. Dieselbe Wochenquest kommt in der Regel erst nach vier Wochen wieder.

| Realm                             | Tagesquests                         | Wochenquests                       |
| :-------------------------------- | :---------------------------------- | :--------------------------------- |
| [Oberwelt](/smp/quests/overworld) | 5: 2 leichte, 2 mittlere, 1 schwere | 3: je 1 leichte, mittlere, schwere |
| [Nether](/smp/quests/nether)      | 3: je 1 leichte, mittlere, schwere  | 3: je 1 leichte, mittlere, schwere |

## Nether-Quests

Die Nether-Quests bekommst du zusätzlich zu deinen Oberwelt-Quests. Du siehst sie, sobald du den Nether zum ersten Mal betreten hast. Dann bekommst du die Nachricht **Du hast den Nether betreten: Neue Nether-Quests sind jetzt freigeschaltet.** Ab da hat `/quests` eine Reihe für den Nether.

## Ziel des Tages

Manche Quests wählen ein Ziel des Tages, zum Beispiel eine bestimmte Holzart. Die Quest zeigt es dir als **Heute: …**. Wie viel du brauchst, hängt vom Ziel ab.

## Kills

Bei Kill-Quests zählt ein Mob für den Spieler, der ihm den meisten Schaden gemacht hat. Bei Gleichstand zählt er für den, der zuletzt getroffen hat. So zählen Kills auch, wenn ihr zusammen kämpft.

## Belohnungen

| Quest       |       Leicht |       Mittel |        Schwer |
| :---------- | -----------: | -----------: | ------------: |
| täglich     | 1.000 Silber | 2.000 Silber |  3.000 Silber |
| wöchentlich | 3.000 Silber | 6.000 Silber | 12.000 Silber |

Quests im Nether bringen 25 % mehr:

| Nether-Quest |       Leicht |       Mittel |        Schwer |
| :----------- | -----------: | -----------: | ------------: |
| täglich      | 1.250 Silber | 2.500 Silber |  3.750 Silber |
| wöchentlich  | 3.750 Silber | 7.500 Silber | 15.000 Silber |

## Abliefern

Bei manchen Quests lieferst du Items ab, zum Beispiel Brot oder Eisenbarren.

1. Öffne `/quests`.
2. Klick bei der Quest auf **Zum Abliefern auswählen**.
3. Klick passende Items in deinem Inventar an. Sie werden verbraucht.

## World Quest

Zusätzlich gibt es eine gemeinsame **World Quest**. Öffne `/quests`. Unter deinen persönlichen Quests steht direkt der Bereich **World Quest**. Alle helfen mit Rohstoffen. Die [Anleitung und Belohnungen](/smp/quests/world-quest) erklären die Abgabe.

Neue Tagesquests bringen seit 0.21.0 die oben genannten Belohnungen. Bereits gezogene Quests behalten ihre Werte. Die Umstellung gilt ab der nächsten täglichen Ziehung oder einer später geplanten Freigabe. Im Zweifel gilt dein Quest-Menü.

## Befehle

- `/quests`: Quests
