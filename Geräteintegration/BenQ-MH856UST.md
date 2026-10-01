# 📽️ BenQ MH856UST (Beamer)

| | |
| --- | --- |
| **Status** | 🔍 Test ausstehend |
| **Priorität** | 🔴 Hoch |
| **Raum** | Multimedia |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Ideen und Szenarien](#ideen-und-szenarien)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Der Beamer soll zuverlässig über openHAB gesteuert werden – mit Befehlen **und** korrekten Zuständen.

---

## Ist-Stand

* **Ansatz 1 – RS232:** Befehle kamen an, die Rückmeldungen (States) waren wegen eines unzureichenden Spannungspegels unbrauchbar.
* **Ansatz 2 – Crestron RoomView:** Steuerung der Flash-Anwendung auf dem Beamer per PyAutoGUI. Funktionierte, ist aber eine Notlösung.
* **Ansatz 3 – RS232 über TCP (LAN):** Aktueller Ansatz. Ein Python-Programm auf einem Raspberry Pi sendet die RS232-Befehle per TCP und ist per MQTT an openHAB angebunden.

---

## Offene Aufgaben

* [ ] Ansatz 3 vollständig testen (alle Befehle, alle Zustände)
* [ ] Dauerbetrieb einrichten (systemd-Service, MQTT mit Passwort und TLS)
* [ ] Alte Ansätze als veraltet kennzeichnen
* [ ] Automatisches Ein-/Ausschalten für den [Pepper-Concierge](../Demos/Pepper-Concierge.md) ermöglichen

---

## Ideen und Szenarien

* Zusammenspiel mit [WebTV](../Experimente/WebTV.md): Sender wählen → Beamer an → Quelle Raspberry Pi → Stream im Vollbild.

---

## Repositories

* [BenQ-RS232-TCP](https://github.com/Michdo93/BenQ-RS232-TCP)
* [openHAB-Crestron-RoomView-Control](https://github.com/Michdo93/openHAB-Crestron-RoomView-Control)
* [crestron-roomview](https://github.com/Michdo93/crestron-roomview)

---
