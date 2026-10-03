# 💿 Vorinstallierte VM-Vorlagen

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Server |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Fertige, vorinstallierte VM-Vorlagen (Templates) bereitstellen, mit denen Studierende und Hiwis sofort loslegen können – ohne stundenlange Einrichtung von openHAB, ROS, NAOqi oder Android Studio.

---

## Ist-Stand

* Aus einer früheren Hiwi-Aufgabe existiert eine Wunschliste an vorinstallierten VMs, u. a.:
  * openHAB-Entwicklung: Ubuntu + Java + openHAB + Mosquitto, Varianten mit HABApp, Jython, Binding-Skeleton
  * Robotik: Ubuntu 16.04 + ROS Kinetic + Python 2.7 + NAOqi (Python/Java/C++) + Pepper-/Nao-/Turtlebot-Pakete
  * App-/VR-Entwicklung: Windows/Ubuntu + Android Studio, Unity, Steam/SteamVR
* Diese Kombinationen sind teils veraltet (ROS Kinetic, Ubuntu 16.04, Python 2.7) und nur für Altgeräte (NAO/Pepper) nötig.

---

## Offene Aufgaben

* [ ] Festlegen, welche Vorlagen heute noch sinnvoll sind (aktuelle openHAB-/Java-Version; Robotik nur für NAO/Pepper als Altumgebung)
* [ ] Vorlagen als **Proxmox-Templates** anlegen und dokumentieren (was ist installiert, Zugangsdaten-Konzept)
* [ ] Wo möglich durch **Container** oder ein Bootstrap-Skript ersetzen statt schwergewichtiger VMs
* [ ] Vorlagen regelmäßig aktualisieren (sonst veralten sie schnell)

---

## Hinweise und Risiken

* Vorinstallierte VMs veralten schnell – ein **reproduzierbares Setup** (Ansible, Dockerfile, Bootstrap-Skript) ist oft wartungsärmer als ein eingefrorenes Image.
* Grundlagen: [Proxmox: VMs und Container](https://github.com/Michdo93/Informatik/blob/main/Virtualisierung/Proxmox.md), [Bootstrapping](https://github.com/Michdo93/Informatik/blob/main/Software-Konzepte/Bootstrapping.md)

---
