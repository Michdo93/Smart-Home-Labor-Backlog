# 🤳 Pepper-Selfie

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟠 Mittel |
| **Raum** | – |
| **Geeignet für** | Hiwi, Praxissemester |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Pepper macht auf Wunsch ein Foto, zeigt es an und druckt es aus.

---

## Ist-Stand

* Integriert ist eine Java-Anwendung (Pepper 1.8a, NAOqi 2.5), die den Kamerastream an einen Webserver überträgt und über einen Client anzeigt – sie **muss refactort werden**.
* Eine Python-Variante (Python 2.7, NAOqi 2.5) ließ sich **nicht zum Laufen bringen**.
* Der Druck soll über den Etikettendrucker Brother VC-500W erfolgen.

---

## Offene Aufgaben

* [ ] Java-Anwendung refactoren und dokumentieren
* [ ] Druckerstatus (Rolle leer, druckbereit) einbinden
* [ ] Bildformat für den Druck optimieren (Weißraum, Papierverbrauch)
* [ ] Entscheiden, ob die Python-Variante weiterverfolgt oder archiviert wird

---

## Abhängigkeiten

* [Brother VC-500W](../Experimente/Brother-VC-500W.md)
* [Pepper-Concierge](Pepper-Concierge.md)

---

## Repositories

* [PepperSelfie](https://github.com/Michdo93/PepperSelfie)
* [Pepper-Selfie-Python](https://github.com/Michdo93/Pepper-Selfie-Python)

---
