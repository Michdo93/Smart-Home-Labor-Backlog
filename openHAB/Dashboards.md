# 🖥️ Eigene HTML-Dashboards

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟠 Mittel |
| **Raum** | Alle Räume |
| **Geeignet für** | Hiwi, Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
<!-- /TOC -->

## Ziel

Eigene Dashboards in HTML/CSS/JavaScript als ansprechendere Alternative zu Sitemaps, HABPanel und CometVisu.

---

## Ist-Stand

* Dashboards liegen unter `/etc/openhab/html/dashboards` und sind unter `/static/dashboards/` erreichbar. Vorteile: kein zusätzlicher Webserver, und die Dashboards sind im Backup von `/etc/openhab` enthalten.
* Zugriff auf openHAB über eine **eigene JavaScript-Bibliothek** für die REST API.
* Die Anwendung könnte auch auf jedem anderen Webserver laufen.
* HABPanel und CometVisu wurden verworfen, weil ein gutes Design dort deutlich aufwendiger war.

---

## Offene Aufgaben

* [ ] Alle Räume vervollständigen
* [ ] Für die [Wand-Tablets](../Infrastruktur/Tablets-und-Kiosk.md) optimieren

---

