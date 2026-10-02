# 🐍 Python-3-Migration älterer openHAB-Projekte

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟠 Mittel |
| **Raum** | – |
| **Geeignet für** | Hiwi, Praxissemester |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Ältere openHAB-Erweiterungen, die noch auf Python 2, Jython oder älteren Bibliotheken basieren, laufen wieder – auf Python 3 bzw. den aktuellen openHAB-Rule-Engines.

---

## Ist-Stand

* **openHAB-Application-Checker:** prüft per Exec Action, ob eine Anwendung läuft, und setzt ein Switch-Item – muss nach Python 3 migriert werden.
* **openHAB-RuleManager:** Verwaltung von Rules – muss nach Python 3 migriert werden.
* **status-openhab-org:** Live-Status von status.openhab.org als Items – muss nach Python 3 migriert werden.
* **openHAB-VoiceRSS-Sonos:** Rule für Sprachausgabe über VoiceRSS auf Sonos – muss nach Python 3 migriert werden.
* **HABApp-MQTT-Event-Bus:** MQTT-Event-Bus für openHAB 2.x/3.x mit HABApp – muss vermutlich auf aktuelle Versionen gebracht werden.

---

## Offene Aufgaben

* [ ] Pro Projekt prüfen, ob es noch gebraucht wird oder durch openHAB-eigene Funktionen ersetzt werden kann
* [ ] Migration auf Python 3 bzw. Python 3 Scripting in openHAB
* [ ] Exec-Aufrufe auf die Whitelist prüfen (`misc/exec.whitelist`)
* [ ] Testen und README aktualisieren (unterstützte openHAB-Version angeben)
* [ ] Nicht mehr benötigte Projekte als **deprecated** kennzeichnen und archivieren

---

## Abhängigkeiten

* [Migration der Rules](Rules-Migration.md)

---

## Hinweise und Risiken

* Leitfaden: [Refactoring & Migration](https://github.com/Michdo93/Informatik/blob/main/Software-Konzepte/Refactoring%20%26%20Migration.md)
* Für VoiceRSS (Cloud-TTS) prüfen, ob lokales TTS (z. B. Piper) eine Alternative ist.

---

## Repositories

* [openHAB-Application-Checker](https://github.com/Michdo93/openHAB-Application-Checker)
* [openHAB-RuleManager](https://github.com/Michdo93/openHAB-RuleManager)
* [status-openhab-org](https://github.com/Michdo93/status-openhab-org)
* [openHAB-VoiceRSS-Sonos](https://github.com/Michdo93/openHAB-VoiceRSS-Sonos)
* [HABApp-MQTT-Event-Bus](https://github.com/Michdo93/HABApp-MQTT-Event-Bus)

---
