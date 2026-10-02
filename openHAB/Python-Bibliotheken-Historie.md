# 📚 Frühere Python-Bibliotheken und Proxys für openHAB

| | |
| --- | --- |
| **Status** | ⚰️ Deprecated |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Alle (zum Nachlesen) |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Ideen und Szenarien](#ideen-und-szenarien)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Dokumentation der früheren Python-Werkzeuge rund um die openHAB REST API – aus ihnen sind die heutigen REST-Clients und Test Suites entstanden.

---

## Ist-Stand

* **REST-Zugriff:** `python-openhab` (Bibliothek für die REST API), `python-openhab-crud` bzw. `openhab_python_crud` (CRUD lokal oder über die Cloud), `openhab-python-rest-api-examples` (Beispiele lokal und über die Cloud).
* **Item-Modell:** `python-openhab-item` bzw. `openHAB-Python-Item` – je Item-Typ eine eigene Klasse.
* **Ereignisse:** `python-openhab-itemevents` bzw. `openHAB-Python-ItemEvents` – Item-Events über Server-Sent Events der REST API.
* **Event-Bus:** `python-openhab-eventbus` und `openHAB-Helper-Libraries-MQTT-Event-Bus` (Helper Libraries für openHAB 2/3) – MQTT-Event-Bus für openHAB.
* **Logs:** `python-openhab-logsaver` bzw. `openHAB-LogSaver` – openHAB-Logs in einer Datenbank speichern.
* **Proxys:** `openHAB-Command-Proxy` und `openHAB-Command-Proxy-Jython` (Commands per GET-Request, weitergeleitet als POST) sowie `openHAB-REST-API-Proxy` (Proxy mit CORS-Headern).
* **Kompendien:** `openHAB-Python-Compendium` und `Exec-Binding-and-Exec-Action-Compendium`.
* **Nachfolger:** REST-Zugriff und Events über `python-openhab-rest-client` (und die Clients in sieben weiteren Sprachen); der Event-Bus über `HABApp-MQTT-Event-Bus`; das Wissen der Kompendien steckt heute im Kompendium Informatik und im Buch zu den openHAB Design Patterns.
* Mehrere Repos existieren doppelt unter zwei Namen (z. B. `python-openhab-item` und `openHAB-Python-Item`) – vermutlich Umbenennungen bzw. Neuauflagen.

---

## Offene Aufgaben

* [ ] Deprecated-Hinweise mit Nachfolger in die READMEs aufnehmen und Repos archivieren (siehe [Deprecated Repositories kennzeichnen und archivieren](../Infrastruktur/Deprecated-Repos-aufraeumen.md))
* [ ] Bei Doppelungen festhalten, welches Repo das ursprüngliche ist

---

## Abhängigkeiten

* Nachfolger: [openHAB REST-Clients und Test Suites](REST-Clients-und-Test-Suites.md)

---

## Ideen und Szenarien

* Der **LogSaver** (Logs in eine Datenbank) und der **CORS-Proxy** lösen Probleme, die es weiterhin gibt – wer daran anknüpfen will, findet hier einen Startpunkt (heute eher mit Loki/Grafana bzw. Nginx als Reverse Proxy, siehe [Web-Server & Deployment](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/Web-Server%20%26%20Deployment.md)).

---

## Repositories

* [python-openhab](https://github.com/Michdo93/python-openhab)
* [python-openhab-crud](https://github.com/Michdo93/python-openhab-crud)
* [openhab_python_crud](https://github.com/Michdo93/openhab_python_crud)
* [openhab-python-rest-api-examples](https://github.com/Michdo93/openhab-python-rest-api-examples)
* [python-openhab-item](https://github.com/Michdo93/python-openhab-item)
* [openHAB-Python-Item](https://github.com/Michdo93/openHAB-Python-Item)
* [python-openhab-itemevents](https://github.com/Michdo93/python-openhab-itemevents)
* [openHAB-Python-ItemEvents](https://github.com/Michdo93/openHAB-Python-ItemEvents)
* [python-openhab-eventbus](https://github.com/Michdo93/python-openhab-eventbus)
* [openHAB-Helper-Libraries-MQTT-Event-Bus](https://github.com/Michdo93/openHAB-Helper-Libraries-MQTT-Event-Bus)
* [python-openhab-logsaver](https://github.com/Michdo93/python-openhab-logsaver)
* [openHAB-LogSaver](https://github.com/Michdo93/openHAB-LogSaver)
* [openHAB-Command-Proxy](https://github.com/Michdo93/openHAB-Command-Proxy)
* [openHAB-Command-Proxy-Jython](https://github.com/Michdo93/openHAB-Command-Proxy-Jython)
* [openHAB-REST-API-Proxy](https://github.com/Michdo93/openHAB-REST-API-Proxy)
* [openHAB-Python-Compendium](https://github.com/Michdo93/openHAB-Python-Compendium)
* [Exec-Binding-and-Exec-Action-Compendium](https://github.com/Michdo93/Exec-Binding-and-Exec-Action-Compendium)

---
