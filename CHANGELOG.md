# Änderungsprotokoll

## 1.7.0 – 2026-09-30

- **Trefferreaktionen:** Wer getroffen wird, zuckt sichtbar weg – je nach Richtung des Schlags:
  von vorn lehnt er sich zurück, von hinten knickt er nach vorn, von der Seite neigt und dreht er sich
  weg. Die Bewegung federt kurz nach und fügt sich über Haltung und Angriff (keine Unterbrechung).
- **Taumeln bei schweren Treffern:** Kraftschläge und wuchtige Axt-/Hammertreffer lassen den Gegner
  mit einem Schritt nach hinten taumeln.
- **Blocktreffer:** Ein geblockter Schlag drückt die Waffe sichtbar gegen den Körper, die Beine fangen ab.
- Während einer Rolle gibt es keine Reaktion (die Rolle bleibt sauber).

## 1.6.0 – 2026-09-29

- **Aufladen statt langsamer Schlag:** Die Vanilla-Angriffssperre und der zähe Schwung (bis 0,9 s)
  sind weg. Jeder Schlag ist jetzt schnell (0,3–0,5 s); schwere Waffen brauchen dafür länger zum
  Aufladen. Während die ⚔-Leiste lädt, holt der Spieler sichtbar aus (eigene Spann-Pose je Waffe) und
  geht genau dann in die Haltung zurück, wenn die Waffe wieder bereit ist. Zu früh schlagen geht weiter,
  trifft aber schwach.
- **Abklingzeit auf dem Item:** Nach einer Spezialfähigkeit läuft auf der Waffe im Inventar und in der
  Schnellleiste der graue Abklingzeit-Balken ab (wie bei Enderperlen). Solange er läuft, reagiert der
  Benutzen-Knopf der Waffe nicht (auch kein Haltungswechsel).
- Kraftschlag und Sturmangriff sind ebenfalls schneller.

## 1.5.1 – 2026-09-29

- **Normale Kombo-Angriffe korrigiert:** Seit der Umstellung auf die Dreizack-Haltung (1.3.0) zeigten
  viele Klingen im Treffermoment in falsche Richtungen (z. B. Rapier-Stoß steil nach oben). Alle
  Techniken haben jetzt Spitzenziele für Ausholen und Treffer: Stiche (Dolche, Rapier) gehen gerade
  zum Gegner, Hiebe (Säbel, Streitkolben, Morgenstern, Langschwert, Axt) holen sichtbar aus und
  ziehen durch. Zwischenbilder geprüft – keine Sprünge oder Umklappen.
- Generator meldet, wie viele Spitzenziele erreicht bzw. (bei Zweihand-/Stangenwaffen) unerreichbar sind.

## 1.5.0 – 2026-09-29

- **Eigener Kampfstil je Waffe:** Block, Aufladen, Kraftschlag und Sturmangriff gibt es jetzt für
  jede der 12 Waffen einzeln (vorher nur je Griffart) – nach historischen Vorbildern, z. B.
  Langschwert: Deckung in der *Krone*, Aufladen im *Zornhut*, Kraftschlag *Zornhau*;
  Rapier: *Quart-Parade* und tiefer Ausfall (*Passata*), Sturm als *Flèche*;
  Säbel: *Hängeparade*, *Moulinet-Hieb*, *Reiterhieb*; Kriegssense: *Großer Mähschnitt* aus der Hüfte;
  Doppeldolche: *Kreuzblock* und *Doppelstich*; Speer: *Langer Stoß* und *Lanzenangriff*.
- **Klingenrichtung exakt gesteuert:** An den Schlüsselmomenten (Ausholen, Treffer, Nachschwung)
  wird der Arm so berechnet, dass die Klinge wirklich dorthin zeigt (z. B. beim Zornhut nach hinten
  über die Schulter, beim Treffer nach vorn). Dazwischen wird gleichmäßig überblendet – keine
  Sprünge mehr. Zweihandwaffen behalten dabei beide Hände am Griff.
- **Ausfallschritt je Waffe:** Rapier und Speer fallen beim Kraftschlag weit aus, der Hammer kaum;
  Sturmangriffe schieben je nach Waffe unterschiedlich stark.
- Anzeige nennt die Technik (z. B. „🛡 Krone“, „⚡ … Zornhau“), Treffer melden ihren Namen.
- Kampfbuch: Waffenseiten zeigen Block, Kraftschlag und Sturmangriff der Waffe.

## 1.4.0 – 2026-09-28

- **Neues Kampfbuch:** Beim Benutzen erscheint ein großes 3D-Buch vor dem Spieler und klappt
  animiert auf. Schlagen blättert weiter, „Zurückblättern“ (Touch-Knopf) blättert zurück – jeweils
  mit einer umschwingenden Seite. 22 Pergamentseiten mit eigener Pixelschrift: Angriff, Ausdauer,
  Haltungen, Verteidigung, besondere Angriffe, Bewegung, Steuerung, je eine Seite pro Waffe
  (Bild, Werte, Fähigkeit, Kombo, Schaden je Stufe, Kampfstil), Duelle und Schmiede.
- **Touch-Steuerung repariert:** Kampfbuch und alle Waffen haben jetzt einen Benutzen-Knopf
  („Kampfbuch öffnen“ bzw. „Fähigkeit“) – auf iPad/Handy ließen sich Buch und Fähigkeiten vorher nicht auslösen.
