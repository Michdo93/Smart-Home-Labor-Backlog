# ☎️ Intercom (Asterisk)

| | |
| --- | --- |
| **Status** | ⛔ Blockiert |
| **Priorität** | 🟠 Mittel |
| **Raum** | Alle Räume |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Eine Gegensprechanlage zwischen den Räumen auf Basis von **Asterisk**, mit alten Raspberry Pis und Touch-Displays.

---

## Ist-Stand

* Der Code ist fertig, aber bisher nur mit **zwei VMs** getestet.
* Nicht mehr benötigte Raspberry Pis bekommen ein Touch-Display.
* **Blockiert:** Die bestellten Konferenzlautsprecher waren die falschen; die Lieferung wurde reklamiert.
* Der **Asterisk-Server** (Ubuntu Server auf Proxmox, mit Piper TTS und einem Python-Smart-Home-Dienst) ist eingerichtet und dokumentiert (`asterisk-smarthome`).

---

## Offene Aufgaben

* [ ] Passende Lautsprecher/Mikrofone beschaffen
* [ ] Auf echter Hardware testen
* [ ] Strom verlegen (neben den Tablets)
* [ ] Geräte montieren

---

## Repositories

* [rpi-intercom](https://github.com/Michdo93/rpi-intercom)
* [asterisk-smarthome](https://github.com/Michdo93/asterisk-smarthome)

---
