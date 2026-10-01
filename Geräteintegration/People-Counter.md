# 👥 People Counter

| | |
| --- | --- |
| **Status** | 🔍 Test ausstehend |
| **Priorität** | 🟠 Mittel |
| **Raum** | Zwischen IoT und Multimedia |
| **Geeignet für** | Hiwi, Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Eine Tiefenkamera zählt Personen, z. B. um grob zu erkennen, wie viele am Konferenztisch sitzen. Die Zahl steht in openHAB zur Verfügung.

---

## Ist-Stand

* Kamera: **Asus Xtion Pro** (Stereo-/Tiefenkamera), bereits montiert.
* Treiber ließen sich nur unter **Windows** installieren, nicht unter Linux.
* Lösung: Die Kamera hängt am Raspberry Pi (derselbe wie für die Gestensteuerung des Newspaper Projectors) und wird per **USB/IP** an eine **Windows-VM** durchgereicht.
* Code unter Windows am Laptop getestet – funktioniert einigermaßen.
* Ergebnis per Webseite abrufbar, openHAB-Integration über das **MQTT-Binding**.
* Auf dem Pi eingerichtet und getestet.

---

## Offene Aufgaben

* [ ] Zählgenauigkeit verbessern: Personen werden über mehrere Frames teilweise **doppelt gezählt**
* [ ] Reichweite prüfen: Ab einer gewissen Distanz wird nicht mehr gemessen
* [ ] Langzeittest im Laborbetrieb

---

## Abhängigkeiten

* [USB/IP-Server](../Infrastruktur/USB-IP-Server.md)

---

## Repositories

* [people-counter](https://github.com/Michdo93/people-counter)

---
