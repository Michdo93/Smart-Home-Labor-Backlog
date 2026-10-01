# 📺 Samsung SmartTV

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

Den Fernseher vollständig steuern – auch nach längerem Standby.

---

## Ist-Stand

* Modell: **UE55KU6079U** (in einer früheren Notiz als UE55MU6179U bezeichnet).
* Teilweise über das **Samsung TV Binding** eingebunden: Ein/Aus und Quelle funktionieren.
* Offiziell getestet sind nur zwei Schwestermodelle.
* Nach **längerem Standby** muss der Fernseher von Hand eingeschaltet und der Zugriff für openHAB erneut zugelassen werden.
* Ein eigenes, KI-generiertes und noch ungetestetes Python-Programm in Anlehnung an bestehende Python-Lösungen liegt vor.

---

## Offene Aufgaben

* [ ] Python-Steuerung testen
* [ ] Bei Erfolg per MQTT an openHAB anbinden

---

## Repositories

* [samsungtv](https://github.com/Michdo93/samsungtv)

---
