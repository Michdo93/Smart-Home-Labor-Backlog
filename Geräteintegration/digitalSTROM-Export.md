# ⚡ digitalSTROM-Messdaten exportieren

| | |
| --- | --- |
| **Status** | ⚰️ Deprecated |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Alle (zum Nachlesen) |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Ideen und Szenarien](#ideen-und-szenarien)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Messdaten des digitalSTROM-Servers automatisch als CSV herunterladen.

---

## Ist-Stand

* Ein Python-Skript öffnete den digitalSTROM-Server mit **Selenium** und lud die CSV-Datei per **PyAutoGUI** herunter (Stand 2023).
* Nicht mehr im Einsatz.

---

## Offene Aufgaben

* [ ] Repository kennzeichnen und archivieren

---

## Ideen und Szenarien

* Browser-Automatisierung mit Selenium/PyAutoGUI ist ein typischer [Workaround](https://github.com/Michdo93/Informatik/blob/main/Workarounds%20%26%20Hacks/Begriffe.md), wenn ein Gerät keine API hat – fragil bei jeder Änderung der Weboberfläche.

---

## Repositories

* [digitalstrom-export-csv](https://github.com/Michdo93/digitalstrom-export-csv)

---
