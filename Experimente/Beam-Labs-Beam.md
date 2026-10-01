# 💡 Beam Labs Beam (Projektor-Lampen)

| | |
| --- | --- |
| **Status** | 🧪 Experiment |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Die Projektor-Lampen ohne die veraltete App steuern und einrichten.

---

## Ist-Stand

* Eine der Lampen bootet nicht richtig.
* Zur Konfiguration muss über Umwege eine alte Android-App installiert werden.
* Die App wurde vor Jahren dekompiliert. Mit einer eigenen Java-Anwendung ließen sich keine Befehle senden; die von der App gesendeten Befehle und Zustandsänderungen konnten aber mitgelesen werden.
* Auf dieser Basis liegt ein KI-generiertes Python-Werkzeug vor.

---

## Offene Aufgaben

* [ ] `beamctl` testen
* [ ] Prüfen, ob sich WLAN per **Bluetooth** aktivieren und konfigurieren lässt (Umgehung der App)
* [ ] Defekte Lampe prüfen

---

## Repositories

* [beamctl](https://github.com/Michdo93/beamctl)
* [Beam-Remote-Decompiled](https://github.com/Michdo93/Beam-Remote-Decompiled)

---
