# Änderungsprotokoll

## 1.20.0 – 2026-10-04

- **Übungspuppe** zum Trainieren ohne zweiten Spieler: Strohpuppe auf einem Pfahl mit Zielscheibe,
  Querbalken und Sackkopf. Item auf einen Block benutzen → die Puppe steht dir zugewandt.
  Jeder Treffer lässt sie gedämpft nachwackeln; über dem Kopf stehen Schaden des letzten Treffers,
  Gesamtschaden der Serie, Trefferzahl sowie Kombo, Technik bzw. „Kraftschlag“. Nach 3 Sekunden ohne
  Treffer heilt sie sich und setzt die Anzeige zurück. Schleichen + Schlagen baut sie ab (Item zurück).
  Rezept: Wolle oben, Heuballen in der Mitte zwischen zwei Stöcken, Stock unten.
- Kampfbuch: Übungspuppe auf „Neu im Add-on“ und „Die Schmiede“.

## 1.19.1 – 2026-10-04

- Korrektur: Buchseite „Neu im Add-on“ war zu lang, der Neubau von 1.19.0 brach ab; Repo-Dateien
  waren unvollständig (die veröffentlichten Pakete waren vollständig). Neues Veröffentlichungsskript
  `tools/veroeffentlichen.sh` bricht bei jedem Fehler ab.

## 1.19.0 – 2026-10-04

- **Zwei mittelalterliche Rüstungssets** (je Helm/Haube, Brust, Beine, Stiefel), am Körper mit
  Mojangs Rüstungsmodell dargestellt:
  - **Gambeson** (aus Wolle): gesteppter Stoff, wenig Schutz, aber Ausdauer kehrt bis zu 30 % schneller
    zurück – ideal für flinke Kämpfer.
  - **Plattenrüstung** (aus Eisenblöcken): polierter Stahl mit Goldnieten und Sehschlitz im Ritterhelm,
    hoher Schutz, aber bis zu 8 % langsamer und 25 % langsamere Ausdauererholung.
  - Die Wirkung gilt anteilig je getragenem Teil; Rüstungen sind verzauberbar und reparierbar.
- Kampfbuch: Rüstungen auf „Die Schmiede“ und „Neu im Add-on“.

## 1.18.0 – 2026-10-04

- **Rundschild (Buckler)** aus Holz oder Eisen für die Nebenhand (Vorbild: Fechtbuch I.33). Zusammen mit
  einer Einhandwaffe: Paradefenster 60 % länger, Block wehrt 15 % mehr ab, parierte Gegner taumeln
  länger. Gewölbte Scheibe mit Schildbuckel, haltbar und reparierbar; die Kampfanzeige zeigt ein
  Schild-Symbol. Rezept: 4 Bretter (bzw. Eisenbarren) im Kreuz um einen Eisen- (bzw. Gold-)Barren.
- **Hiebspur:** Finisher und Kraftschläge erzeugen einen hellen Strichring um das Ziel.
- **Rangliste:** Duell-Menü → „Rangliste“ zeigt die zehn besten Duellanten der Welt (Siege/Niederlagen).
- Kampfbuch: Rundschild auf den Seiten „Verteidigung“ und „Neu im Add-on“.

## 1.17.1 – 2026-10-04

- Korrektur: 1.17.0 wurde nach einem fehlgeschlagenen Neubau (zu lange Duell-Seite im Kampfbuch)
  unvollständig veröffentlicht. Seite gekürzt, Paket vollständig neu gebaut.

## 1.17.0 – 2026-10-04

- **Duell mit gleichen Waffen:** Nach der Gegnerwahl lässt sich festlegen, ob mit eigener Ausrüstung
  oder mit derselben Waffe gekämpft wird (alle 12 Waffen wählbar, Eisen-Stufe). Beide bekommen die
  Leihwaffe in die Schnellleiste (direkt ausgewählt); sie lässt sich nicht fallen lassen, bleibt beim
  Rundenverlust erhalten und wird nach dem Duell wieder eingesammelt.

## 1.16.0 – 2026-10-03

- **Duelle im Best-of-3-Modus:** Wer zuerst zwei Runden gewinnt, siegt. Eine Runde ist verloren, sobald
  ein Kämpfer unter 5 Lebenspunkte fällt – kein Tod, keine verlorenen Gegenstände. Zwischen den Runden
  werden beide geheilt, an ihre Startpunkte gegenüber gesetzt (Blick zueinander) und es gibt einen neuen
  Countdown mit Rundenanzeige und Spielstand.
- **Kampfring:** Ein Kreis aus Flammen (Radius 7) markiert die Arena. Wer ihn verlässt, wird
  zurückgestoßen und gewarnt.
- Kampfbuch: Duell-Seite aktualisiert.

## 1.15.0 – 2026-10-02

- **Kampfstand überarbeitet:** In allen Haltungen stehen die Füße jetzt schulterbreit auseinander,
  der Oberkörper lehnt leicht vor und der Kopf bleibt auf den Gegner gerichtet – in der tiefen Haltung
  breiter und tiefer, in der hohen aufrechter.
- **Kampfbereitschaft im Stand:** Wer mit Waffe stillsteht, atmet sichtbar und verlagert ruhig das
  Gewicht, die Waffe wiegt leicht mit. Sobald gelaufen wird, übernimmt die Laufbewegung.
- Die Waffenausrichtung aus 1.14.0 bleibt unverändert, bis Rückmeldung aus dem Spiel vorliegt.

## 1.14.0 – 2026-10-01

- **Waffenhaltung fest im Modell:** Die Haltedrehung wird nicht mehr per Animation gesetzt, sondern
  steckt fest in der 3D-Geometrie jeder Waffe – so macht es auch Mojang beim Bogen. Damit wirkt sie
  im Spiel garantiert (Animationen am Haltepunkt der Hand wurden offenbar ignoriert).

