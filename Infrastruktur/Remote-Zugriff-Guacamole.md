# 🖥️ Remote-Zugriff (Guacamole, WOLverine)

| | |
| --- | --- |
| **Status** | 🔍 Test ausstehend |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Server |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Laborrechner lassen sich über den Browser fernsteuern, einschalten und überwachen.

---

## Ist-Stand

* Ein Installationsskript für **Apache Guacamole 1.6.0** (mit Tomcat 10, MariaDB, MySQL Connector) liegt vor und ist integriert.
* **WOLverine** – ein Flask-Dashboard zum Ein- und Ausschalten entfernter Rechner (Wake-on-LAN) und zur Überwachung ihrer Auslastung – ist noch nicht integriert.
* Hinweis: Die Repo-Beschreibung des Guacamole-Skripts nennt Ubuntu 20.04, der Repo-Name Ubuntu 24.04 – angleichen.

---

## Offene Aufgaben

* [ ] WOLverine integrieren (Gunicorn, systemd, HTTPS)
* [ ] Wake-on-LAN auf den Zielrechnern aktivieren und testen
* [ ] Zugang zu Guacamole und WOLverine absichern (Authentifizierung, nur im Labornetz)
* [ ] Repo-Beschreibung des Guacamole-Skripts korrigieren

---

## Repositories

* [Apache-Guacamole-1.6.0-Ubuntu-24.04-Install-Script](https://github.com/Michdo93/Apache-Guacamole-1.6.0-Ubuntu-24.04-Install-Script)
* [WOLverine](https://github.com/Michdo93/WOLverine)

---