- Schleichen + Kampfbuch öffnet das Duell-Menü.

## 1.3.0 – 2026-09-28

- **Waffen richtig herum in der Hand:** Alle Waffen nutzen die im Spiel erprobte Ausrichtung des
  Vanilla-Dreizacks, der Griff sitzt in der Hand. Wohin die Klinge zeigt, wird über den Arm eingestellt.
  Die Arm-Kinematik ist an Mojangs Armbrust-Pose überprüft (beide Hände treffen sich vorn).
- **Waffe bleibt beim Schlagen in der Hand:** Der Waffenschwung verschiebt die Waffe nicht mehr.
- **Block** (Schleichen halten): Waffe quer vor dem Körper, Frontaltreffer werden zu 50–60 % abgewehrt
  (Ausdauerkosten, Äxte/Hämmer zehren doppelt, Deckungsbruch bei leerer Ausdauer).
- **Kraftschlag:** Im Block lädt sich ein Kraftschlag auf (⚡-Leiste, eigene Lade-Pose); Zuschlagen gibt bis
  zu +90 % Schaden, Ausfallschritt, starken Rückstoß und durchbricht gegnerische Blöcke.
- **Sturmangriff** aus dem Sprint: Vorwärtsschub, eigene Animation, +25 % Schaden.
- **Rollen** statt Seitschritt: Vorwärts-, Rückwärts- und Seitrolle in Laufrichtung.
- **Körperbewegung je Technik:** Ausfallschritte (Rapier, Speer), Nachsetzen (Schwerter), Zurückziehen
  (Hakenzug der Hellebarde); schwere Schläge bremsen kurz ab.
- **Waffengewicht:** Dolche und Rapier machen schneller, Zweihänder und Hammer langsamer.

## 1.2.1 – 2026-09-28

- Kalibrierstäbe A/B/C (Kreativ-Inventar → Ausrüstung): zeigen im Spiel die Achsen des
  Waffenknochens (Rot = x, Grün = y, Blau = z), der Spieler hält dabei den Arm gerade nach vorn.
  Damit wird die in 1.2.0 falsch herum sitzende Waffenhaltung exakt vermessen.

## 1.2.0 – 2026-09-27

- **Waffenhaltung komplett neu berechnet:** Ein Kinematik-Modell des Spielerskeletts (kalibriert an
  Screenshots aus dem Spiel) setzt den Griff jeder Waffe exakt in die Hand – vorher hielt die Hand
  die Klinge etwa 10 Pixel über dem Griff.
- **Zweihandwaffen werden mit beiden Händen gehalten:** Die linke Hand liegt per inverser Kinematik
  am Griff – in jeder Haltung und in jedem Bild jeder Angriffs- und Fähigkeitsanimation.
- **Eigene Grundstellung je Waffe** nach historischen Vorbildern (Pflug, Vom Tag, Terz,
  Lanzenwacht …), jeweils in drei Varianten (Mitte/Hoch/Tief), mit passender Körperdrehung und
  Beinstellung.
- **Vanilla-Bewegungen neutralisiert:** Minecrafts eigener Schlag, das Armpendeln beim Laufen und das
  Atmen überlagern die Waffenposen nicht mehr.
- **Angriffe und Fähigkeiten als Ganzkörper-Animationen** (Arme, Körper, Kopf, Beine) anstelle der
  Haltung; danach kehrt der Spieler nahtlos in seine Stellung zurück. 11 eigene Fähigkeitsanimationen.
- Kriegssense mit langer, geschwungener Klinge; Icons skalieren nach Waffengröße.

## 1.1.0 – 2026-09-27

- Jede der 12 Waffen hat jetzt eine eigene Kombo-Folge an Angriffsanimationen (38 Techniken,
  z. B. Oberhau/Unterhau/Zornhau beim Langschwert, Ausfall beim Rapier, Hammerfall beim Kriegshammer),
  mit weicher Interpolation und Einsatz von Körper, Kopf und Beinen (Ausfallschritte).
- Eigener Waffenschwung im Attachable je Waffe (z. B. kreisender Morgenstern, mähende Sense).
- Zweihandwaffen sperren die Nebenhand sichtbar mit einem roten ✖; der Gegenstand wird ausgelagert
  und automatisch zurückgelegt.
- Angriffstempo nach Java-Vorbild: Aufladeleiste, schwache Treffer bei zu frühem Zuschlagen,
  Kombo nur mit voll geladenen Schlägen, Reset beim Waffenwechsel.
- Technik-Name wird beim Treffer angezeigt; Kampfbuch zeigt Techniken und Zweihand-Hinweis.

## 1.0.0 – 2026-09-27

- 12 mittelalterliche Waffen in Eisen, Gold, Diamant und Netherit (48 Items) mit 3D-Modellen.
- Neues Kampfsystem: Ausdauer, Angriffstempo je Waffe, Kombos mit Finisher, Rückenstich,
  Parade, Ausweichen, drei Haltungen, Spezialfähigkeiten, Blutung, Schildbrechen, Betäubung.
- Sichtbare Körperanimationen: Haltungsposen und Kombo-Angriffe je Waffe.
- Kampfbuch mit Anleitung, Waffenkunde und 1v1-Duellen inklusive Statistik.
