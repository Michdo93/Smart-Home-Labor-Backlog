# 🗑️ Abfallkalender

| | |
| --- | --- |
| **Status** | ⛔ Blockiert |
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

Der Abfallkalender wird automatisch heruntergeladen und steht in openHAB zur Verfügung (z. B. Erinnerung am Vorabend).

---

## Ist-Stand

* Ein Python-Programm mit Selenium lud den Abfallkalender für die Hochschule Furtwangen herunter.
* Es **lief zuletzt gar nicht mehr** und muss grundlegend überarbeitet werden.

---

## Offene Aufgaben

* [ ] Ursache finden (geänderte Webseite, Selenium-/Browser-Version)
* [ ] Prüfen, ob es eine stabilere Quelle gibt (iCal-Export, Schnittstelle) statt Web-Scraping
* [ ] Refactoring, Betrieb als Timer-Dienst
* [ ] Anbindung an openHAB (z. B. über ein iCal-Binding oder MQTT)

---

## Repositories

* [waste-calendar-downloader](https://github.com/Michdo93/waste-calendar-downloader)

---
