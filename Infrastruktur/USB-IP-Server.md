# 🔌 Raspberry Pis als USB/IP-Server

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟠 Mittel |
| **Raum** | Alle Räume (Konferenz: 2) |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
<!-- /TOC -->

## Ziel

In jedem Raum stellt ein Raspberry Pi per **USB/IP** USB-Geräte (Leap Motion, NFC-Leser, Kameras …) im Netzwerk bereit, sodass sie von Servern oder VMs genutzt werden können.

---

## Ist-Stand

* Die Images sind geflasht.
* Geplant: ein Pi pro Raum, im Konferenzraum zwei.

---

## Offene Aufgaben

* [ ] Pis installieren, feste IPs vergeben, ins Ansible-Inventar aufnehmen
* [ ] USB/IP als systemd-Service einrichten
* [ ] Geräte zuordnen und dokumentieren

---

## Abhängigkeiten

* Wird genutzt von: [People Counter](../Geräteintegration/People-Counter.md), [Leap Motion](../Experimente/Leap-Motion.md), [NFC/RFID](../Experimente/NFC-RFID.md)

---

