# 🎛️ Roboter-Controller in mehreren Sprachen

| | |
| --- | --- |
| **Status** | 🔍 Test ausstehend |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Studienprojekt |

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

Beispielanwendungen, die Pepper und Nao über ihre SDKs steuern – jeweils in verschiedenen Sprachen und mit verschiedenen Anbindungen (Controller-App, MQTT, Flask), als Lehr- und Demonstrationsmaterial.

---

## Ist-Stand

* Aus den Projektarbeiten (WiSe 22/23) sind zahlreiche Beispiel-Repos entstanden: `pepper-java-example`, `pepper-java-ee-example`, `pepper-javascript-example`, `pepper-python-flask-example`, der `pepper_controller` (pynput) sowie `albehaviormanager` (Behaviour Manager für Pepper und Nao).
* Die SDKs selbst sind als Repos abgelegt (`pynaoqi-*`, `naoqi-sdk-*`, `java-naoqi-sdk-*`, `jnaoqi*`).
* Die Controller-App-Varianten (Android/Java/Java-EE/JavaScript/Python-Flask/MQTT) für Pepper und Nao waren jeweils eigene Projektthemen.

---

## Offene Aufgaben

* [ ] Sichten, welche Beispiel-Repos aktuell und lauffähig sind
* [ ] Eine **Übersicht** erstellen, welches Beispiel welche Sprache/Anbindung zeigt
* [ ] Veraltete Varianten zusammenführen oder als deprecated kennzeichnen
* [ ] Bezug zur aktuellen Pepper-/Nao-Nutzung herstellen (Concierge, Selfie, ROS 2)

---

## Abhängigkeiten

* [Pepper-Concierge](../Demos/Pepper-Concierge.md)
* [NAO Gym Instructor](NAO-Gym-Instructor.md)

---

## Hinweise und Risiken

* Viele dieser Beispiele stammen aus 2022 und dienen vor allem als **Lernmaterial**. Für den Produktivbetrieb zählt, was im [Pepper-Concierge](../Demos/Pepper-Concierge.md) und bei [Pepper-Selfie](../Demos/Pepper-Selfie.md) läuft.

---

## Repositories

* [pepper-java-example](https://github.com/Michdo93/pepper-java-example)
* [pepper-java-ee-example](https://github.com/Michdo93/pepper-java-ee-example)
* [pepper-javascript-example](https://github.com/Michdo93/pepper-javascript-example)
* [pepper-python-flask-example](https://github.com/Michdo93/pepper-python-flask-example)
* [pepper_controller](https://github.com/Michdo93/pepper_controller)
* [albehaviormanager](https://github.com/Michdo93/albehaviormanager)

---
