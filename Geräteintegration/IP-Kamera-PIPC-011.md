# 📷 PTZ-IP-Kamera PremiumBlue PIPC-011

| | |
| --- | --- |
| **Status** | ⛔ Blockiert |
| **Priorität** | 🟠 Mittel |
| **Raum** | – |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Die schwenkbare IP-Kamera soll mit Livebild und allen Steuerbefehlen in openHAB verfügbar sein.

---

## Ist-Stand

* Kamera-Stream über das **ipcamera-Binding**.
* Steuerung über ein eigenes Python-Skript und das **MQTT-Binding**.
* **Problem:** Nach einem Neustart ist die Kamera abgestürzt und benötigte einen **Hardware-Reset**.
* Hinweis: Die Kamera wurde zunächst für eine **LogiLink WC0030A** gehalten; tatsächlich ist es eine **PremiumBlue PIPC-011**.

---

## Offene Aufgaben

* [ ] Absturz nach Neustart reproduzieren und Ursache finden
* [ ] Alle Steuerbefehle testen
* [ ] Python-Steuerung als Dienst betreiben

---

## Repositories

* [PremiumBlue-PIPC-011-Python](https://github.com/Michdo93/PremiumBlue-PIPC-011-Python)

---
