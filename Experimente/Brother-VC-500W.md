# 🖨️ Brother VC-500W (Etikettendrucker)

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

Druckerstatus (z. B. Rolle leer, druckbereit) abfragen und für die Selfie-Anwendung nutzen.

---

## Ist-Stand

* Die klassischen Drucker-Bindings in openHAB funktionieren nicht.
* Über eine Schwachstelle lassen sich offenbar Informationen vom Drucker abfragen; zwei Testskripte liegen vor.
* Der Drucker lässt sich nicht per WoL/WoWLAN einschalten, kann aber über die **Smartphone-App** (nicht die Windows-App) so konfiguriert werden, dass er dauerhaft an bleibt.

---

## Offene Aufgaben

* [ ] Testskripte prüfen
* [ ] Statusabfrage in die Selfie-Anwendung integrieren
* [ ] Papierverbrauch optimieren: prüfen, ob das gesendete Bildformat unnötig viel Weißraum erzeugt

---

## Repositories

* [Brother-VC-500W](https://github.com/Michdo93/Brother-VC-500W)

---
