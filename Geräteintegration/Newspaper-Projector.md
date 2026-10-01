# 📰 Newspaper Projector

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🔴 Hoch |
| **Raum** | Multimedia |
| **Geeignet für** | Hiwi, Praxissemester |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Ein kleiner Projektor zeigt morgens die **aktuelle Tageszeitung** an – als Teil der Morgenroutine. Später soll er über **Gesten** (hoch/runter, links/rechts) bedient werden.

---

## Ist-Stand

* Hardware: **BeagleBone Black** mit dem selbst programmierbaren Projektor **DLPDLCR2000EVM**.
* ✅ Projektor funktioniert.
* ✅ Die Zeitung wird täglich neu generiert.
* ✅ Web-App funktioniert.
* ✅ openHAB-Integration über das **MQTT-Binding** funktioniert.
* Die Ausrichtung (gedreht/gespiegelt) ist umgesetzt: Liest man von innen, muss das Bild nicht gedreht werden, von außen schon.
* Die letzten Änderungen (angepasste I2C-Befehle) sind noch nicht auf das Board übertragen.
* ⏳ Gestensteuerung über **Raspberry Pi + Kinect**: Die Software läuft, die Kamera wirft keine Fehler mehr. Ob Gesten richtig erkannt werden, ist noch nicht getestet. Der Code ist bislang KI-generiert.

---

## Offene Aufgaben

* [ ] Angepasste I2C-Befehle auf das Board übertragen
* [ ] Gestenerkennung **mit GUI** testen: Kamera am Laptop bzw. an einer Ubuntu-VM, um zu sehen, was erkannt wird
* [ ] Gestenerkennung anpassen und auf dem Raspberry Pi in Betrieb nehmen
* [ ] **Switch** für den Raspberry Pi besorgen, damit er per LAN-Kabel am gewünschten Ort angeschlossen werden kann
* [ ] Bildausrichtung in der Morgenroutine passend steuern
* [ ] In die [Morgenroutine](../Demos/Morgenroutine.md) integrieren

---

## Hinweise und Risiken

* Auf demselben Raspberry Pi läuft bereits der [People Counter](People-Counter.md).

---

## Repositories

* [newspaperprojector](https://github.com/Michdo93/newspaperprojector)
* [newspaperprojector-gesture-control](https://github.com/Michdo93/newspaperprojector-gesture-control)

---
