# 🤖 Pepper-Concierge

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🔴 Hoch |
| **Raum** | Multimedia |
| **Geeignet für** | Labormitarbeitende, Praxissemester |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Der Pepper-Concierge soll als Labor-Demo zuverlässig laufen.

---

## Ist-Stand

* Die IP-Adresse des zugehörigen Raspberry Pi hat sich geändert und wurde in der Konfigurationsdatei des Concierge bereits angepasst.
* Der Sonos-Lautsprecher im Multimedia-Raum wird nicht über openHAB, sondern direkt über eine JAR-Datei mit eigener Bibliothek angesprochen. Deshalb hatte er als einziges Sonos-Gerät schon eine feste IP-Adresse.
* Alle Geräte (inkl. Pepper) wurden durchgemessen.
* Die Anwendung läuft mit **NAOqi 2.5 und Python 2.7** (`Pepper-Concierge-Python`) und **muss refactort werden**; ebenso die SSH-Kurzvariante `Pepper_ConciergeShortSSH` (Java).
* Ein ROS-2-Workspace für Pepper (`pepper_ros2_ws`) liegt vor, ist aber ungetestet.
* Die frühere Kurzvariante `Pepper_ConciergeShort` ist deprecated.

---

## Offene Aufgaben

* [ ] Beamer wieder **automatisch ein- und ausschalten** (Codeänderung im Concierge) – optional, falls die Zeit reicht
* [ ] Klären, wie es mit Pepper insgesamt weitergeht
* [ ] `Pepper-Concierge-Python` refactoren: Konfiguration (IPs, Geräte) aus dem Code in eine Konfigurationsdatei, Python-2.7-Teil auf das Nötigste beschränken
* [ ] `Pepper_ConciergeShortSSH` refactoren oder in die Hauptanwendung überführen
* [ ] `pepper_ros2_ws` testen

---

## Abhängigkeiten

* [BenQ MH856UST](../Geräteintegration/BenQ-MH856UST.md)
* [Sonos und Webradio](../Geräteintegration/Sonos-und-Webradio.md)
* [Pepper-Selfie](Pepper-Selfie.md)

---

## Hinweise und Risiken

* Dass der Beamer vorher schon dauerhaft eingeschaltet war, hat in Demos bisher nicht gestört.

---

## Repositories

* [Pepper-Concierge-Python](https://github.com/Michdo93/Pepper-Concierge-Python)
* [Pepper_ConciergeShortSSH](https://github.com/Michdo93/Pepper_ConciergeShortSSH)
* [pepper_ros2_ws](https://github.com/Michdo93/pepper_ros2_ws)

---