## 1.13.0 – 2026-10-01

- **Ursache der falsch sitzenden Waffen gefunden:** Die Haltedrehung lag auf dem Modellknochen, der an
  die Hand gebunden ist – diese Drehung überschreibt Minecraft. Alle Screenshots passten genau zu
  „Waffe ungedreht längs des Arms“ (Rapier nach oben, Axt/Zweihänder nach hinten an der Hüfte).
  Die Drehung sitzt jetzt auf einem eigenen Unterknochen („halt“) und wirkt damit erstmals im Spiel.
- Kalibrierstäbe ebenso umgestellt. Ego-Perspektive bleibt unverändert.

## 1.12.0 – 2026-10-01

- **Waffenhaltung neu aufgebaut (Nutzer-Screenshots 01.10.):** Die Waffen saßen weiterhin falsch
  (Rapier nach oben, Zweihänder und Axt nach unten, Hellebarde quer). Die Auswertung der Bilder hat
  gezeigt, dass sich die übernommene Dreizack-Ausrichtung nicht zuverlässig vorhersagen lässt.
  Neu: **natürlicher Faustgriff** – die Klinge kommt vorn aus der Faust (nur eine Drehachse), der Arm
  bestimmt die Richtung (Arm hängt → Klinge waagerecht nach vorn, Arm vorgestreckt → Klinge oben).
  Zweihand- und Stangenwaffen: rechte Hand am Griff, linke Hand per Kinematik am Griff bzw. Schaft,
  Arme möglichst ohne verdrehte Kombinationen.
- Sollte die Klinge jetzt genau nach hinten zeigen: Duell-Menü → „Waffenhaltung testen“ →
  Variante 1 dreht alle Waffen auf einmal richtig herum (dann bitte die Nummer melden).

## 1.11.0 – 2026-10-01

- **Der Körper läuft mit:** Neue Lauf-Ebene für alle Waffen. Beim Gehen drehen die Schultern gegen
  die Schritte, die Hüfte wiegt leicht, der Körper federt im Schritt und die Waffe wippt mit (bei
  Zweihandwaffen bleiben beide Hände am Griff). Im Sprint lehnt sich der Kämpfer nach vorn. Der Kopf
  gleicht die Bewegung aus, der Blick bleibt ruhig. Leichte Waffen schwingen freier, schwere Waffen
  federn mehr und drehen weniger. Vorher wirkte der Oberkörper mit Waffe beim Laufen starr.
- Nach Tod oder Wiedereintritt starten Haltung und Lauf-Ebene sofort neu.

## 1.10.0 – 2026-09-30

- **Eigene Kampfklänge** (selbst synthetisiert, 13 Varianten): Klingenklirren beim Block, helles
  Singen der Klinge bei Parade und Riposte, Luftrauschen bei jedem Schlag (leichte Waffen zischen
  hell, schwere brummen tief), satter Trefferklang (stumpfe Waffen dumpfer), tiefer Wucht-Schlag bei
  Kraftschlag und Erdbeben.
- **Eigene Partikel:** glühende Funken genau zwischen den Kämpfern bei Block und Parade,
  Blutspritzer bei vollen Klingentreffern und bei Blutung (Tropfen fallen zu Boden), Staubring am
  Boden bei Kraftschlag und Erdbeben.
- Kampfbuch: „Neu im Add-on“ um Klänge und Funken ergänzt.

## 1.9.0 – 2026-09-30

- **Kampfbuch als 3D-Buch zum Aufstellen:** Im Inventar ein flaches Buch – auf einen Block benutzt,
  steht es als großes aufgeschlagenes Buch auf einem hölzernen Lesepult (bleibt stehen, jeder kann
  darin lesen). In die Luft benutzt schwebt es wie bisher vor dir.
  Neue Steuerung: **Benutzen = weiterblättern** (Touch-Knopf „Weiterblättern“), **Schlagen = zurück**,
  **Schleichen + Schlagen = zuklappen/aufheben**. Jedes Umblättern ist animiert.
- Neue Buchseite **„Neu im Add-on“**, Inhaltsverzeichnis und Steuerung aktualisiert.
- **Neue Kampfleisten:** eigene Pixel-Symbole (Schwert, Ausdauer, Blitz, Schild, Stern) und farbige
  Leistenstücke statt Textstrichen – Tempo, Ausdauer, Kraftschlag und Fähigkeit auf einen Blick.
- **Abklingzeit direkt auf dem Item:** Die Waffe trägt die Abklingzeit ihrer Fähigkeit jetzt selbst
  (`minecraft:cooldown`) – nach dem Benutzen läuft auf dem Item in Schnellleiste und Inventar die
  weiße Anzeige herunter, wie bei Enderperlen.
- **Haltung wechseln jetzt mit Schleichen + Springen** (der Benutzen-Knopf gehört ganz der Fähigkeit).

## 1.8.0 – 2026-09-30

- **Versionsanzeige:** Beim Betreten der Welt meldet der Chat „Verhalten v…“; der Name des Kampfbuchs
  zeigt „(Bilder v…)“, dazu Paketnamen in den Welteinstellungen, Duell-Menü und Titelseite des Buchs.
  Stimmen beide Nummern nicht überein oder fehlt die Meldung, ist eine alte Version geladen.
- **Drehtest für die Waffenhaltung:** Schleichen + Kampfbuch → „Waffenhaltung testen“ schaltet acht
  Varianten durch (Waffe um den Griff gekippt/gedreht). Die gewählte Variante bleibt gespeichert und gilt
  sofort für alle Waffen; die passende Nummer wird danach fest eingebaut.

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
