# 🚪 Türdurchgangszähler (TF-Luna)

| | |
| --- | --- |
| **Status** | 🧪 Experiment |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
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

Ein Richtungs-Durchgangszähler an der Tür zählt, wer einen Raum betritt oder verlässt – als Ergänzung oder Alternative zum People Counter.

---

## Ist-Stand

* Ein ESP32 mit zwei **TF-Luna-LiDAR-Sensoren** erkennt die Durchgangsrichtung und ist per MQTT an openHAB angebunden – ungetestet.

---

## Offene Aufgaben

* [ ] Hardware aufbauen und flashen
* [ ] An einer Labortür testen und Zählgenauigkeit messen
* [ ] Mit dem People Counter vergleichen

---

## Abhängigkeiten

* [People Counter](../Geräteintegration/People-Counter.md)

---

## Repositories

* [door-traffic-counter](https://github.com/Michdo93/door-traffic-counter)

---
