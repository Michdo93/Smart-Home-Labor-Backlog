# 🌀 3D Hologram Fan Projector

| | |
| --- | --- |
| **Status** | 🧪 Experiment |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Den LED-Ventilator-Projektor ohne die Hersteller-App steuern und mit eigenen Inhalten bespielen.

---

## Ist-Stand

* Das Protokoll wurde mit **Wireshark** mitgeschnitten (Befehle aus der Windows-App) und per Reverse Engineering in ein eigenes Python-Programm übertragen.
* Ein Konverter von **MP4 zu BIN** (Format des Geräts) wurde erstellt.
* Einordnung: Das Gerät erzeugt ein **ebenes 2D-Bild** mit LEDs auf rotierenden Armen. „3D“ ist Marketing – das Bild wirkt nur schwebend, weil man die Rotorblätter nicht sieht. Zusätzlich lässt sich eine Uhr einblenden.
* Der Pepper's-Ghost-Ansatz (umgedrehte Pyramide) am Multi Touch Table im IoT-Raum ist räumlicher, wenn auch nur aus vier Blickrichtungen.

---

## Offene Aufgaben

* [ ] Steuerung und Konverter weiter testen
* [ ] Ggf. per MQTT in openHAB einbinden

---

## Repositories

* [hologram-fan-projector](https://github.com/Michdo93/hologram-fan-projector)

---
