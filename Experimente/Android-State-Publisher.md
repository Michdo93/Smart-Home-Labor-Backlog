# 📱 Android State Publisher

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Ideen und Szenarien](#ideen-und-szenarien)
<!-- /TOC -->

## Ziel

Eine Android-App veröffentlicht den Systemzustand des Smartphones oder Tablets (Akkustand, Speicher, CPU) per MQTT an openHAB – z. B. um bei niedrigem Akku der Wand-Tablets eine Warnung auszulösen.

---

## Ist-Stand

* Ursprünglich eine Projektarbeit (WiSe 22/23); bisher nur Idee und Code-Schnipsel, kein Repository.
* Besonders interessant für die [Wand-Tablets](../Infrastruktur/Tablets-und-Kiosk.md): ein fast leeres Tablet meldet sich selbst.

---

## Offene Aufgaben

* [ ] Android-App mit Paho-MQTT, die Akkustand/Ladezustand periodisch publiziert
* [ ] Thing und Items in openHAB anlegen
* [ ] Beispiel-Regel: Akku unter Schwelle → Benachrichtigung (Tablet laden)

---

## Abhängigkeiten

* [Wand-Tablets](../Infrastruktur/Tablets-und-Kiosk.md)

---

## Ideen und Szenarien

* Szenario aus der Idee: Akkustand unter 10 % → Sprachansage „Akku aufladen“.

---

