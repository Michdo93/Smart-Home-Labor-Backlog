# 🐳 Container in der Docker-VM

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🔴 Hoch |
| **Raum** | Server |
| **Geeignet für** | Hiwi, Praxissemester |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Bestandsaufnahme](#bestandsaufnahme)
<!-- /TOC -->

## Ziel

Alle Container in der Docker-VM sind **einheitlich, nachvollziehbar und wiederherstellbar** konfiguriert: als Docker-Compose-Stacks mit festen Versionen, sauberen Volumes, Zugangsdaten außerhalb der Compose-Datei, Backups und dokumentiertem Update-Weg.

---

## Ist-Stand

* Es gibt eine Docker-VM in Proxmox mit mehreren Containern.
* Die Container müssen **alle angepasst und konfiguriert** werden.

---

## Offene Aufgaben

* [ ] **Bestandsaufnahme:** `docker ps -a`, `docker volume ls`, `docker network ls` – Tabelle unten ausfüllen
* [ ] Für jeden Container, der per `docker run` gestartet wurde: in eine **`compose.yaml`** überführen (ein Verzeichnis pro Stack, z. B. `/opt/stacks/<name>/`)
* [ ] **Image-Versionen festschreiben** (kein `:latest`)
* [ ] Zugangsdaten in `.env`-Dateien mit Rechten `600` auslagern; `.env` nicht ins Git
* [ ] Volumes prüfen: Welche Daten sind persistent? Bind-Mounts oder benannte Volumes – einheitlich festlegen
* [ ] `restart: unless-stopped`, Healthchecks und Log-Begrenzung (`max-size`) setzen
* [ ] Weboberflächen hinter einen Reverse Proxy mit HTTPS stellen
* [ ] Backup der Volumes und Compose-Dateien einrichten und **Wiederherstellung testen**
* [ ] Nicht mehr benötigte Container, Images und Volumes entfernen
* [ ] Update-Vorgehen dokumentieren (`docker compose pull && docker compose up -d`) und Compose-Dateien versionieren

---

## Abhängigkeiten

* [VMs in Proxmox umziehen](Proxmox-VM-Umzug.md)

---

## Hinweise und Risiken

* Bevor ein Container neu erstellt wird: prüfen, ob seine Daten in einem Volume liegen. Daten im Container-Dateisystem gehen beim Neuerstellen **verloren**.
* Ports nur dort veröffentlichen, wo nötig – idealerweise nur auf `127.0.0.1` hinter dem Reverse Proxy.
* Grundlagen: [Docker & Compose betreiben](https://github.com/Michdo93/Informatik/blob/main/Virtualisierung/Docker%20%26%20Compose.md), [Web-Server & Deployment](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/Web-Server%20%26%20Deployment.md)

---

## Bestandsaufnahme

| Container / Stack | Image + Version | Zweck | Ports | Volumes | Compose? | Backup? | Status |
| --- | --- | --- | --- | --- | --- | --- | --- |
| | | | | | ☐ | ☐ | ☐ |

---

