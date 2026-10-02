# 🪴 Pflanzenüberwachung

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Hiwi, Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Bodenfeuchte, Temperatur und Licht einer Zimmerpflanze werden gemessen und in openHAB angezeigt; bei zu trockener Erde gibt es eine Erinnerung zum Gießen.

---

## Ist-Stand

* Projektidee (WiSe 22/23) mit einem Pflanzensensor und openHAB; bisher kein Repository.
* Lässt sich gut über das MySensors-/ESP-Thema umsetzen (günstiger Sensor, MQTT).

---

## Offene Aufgaben

* [ ] Sensor wählen (z. B. kapazitiver Bodenfeuchtesensor an ESP32) und aufbauen
* [ ] Werte per MQTT an openHAB senden
* [ ] Regel: zu trocken → Erinnerung; Verlauf per Persistence aufzeichnen

---

## Abhängigkeiten

* [MySensors / DIY-Funksensoren](MySensors-DIY-Sensoren.md)

---

## Hinweise und Risiken

* Grundlagen: [Zeitreihen & openHAB Persistence](https://github.com/Michdo93/Informatik/blob/main/Datenbanken/Zeitreihen%20%26%20openHAB%20Persistence.md)

---

