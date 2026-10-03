# 📜 Migration der Rules

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🔴 Hoch |
| **Raum** | – |
| **Geeignet für** | Labormitarbeitende, Praxissemester |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Grundlagen](#grundlagen)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Alle Rules laufen fehlerfrei auf den aktuellen Rule Engines (vor allem **Python 3 Scripting**).

---

## Ist-Stand

* Einige Rules sind noch nicht migriert bzw. noch nicht getestet.
* Die [Morgenroutine](../Demos/Morgenroutine.md) läuft zeitlich nicht korrekt.
* Die openHAB Design Patterns wurden bereits auf Rules DSL, JavaScript Scripting und Python 3 Scripting übertragen.
* Umfangreiche **Referenzsammlung** zu openHAB Design Patterns (Time of Day, Gate Keeper, Debounce, Proxy Item, Separation of Behaviors, Timer Management u. v. m.) liegt als Material vor und fließt in Buch und Beispiel-Repo ein.
* Tests mit openHAB 5 und **GraalPy** liegen im Repository `openHAB5-Test`.

---

## Offene Aufgaben

* [ ] Übersicht aller Rules mit Migrationsstatus erstellen
* [ ] Verbleibende kleinere Rules migrieren und testen
* [ ] Rules mit Wartezeiten/Threads besonders prüfen

---

## Grundlagen

* [openHAB: Betrieb & Konfiguration](https://github.com/Michdo93/Informatik/blob/main/openHAB/Betrieb%20%26%20Konfiguration.md) – Rule Engines und openHAB-Entwurfsmuster
* [Refactoring & Migration](https://github.com/Michdo93/Informatik/blob/main/Software-Konzepte/Refactoring%20%26%20Migration.md) – Jython/DSL → Python 3, Timing und Nebenläufigkeit

---

## Repositories

* [openhab-design-patterns-examples](https://github.com/Michdo93/openhab-design-patterns-examples)
* [openHAB5-Test](https://github.com/Michdo93/openHAB5-Test)

---
