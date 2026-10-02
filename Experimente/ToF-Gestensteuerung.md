# 👋 Gestensteuerung mit ToF-Sensoren

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
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Mit kleinen **Time-of-Flight-Sensoren** (VL53L1X, VL53L5CX) und Mikrocontrollern einfache Gesten (wischen, nähern) erkennen und an openHAB senden.

---

## Ist-Stand

* **vl53l1x-gesture-toolkit:** Gestensteuerung mit einem einzelnen VL53L1X an ESP32, ESP32-C3, Arduino oder RP2040 – ungetestet.
* **vl53l5cx_gesture_experiments:** Python-Skript zur Gestenerkennung mit dem VL53L5CX (Mehrzonen-Sensor) – ungetestet.
* Ein weiteres Repository `GestureControl` ist öffentlich nicht auffindbar.

---

## Offene Aufgaben

* [ ] Sensoren beschaffen bzw. vorhandene prüfen, ggf. löten
* [ ] Firmware flashen und testen
* [ ] Gesten per MQTT an openHAB senden und eine Demo-Regel erstellen
* [ ] Repository `GestureControl` klären

---

## Repositories

* [vl53l1x-gesture-toolkit](https://github.com/Michdo93/vl53l1x-gesture-toolkit)
* [vl53l5cx_gesture_experiments](https://github.com/Michdo93/vl53l5cx_gesture_experiments)

---
