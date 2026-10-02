# 🎥 Interaktion mit Kinect-Kameras

| | |
| --- | --- |
| **Status** | 🧪 Experiment |
| **Priorität** | 🟠 Mittel |
| **Raum** | Multimedia, IoT |
| **Geeignet für** | Studienprojekt, Abschlussarbeit |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Mit Kinect-Kameras (V1 und V2) entstehen berührungslose Bedienkonzepte: unsichtbare Schalter an der Wand, interaktive Projektionen, ein virtuelles Theremin.

---

## Ist-Stand

* **invisible-spatial-switch:** macht Wände mit einer Kinect V1 und einem Raspberry Pi bzw. Ubuntu-Server zu unsichtbaren Touch-Flächen (Zonen, Schieberegler, Farbräder) – ungetestet.
* **interactive-projector:** Kinect V2 + Projektor, Bild nach Kalibrierung interaktiv steuerbar – ungetestet.
* **therenect-linux:** Linux-Portierung eines virtuellen Theremins für die Kinect V1 (Original von Martin Kaltenbrunner, GPL) – ungetestet.
* Die Gestensteuerung des Newspaper Projectors nutzt ebenfalls eine Kinect.

---

## Offene Aufgaben

* [ ] Projekte einzeln testen (zunächst mit GUI am Laptop/in einer Ubuntu-VM)
* [ ] Hardware zuordnen: Welche Kinect (V1/V2) steht wo zur Verfügung?
* [ ] Funktionierende Projekte per MQTT an openHAB anbinden
* [ ] Lizenzbedingungen bei therenect-linux beachten (GPL)

---

## Repositories

* [invisible-spatial-switch](https://github.com/Michdo93/invisible-spatial-switch)
* [interactive-projector](https://github.com/Michdo93/interactive-projector)
* [therenect-linux](https://github.com/Michdo93/therenect-linux)
* [newspaperprojector-gesture-control](https://github.com/Michdo93/newspaperprojector-gesture-control)

---
