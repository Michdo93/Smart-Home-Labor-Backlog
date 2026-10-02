# 🗓️ Laufender Betrieb (Daily Business)

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🔴 Hoch |
| **Raum** | Alle Räume |
| **Geeignet für** | Hiwi, Praxissemester |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Wiederkehrende Aufgaben, die anfallen, damit Labor, Demos und Lehrveranstaltungen funktionieren. Sie sind nie „fertig“, sondern werden regelmäßig erledigt.

---

## Ist-Stand

* Updates von openHAB-Server, Proxmox VE und Proxmox Backup Server laufen automatisiert über Ansible; Git-Backups von openHAB jeden Sonntag.
* Alle Geräte wurden durchgemessen.

---

## Offene Aufgaben

* [ ] **Wöchentlich:** Ergebnis der automatischen Updates und Backups prüfen (Ansible-Läufe, Proxmox-Backup-Jobs, Git-Backup)
* [ ] **Wöchentlich:** Dienste-Status prüfen (openHAB, MQTT-Broker, Docker-Container, Dashboards)
* [ ] **Vor jeder Labor-Demo:** Demo-Abläufe testen (Morgenroutine, Pepper-Concierge), Geräte einschalten und prüfen, Tablets laden; keine Updates oder Umbauten kurz vorher
* [ ] **Nach jeder Labor-Demo:** Labor aufräumen, Geräte in den Ausgangszustand, Defekte melden
* [ ] **Vor Semesterbeginn:** Praktika vorbereiten (z. B. Boxen für das Plattformen-Praktikum zusammenstellen, SD-Karten neu formatieren bzw. flashen, Laborrechner testen, Roboter wie die GoPiGos prüfen)
* [ ] **Regelmäßig:** Batterien von Funksensoren prüfen und tauschen
* [ ] **Regelmäßig:** Zertifikate auf Ablaufdatum prüfen
* [ ] **Nach Bedarf:** Neue Geräte aufnehmen (feste IP, Hostname, SSH, Ansible-Inventar, Dokumentation)
* [ ] **Laufend:** Erledigte Aufgaben im Backlog und in den Projekt-Repositories abhaken

---

## Abhängigkeiten

* [Ansible](../Infrastruktur/Ansible.md)
* [Morgenroutine](../Demos/Morgenroutine.md)
* [Pepper-Concierge](../Demos/Pepper-Concierge.md)

---

## Hinweise und Risiken

* Diese Liste ist ein Anfang – bitte um weitere wiederkehrende Aufgaben ergänzen.
* Wo möglich automatisieren (Ansible, systemd-Timer) und nur das **Prüfen** als Aufgabe stehen lassen.
* Grundlagen: [Best Practices](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/README.md), [Backup-Strategien](https://github.com/Michdo93/Informatik/blob/main/Backup-Strategien/README.md), [Cron & systemd-Timer](https://github.com/Michdo93/Informatik/blob/main/Linux%20%26%20Werkzeuge/Cron%20%26%20systemd-Timer.md)

---

