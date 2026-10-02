# 📡 MQTT Live Monitor

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Server |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Eine Weboberfläche zeigt live, welche MQTT-Topics abonniert sind und welche Nachrichten ankommen – zur Fehlersuche im Labor.

---

## Ist-Stand

* Die Anwendung nutzt MQTT über WebSockets und zeigt Topics und Nachrichten auf der Webseite und in der Browser-Konsole.
* Sie ist noch nicht in die Laborinfrastruktur integriert.

---

## Offene Aufgaben

* [ ] WebSocket-Listener am Broker prüfen bzw. einrichten (mit TLS und Passwort)
* [ ] Bereitstellen (z. B. statisch über Nginx oder den openHAB-Webserver)
* [ ] Zugriff absichern: Der Monitor sieht **alle** Nachrichten – eigener MQTT-Benutzer mit nur lesender ACL

---

## Hinweise und Risiken

* Best Practice: [MQTT](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/MQTT.md)

---

## Repositories

* [MQTT-Live-Monitor](https://github.com/Michdo93/MQTT-Live-Monitor)

---
