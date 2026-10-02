# 📶 ESP32-CSI-Präsenzsensor

| | |
| --- | --- |
| **Status** | 🧪 Experiment |
| **Priorität** | 🟠 Mittel |
| **Raum** | – |
| **Geeignet für** | Studienprojekt, Abschlussarbeit |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Ideen und Szenarien](#ideen-und-szenarien)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Mit **Channel State Information (CSI)** eines ESP32 Anwesenheit erkennen – als WLAN-basierter Präsenzmelder in openHAB.

---

## Ist-Stand

* Eine einfache Variante, die wie ein Präsenzmelder funktioniert, wurde getestet (Heatmap).
* Die komplexere Variante mit mehreren Antennen und 3D-Wahrnehmung ist noch nicht getestet.
* Zusätzlich liegt ein Fork eines Echtzeit-Wi-Fi-Sensing-Systems vor (`ESP32-Realtime-System`, ungetestet).
* **Gescheitert:** Das Flashen eines Asus RT-AC86U für Wi-Fi Sensing (`Flashing-Asus-RT-AC86U-for-Wi-Fi-Sensing`) gelang nicht.

---

## Offene Aufgaben

* [ ] Präsenzsensor ausbauen, sodass er zuverlässig einen Zustand liefert
* [ ] Zustand per MQTT veröffentlichen und in openHAB einbinden
* [ ] Kleine Demo aufbauen

---

## Ideen und Szenarien

* Demo: Nähert man sich dem Sensor oder hält eine Hand darüber, ändert sich der Zustand → Licht an; entfernt man sich, geht es wieder aus.
* Das Thema eignet sich als Abschlussarbeit und kann in [SmartHome-Ideen](https://github.com/Michdo93/SmartHome-Ideen) als eigene Idee ausgearbeitet werden.

---

## Repositories

* [esp32-csi-heatmap](https://github.com/Michdo93/esp32-csi-heatmap)
* [esp32-csi-presence-sensor](https://github.com/Michdo93/esp32-csi-presence-sensor)
* [ESP32-Realtime-System](https://github.com/Michdo93/ESP32-Realtime-System)
* [Flashing-Asus-RT-AC86U-for-Wi-Fi-Sensing](https://github.com/Michdo93/Flashing-Asus-RT-AC86U-for-Wi-Fi-Sensing)

---
