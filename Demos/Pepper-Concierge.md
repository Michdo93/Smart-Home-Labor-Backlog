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
<!-- /TOC -->

## Ziel

Der Pepper-Concierge soll als Labor-Demo zuverlässig laufen.

---

## Ist-Stand

* Die IP-Adresse des zugehörigen Raspberry Pi hat sich geändert und wurde in der Konfigurationsdatei des Concierge bereits angepasst.
* Der Sonos-Lautsprecher im Multimedia-Raum wird nicht über openHAB, sondern direkt über eine JAR-Datei mit eigener Bibliothek angesprochen. Deshalb hatte er als einziges Sonos-Gerät schon eine feste IP-Adresse.
* Alle Geräte (inkl. Pepper) wurden durchgemessen.

---

## Offene Aufgaben

* [ ] Beamer wieder **automatisch ein- und ausschalten** (Codeänderung im Concierge) – optional, falls die Zeit reicht
* [ ] Klären, wie es mit Pepper insgesamt weitergeht

---

## Abhängigkeiten

* [BenQ MH856UST](../Geräteintegration/BenQ-MH856UST.md)
* [Sonos und Webradio](../Geräteintegration/Sonos-und-Webradio.md)

---

## Hinweise und Risiken

* Dass der Beamer vorher schon dauerhaft eingeschaltet war, hat in Demos bisher nicht gestört.

---

