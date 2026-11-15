---
verified: 0.29.0
title: 'Städte'
description: 'Gemeinsam bauen, verwalten und über acht Stufen wachsen, mit Stadtkasse und Claims 2.0.'
icon: lucide:castle
categories: ['SMP', 'Befehle', 'Wirtschaft']
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

Eine Stadt ist ein gemeinsames Gebiet aus ganzen Chunks in der Oberwelt. Ihr verwaltet sie zusammen, vergebt Ränge, haltet Wahlen ab und könnt Plots verkaufen oder vermieten. Mit eurer Spielzeit steigt die Stadt über acht [Stufen](/smp/cities/tiers) auf, von der Lichtung bis zur Metropole.

::callout{type="info" title="Claims 2.0"}
Seit Version 0.24.0 wachsen Städte über Stufen statt über gekaufte Kapazität, und Upkeep gibt es keinen mehr. Ältere Städte sind inzwischen auch alle im Stufensystem. Was dabei mit ihnen passiert ist, steht unter [Claims 2.0](/smp/cities#claims-20).
::

## Stadt gründen

Zum Gründen brauchst du Netzwerk-Level 5 und 100.000 Silber, die du selbst bezahlst. Was dir noch fehlt, zeigt dir `/city`, und die Kosten siehst du immer, bevor du bestätigst.

- Im Preis sind die ersten 16 Chunks enthalten, zum Beispiel 4 × 4 Chunks, also 64 × 64 Blöcke.
- Jede neue Stadt startet auf Stufe 1, der **Lichtung**.
- Du kannst nur in einer Stadt wohnen.
- Gründest du eine Stadt, erfährt es der ganze Server: „{player} hat die Stadt {city} gegründet.“

### Aus deinem Camp

Hast du ein [Camp](/smp/camps), kannst du es direkt zur Stadt ausbauen. Wähle dafür in `/camp` **Stadt gründen**. Du brauchst Netzwerk-Level 5 und darfst noch in keiner Stadt sein.

- Die Camp-Chunks werden zur Stadt. Zusätzliche 16 Chunks bekommt die Stadt dabei nicht.
- Silber, das du für Camp-Erweiterungen bezahlt hast, wird auf den Gründungspreis angerechnet, aber höchstens so viel, wie die Erweiterungen deines jetzigen Camps wert sind. Der Preis fällt dabei nie unter 0.
- Danach ist das Camp weg. Mitbewohner und Rechte werden nicht übernommen, die Stadt startet mit Standardeinstellungen.

## Größe

Ein Chunk ist 16 × 16 Blöcke groß und reicht über die volle Höhe. Die Form eurer Stadt bestimmt ihr selbst, nur muss jeder neue Chunk mit einer Seite an einen Chunk der Stadt grenzen.

Wie viele Chunks eure Stadt haben darf, hängt von ihrer [Stufe](/smp/cities/tiers) ab: auf der Lichtung 24, als Metropole 640. Die Chunks von [Außenposten](/smp/cities/outposts) zählen mit. Mit einer Bestätigung nehmt ihr höchstens 25 Chunks dazu.

Im Stadtmenü steht die Grenze als „{belegt} / {Grenze} · Stufe {Stufe} · {Name}“.

## Abstände

Gemessen wird waagerecht von Grenze zu Grenze. Die Chunks deiner eigenen Stadt grenzen direkt aneinander.

- zum Spawn: mindestens 512 Blöcke
- zu anderen Städten: mindestens 256 Blöcke
- zu Außenposten, auch deinen eigenen: mindestens 384 Blöcke
- zu verkauften Plots anderer Städte: mindestens 256 Blöcke
- zu Camps: mindestens 64 Blöcke

Festungen gehören allen. Auf einer Festung und dem Chunk um sie herum kannst du nichts claimen, weder ein Camp noch eine Stadt oder einen Außenposten. Lag dein Land schon dort, wurde es freigegeben und der bezahlte Preis zurückerstattet. Was dort gebaut war, bleibt stehen und gehört jetzt zur Wildnis.

Städte gibt es nur in der Oberwelt.

## Beitreten und verlassen

- Eine Stadt lädt dich ein, und du nimmst die Einladung in `/city` mit **Stadt beitreten** an.
- Zum Verlassen wählst du in `/city` **Stadt verlassen**.

## Land dazunehmen

Mit **Aktuellen Chunk hinzufügen** nehmt ihr den Chunk dazu, in dem du gerade stehst. Jeder neue Chunk kostet 16.000 Silber aus der Stadtkasse, bezahlt direkt beim Claimen. Vor der Bestätigung kannst du dir die Chunks unter **Gebietsverwaltung** ansehen.

Ist die Grenze eurer Stufe erreicht, meldet das Spiel: „Die Stadt hat die Chunk-Grenze ihrer Stufe erreicht.“ Mehr Land gibt es dann erst mit der nächsten Stufe.

## Land freigeben

Unter **Gebietsverwaltung** gibst du mit **Chunk freigeben** den Chunk auf, in dem du stehst. Dafür brauchst du das Recht **Stadt erweitern**, bei Außenposten **Außenposten verwalten**.

- Du bekommst nichts zurück, und neues Land kostet wieder den vollen Preis.
- Einen Chunk mit Plot kannst du nicht freigeben.
- Die Stadt darf dadurch nicht in zwei Teile zerfallen.
- Den letzten Chunk der Stadt kannst du nicht freigeben. Dafür gibt es **Stadt auflösen**.
- Stehen Spawner im Chunk, zeigt die Bestätigung sie dir an.

## Rechte und Schutz

Wer in eurer Stadt was darf, legen die Stadt-Ränge fest, zum Beispiel bauen, Plots verwalten, Bewohner einladen oder die Kasse nutzen. Wie das im Einzelnen funktioniert, steht unter [Regierung & Ränge](/smp/cities/government) und [Rechte & Plots](/smp/cities/rights).

In der Stadt schützt der Server eure Bauten. TNT und PvP sind aus, bis die Stadt sie einschaltet. Ist das [Drachenei](/smp/dragon-egg#offenes-ei) in der Stadt offen, ist dort PvP für alle an. Blockt der Schutz etwas, nennt dir die Meldung den Grund, zum Beispiel „Fehlendes Recht: {Recht} in {Gebiet}.“

## Stadtkasse

Jede Stadt hat eine Kasse. Wer das Recht dazu hat, zahlt Silber ein oder hebt es ab. Was die Stadt kauft, bezahlt die Kasse erst, wenn ihr bestätigt habt.

### Was die Stadt bezahlt

| Kauf                                 | Preis aus der Kasse |
| :----------------------------------- | ------------------: |
| neuer Chunk der Stadt                |       16.000 Silber |
| neuer Außenposten in der Oberwelt    |       80.000 Silber |
| neuer Außenposten im Nether          |       96.000 Silber |
| weiterer Außenposten-Chunk, Oberwelt |       20.000 Silber |
| weiterer Außenposten-Chunk, Nether   |       24.000 Silber |

Bezahlt wird immer direkt beim Claimen. Was Außenposten kosten, steht unter [Außenposten](/smp/cities/outposts). Die Gründung bezahlt der Gründer selbst, siehe [Stadt gründen](/smp/cities#stadt-gründen).

Städte zahlen keinen Upkeep. Ihre Stufe steigt durch Spielzeit und [Stufenprojekte](/smp/cities/tiers), nicht durch Silber.

### Kassenverlauf

Unter **Verwaltung**, **Kasse** und **Kassenverlauf** siehst du alle Buchungen der Stadtkasse, die neuesten zuerst, 8 pro Seite.

- Jede Zeile nennt Betrag, Währung und Grund, dazu Datum und Uhrzeit.
- Ist noch jemand beteiligt, steht er auch dabei, zum Beispiel der Spieler, der eingezahlt hat.
- Dafür brauchst du das Recht **Kassenverlauf ansehen**. Das Oberhaupt hat es immer, Ratsmitglieder haben es von Anfang an.

### Gekaufte Plots

Verkaufte Plots bleiben für ihre Besitzer geschützt, auch wenn die Stadt eingefroren ist.

### Stadt auflösen

Das Oberhaupt kann die Stadt auflösen.

## Eingefrorene Städte

Ist längere Zeit kein Mitglied aktiv, friert die Stadt ein. Vorher bekommen Mitglieder mit verknüpftem Discord zwei Warnungen per Direktnachricht, in denen das Datum steht.

- Die Stadt bleibt **eingefroren und geschützt**. Land, Kasse, Stufe, Mitglieder und verkaufte Plots bleiben erhalten.
- Stadtaktionen, Mieten und das Stufenprojekt ruhen so lange.
- Sobald ein Mitglied wieder aktiv ist, taut die Stadt kostenlos auf.

::callout{type="info"}
Im Moment bleiben verlassene Städte eingefroren und geschützt. Sie werden nicht zur Ruine, verfallen nicht und lassen sich nicht übernehmen. Das kann sich noch ändern.
::

## Feststecken

Steckst du auf fremdem Land fest, hilft dir `/unstuck`:

1. Gib `/unstuck` ein.
2. Bleib fünf Sekunden still stehen. Bewegst du dich oder bekommst du Schaden, bricht es ab.
3. Dann bringt dich das Spiel zum nächsten sicheren Block außerhalb geschützter Gebiete.

- Das geht nur auf fremdem Land, also nicht auf deinem eigenen Camp, Plot oder Stadtgebiet und auch nicht in der Wildnis.
- Es klappt nur im Überlebensmodus und nicht im Kampf.
- Auf einem Reittier oder im Bett geht es nicht.
- Du kannst dich nur alle zehn Minuten befreien.
- Klappt es nicht, nennt dir die Meldung den Grund, zum Beispiel weil das Spiel gerade die Gebiete lädt oder dein Inventar kurz beschäftigt ist.

## Claims 2.0

Mit Version 0.24.0 kam **Claims 2.0**. Seitdem wachsen Städte über [Stufen](/smp/cities/tiers) statt über gekaufte Kapazität und Upkeep. Ältere Städte durften zuerst selbst entscheiden, ob sie wechseln. Das alte System gibt es inzwischen nicht mehr, und jede Stadt, die bis dahin nicht gewechselt hatte, ist von selbst ins Stufensystem gekommen.

Dieser Wechsel war kostenlos. Die Stadtkasse hat nichts bezahlt und nichts zurückbekommen, auch wenn sie für den alten Aufpreis zu wenig Silber gehabt hätte. Offene Rückstände sind weggefallen.

Eure Stadt ist auf der Stufe gelandet, die sich ihre heutigen Mitglieder mit ihrer aktiven Spielzeit im SMP verdient haben, seit sie in der Stadt sind. Für die Metropole braucht es aber auch hier 15 Mitglieder. Ab dem Wechsel sammelt ihr neue Stadtstunden.

Euer ganzes Land ist geblieben, auch das über der Grenze eurer Stufe. Liegt ihr darüber, könnt ihr erst wieder claimen, wenn ihr unter die Grenze kommt oder aufsteigt. Ebenso geblieben sind alle Plots mit ihren Kauf- und Mietverträgen und Plot-Mitbewohnern, die Stadtkasse und die Stadtform.

Neu gestartet sind dagegen die Ränge:

- Eure eigenen Ränge sind gelöscht. Legt sie unter [Regierung & Ränge](/smp/cities/government) neu an.
- Oberhaupt, Bewohner und Gast haben wieder ihre Standardrechte, im Stadtrat auch das Ratsmitglied.
- Alle Mitglieder außer dem Oberhaupt sind jetzt Bewohner.
- Laufende Stadtwahlen wurden beendet.

## Befehle

`<…>` und `[…]` sind Platzhalter; `[…]` ist optional, `a|b` heißt: eins davon.

- `/city`: Stadt öffnen
- `/city plot`: der Plot, auf dem du stehst
- `/city plots`: freie Plots
- `/city outpost`: Außenposten
- `/city view`: Grenzen zeigen
- `/city off`: Grenzen ausblenden
- `/city retry`: Änderung mit unklarem Ergebnis wiederholen
- `/unstuck`: dich von fremdem Land befreien

## Häufige Fragen

### Warum ist meine alte Stadt nach dem Wechsel eingefroren?

War sie nach den alten Regeln schon eingefroren oder eine Ruine, oder hat sie eine kommissarische Leitung geführt, ist sie eingefroren ins Stufensystem gekommen. Sie bleibt dann [eingefroren und geschützt](#eingefrorene-städte) wie jede verlassene Stadt. Sobald ein Mitglied wieder aktiv ist, taut sie kostenlos auf.

### Kann ich eine Ruine noch übernehmen?

Nein. Eine Ruine hat keine Mitglieder mehr, deshalb bleibt sie eingefroren und geschützt.

::page-cards
::

::navbox{category="SMP"}
::
