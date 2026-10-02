# 🦄 Python-Webanwendungen auf Gunicorn umstellen

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟠 Mittel |
| **Raum** | Server / Raspberry Pis |
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

Alle Flask- und anderen WSGI-Anwendungen im Labor laufen mit **Gunicorn als systemd-Service** (ggf. hinter Nginx) statt mit dem Entwicklungsserver (`python3 app.py`).

---

## Ist-Stand

* Eine deutschsprachige Anleitung zur Einrichtung eines WSGI-Servers liegt vor (Repo `WSGI-Server`).
* Der Großteil der Anwendungen läuft aber **noch direkt unter `python3`**.

---

## Offene Aufgaben

* [ ] Liste aller Python-Webanwendungen im Labor erstellen (Gerät, Repo, Port, Startweg)
* [ ] Pro Anwendung: virtuelle Umgebung, `gunicorn` installieren, systemd-Unit anlegen
* [ ] Wo sinnvoll: Nginx davor, HTTPS
* [ ] Debug-Modus abschalten
* [ ] Anleitung im Repo `WSGI-Server` an die Best Practices angleichen
* [ ] In den READMEs der Projekte den Betrieb mit Gunicorn dokumentieren

---

## Hinweise und Risiken

* Grundlagen: [Web-Server & Deployment](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/Web-Server%20%26%20Deployment.md), [systemd-Services](https://github.com/Michdo93/Informatik/blob/main/Linux%20%26%20Werkzeuge/systemd-Services.md)

---

## Repositories

* [WSGI-Server](https://github.com/Michdo93/WSGI-Server)
* [WOLverine](https://github.com/Michdo93/WOLverine)

---
