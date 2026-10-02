# ✋ Leap Motion

| | |
| --- | --- |
| **Status** | 🔍 Test ausstehend |
| **Priorität** | 🟢 Niedrig |
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

Smart-Home-Geräte per Handgesten steuern.

---

## Ist-Stand

* Anschluss über die [USB/IP-Server](../Infrastruktur/USB-IP-Server.md).
* Fertige Beispiele: Musik lauter/leiser, Sender vor/zurück, Jalousien und Rollladen hoch/runter.
* Die Beispiele liegen im Repository `Leap-Motion-Examples` – **unklar ist, welche Codes am Ende korrekt waren**.
* Integriert ist außerdem ein ROS-2-Node, der Roboter über den Ultraleap-Controller per `cmd_vel` steuert (`leap_control`).

---

## Offene Aufgaben

* [ ] Jalousien/Rollladen-Beispiel erneut testen
* [ ] Lichtsteuerung umsetzen
* [ ] Codes in `Leap-Motion-Examples` sichten, die funktionierenden kennzeichnen, veraltete in `archive/` verschieben

---

## Repositories

* [Leap-Motion-Examples](https://github.com/Michdo93/Leap-Motion-Examples)
* [leap_control](https://github.com/Michdo93/leap_control)

---
