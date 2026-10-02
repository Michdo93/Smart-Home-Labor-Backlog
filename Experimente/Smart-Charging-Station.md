# 🔋 Smart Charging Station

| | |
| --- | --- |
| **Status** | ⚰️ Deprecated |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Alle (zum Nachlesen), Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Ideen und Szenarien](#ideen-und-szenarien)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Eine Ladestation, die USB-Ports abhängig vom Akkustand der angeschlossenen Geräte schaltet.

---

## Ist-Stand

* Eine Python-REST-API (Flask) schaltete die Ports eines **RSH-A16-USB-Hubs** mit **uhubctl**. Ein angeschlossenes Gerät meldete seinen Akkustand an die API (Stand 2023).
* Nicht mehr im Einsatz.

---

## Offene Aufgaben

* [ ] Repository kennzeichnen und archivieren

---

## Ideen und Szenarien

* Weiterhin sinnvoll: Tablets und Akkugeräte im Labor nur zwischen z. B. 20 % und 80 % laden, um die Akkus zu schonen – heute eher über openHAB und schaltbare Steckdosen oder USB-Hubs mit uhubctl.

---

## Repositories

* [Smart-Charging-Station](https://github.com/Michdo93/Smart-Charging-Station)

---
