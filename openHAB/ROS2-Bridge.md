# 🔗 ROS 2 und openHAB

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
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Roboter (ROS 2) und das Smart Home (openHAB) tauschen Zustände und Befehle aus.

---

## Ist-Stand

* Ein ROS-2-Workspace für openHAB liegt vor, ist aber **ungetestet**.
* Browserbasierte Fernsteuerungs- und Diagnose-Clients für ROS 1 und ROS 2 (roslibjs, statische Seite) sind integriert.
* Die früheren ROS-1-Bridges (über HABApp) sind **deprecated** – siehe [Repository-Übersicht](../Repositories.md#deprecated-und-entfernt).

---

## Offene Aufgaben

* [ ] `ros2_openhab_ws` bauen und testen
* [ ] Erkenntnisse aus den alten ROS-1-Bridges übernehmen (Nachrichtentypen, Bildübertragung)
* [ ] Anwendungsfall definieren (z. B. Roboter meldet Position, openHAB schaltet Licht)

---

## Repositories

* [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws)
* [ros2-browser-client](https://github.com/Michdo93/ros2-browser-client)
* [ros1-browser-client](https://github.com/Michdo93/ros1-browser-client)
* [leap_control](https://github.com/Michdo93/leap_control)

---
