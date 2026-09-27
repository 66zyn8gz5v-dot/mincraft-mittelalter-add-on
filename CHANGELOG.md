# Änderungsprotokoll

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
