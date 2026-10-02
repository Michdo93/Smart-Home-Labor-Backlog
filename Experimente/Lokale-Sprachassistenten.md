# 🗣️ Lokale Sprachassistenten (LIVA, Spracherkennungs-App)

| | |
| --- | --- |
| **Status** | 🧪 Experiment |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Studienprojekt, Abschlussarbeit |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Erfahrungen mit lokalen Sprachassistenten sammeln – als Vorarbeit für die Idee eines eigenen Sprachassistenten.

---

## Ist-Stand

* Zwei Forks (`liva-jetson-ai`, `liva-raspberry-va`) für Jetson bzw. Raspberry Pi liegen vor – Inhalt und Stand sind zu sichten.
* Integriert ist eine Android-App, die erkannten Text an ein STT-Puffer-Item in openHAB sendet.
* Der Asterisk-Server des Labors nutzt bereits Piper (TTS).

---

## Offene Aufgaben

* [ ] Forks sichten: Was können sie, läuft das auf der vorhandenen Hardware?
* [ ] Mit der openHAB-eigenen Sprachinfrastruktur (Whisper, Piper, Rustpotter) vergleichen
* [ ] Ergebnisse in die Idee „Sprachassistent“ im Repo SmartHome-Ideen einfließen lassen

---

## Hinweise und Risiken

* Grundlagen: [Sprachassistenten](https://github.com/Michdo93/Informatik/blob/main/KI%20%26%20Sprachverarbeitung/Sprachassistenten.md)

---

## Repositories

* [liva-jetson-ai](https://github.com/Michdo93/liva-jetson-ai)
* [liva-raspberry-va](https://github.com/Michdo93/liva-raspberry-va)
* [openHABSpeechRecognizer](https://github.com/Michdo93/openHABSpeechRecognizer)
* [asterisk-smarthome](https://github.com/Michdo93/asterisk-smarthome)

---
