# 🔳 Geräteerkennung per QR-Code

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Alle Räume |
| **Geeignet für** | Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Ein Webdienst liefert zu jedem Gerät im Labor Informationen, die über einen QR-Code abgerufen werden. Pepper, HoloLens oder Handykameras erkennen ein Gerät am QR-Code und wissen, worum es sich handelt.

---

## Ist-Stand

* Projektidee (WiSe 22/23): ursprünglich mit Barcodes, besser mit QR-Codes.
* Die QR-Code-Grundlagen sind im Labor bereits vorhanden: Scanner-Web-App, QR-Generator, QR-zu-PDF (siehe [QR-Code-Steuerung](../Geräteintegration/QR-Code-Steuerung.md)).
* Neu gegenüber der bestehenden QR-Steuerung ist die **Gerätedatenbank mit Infos** statt nur der Bedienung.

---

## Offene Aufgaben

* [ ] Datenmodell für Geräteinfos festlegen (Name, Raum, Handbuch, Wartung, openHAB-Items)
* [ ] Webdienst, der zu einer QR-Code-ID die Geräteinfos liefert
* [ ] Mit der vorhandenen Scanner-App verbinden

---

## Abhängigkeiten

* [QR-Code-Steuerung](../Geräteintegration/QR-Code-Steuerung.md)

---

## Hinweise und Risiken

* Verwandt mit der Idee [AR-Steuerung mit openHAB](https://github.com/Michdo93/SmartHome-Ideen) (Geräteerkennung per Kamera).
* Grundlagen: [Relationale Modellierung](https://github.com/Michdo93/Informatik/blob/main/Datenbanken/Relationale%20Modellierung.md)

---

