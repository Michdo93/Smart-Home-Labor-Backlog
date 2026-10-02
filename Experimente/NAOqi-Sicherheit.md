# 🔓 Sicherheit der NAO-/Pepper-Roboter

| | |
| --- | --- |
| **Status** | ⚰️ Deprecated |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Alle (zum Nachlesen), Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Untersuchung, wie ungeschützt die NAOqi-Schnittstelle der Roboter ist – als Sensibilisierung, nicht als Angriffswerkzeug.

---

## Ist-Stand

* Projektidee (WiSe 22/23) „NAOqi Ethical Hacking“: Das NAOqi-SDK lässt sich **ohne Passwort** nutzen – IP und Port 9559 genügen; die JavaScript-Bibliothek ist sogar direkt per HTTP erreichbar.
* Dazu existierte `pepper_brute_force` (fährt alle Pepper im Netz herunter) – im Backlog bereits als deprecated unter [Pepper-Concierge → Historie](../Demos/Pepper-Concierge.md) geführt und **nicht zu verwenden**.

---

## Offene Aufgaben

* [ ] Die Erkenntnis dokumentieren: Roboter gehören in ein **getrenntes, geschütztes Netz** (VLAN), Zugriff nur aus dem Labornetz
* [ ] Keine Angriffsskripte im Repo belassen; `pepper_brute_force` archivieren
* [ ] Als Hinweis in die Sicherheits-/Netzwerkdokumentation aufnehmen

---

## Hinweise und Risiken

* Nur im eigenen Labornetz und zu Lehrzwecken. Grundlagen: [Zugriffskontrolle](https://github.com/Michdo93/Informatik/blob/main/Zugriffskontrolle/README.md), [Netzwerk-Grundlagen](https://github.com/Michdo93/Informatik/blob/main/Netzwerk/Netzwerk-Grundlagen.md)

---

## Repositories

* [pepper_brute_force](https://github.com/Michdo93/pepper_brute_force)

---
