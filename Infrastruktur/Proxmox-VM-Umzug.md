# 🚚 VMs in Proxmox umziehen

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🔴 Hoch |
| **Raum** | Server |
| **Geeignet für** | Labormitarbeitende, Praxissemester |

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

Mehrere virtuelle Maschinen müssen innerhalb der Proxmox-Umgebung **umgezogen** werden (anderer Knoten, anderer Speicher oder neu aufgesetzte Umgebung) – ohne Datenverlust und mit möglichst kurzer Ausfallzeit.

---

## Ist-Stand

* Es gibt einen **Proxmox Virtual Environment**-Server und einen **Proxmox Backup Server**; beide werden bereits automatisch per Ansible aktualisiert.
* Welche VMs genau umziehen, wohin und in welcher Reihenfolge, ist in der Tabelle unten zu erfassen.
* Konkret zu migrierende/umzuziehende VMs (aus früherer Planung): Redmine-VM, Projekt-Webserver, openHAB-Cloud, Monitoring-VM, IP-Kamera-VM, Nextcloud (groß, ~800 GB), Pepper-VM (Ubuntu 16.04), ROS-Kinetic-VM (Ubuntu 16.04), zwei „Gesichter zählen“-VMs (Windows 7 → aktuelles Windows).
* Viele VMs laufen noch unter **Ubuntu-Desktop**-Versionen und sollten auf **Ubuntu Server** umgestellt werden; einige brauchen Software-Upgrades und Datenmigration (Redmine/Ruby, Nextcloud, MySQL).

---

## Offene Aufgaben

* [ ] **Bestandsaufnahme:** Tabelle unten für alle betroffenen VMs ausfüllen (ID, Name, Zweck, Ziel, Abhängigkeiten, feste IP/MAC)
* [ ] Für jede VM ein aktuelles **Backup** auf dem Proxmox Backup Server erstellen und die **Wiederherstellung testen**
* [ ] Reihenfolge festlegen: Abhängigkeiten zuerst (z. B. MQTT-Broker vor openHAB, Datenbanken vor Anwendungen)
* [ ] Wartungsfenster festlegen – **nicht** vor Labor-Demos
* [ ] Umzug durchführen (Live-Migration, Offline-Migration oder Backup/Restore, siehe Hinweise)
* [ ] Nach dem Umzug prüfen: Netzwerk, feste IP, Dienste, Autostart (`onboot`), Backups-Job zeigt auf die neue VM
* [ ] Ansible-Inventar und Dokumentation aktualisieren
* [ ] Alte VM erst nach erfolgreichem Test und Wartezeit löschen
* [ ] Pro VM entscheiden: Desktop → Server, Betriebssystem-Upgrade nötig? Software-/Daten-Migration?
* [ ] Alt-VMs mit EOL-Systemen (Ubuntu 16.04, Windows 7) gesondert behandeln (Isolierung, Ersatz, Risiko)
* [ ] Netzwerkzuordnung festlegen (öffentliches Netz / Informatik-Netz / Labornetz), feste IP per MAC

---

## Abhängigkeiten

* [Ansible](Ansible.md)
* [VMs in LXC-Container umwandeln](Proxmox-VM-zu-LXC.md)

---

## Hinweise und Risiken

* **MAC-Adresse beibehalten:** Bei Backup/Restore oder Neuanlage kann sich die MAC-Adresse der virtuellen Netzwerkkarte ändern – dann greift die DHCP-Reservierung nicht mehr und die VM bekommt eine andere IP.
* Innerhalb eines Clusters ist eine Migration per `qm migrate` möglich (mit `--online` im laufenden Betrieb, sofern gemeinsamer Speicher oder `--with-local-disks`). Zwischen getrennten Proxmox-Servern ist **Backup/Restore** über den Backup Server der robusteste Weg.
* Durchgereichte Hardware (USB, PCI) und lokale ISO-Images verhindern eine Live-Migration.
* Grundlagen und Befehle: [Proxmox: VMs und Container](https://github.com/Michdo93/Informatik/blob/main/Virtualisierung/Proxmox.md)

---

## Bestandsaufnahme

| VM-ID | Name | Zweck | Von | Nach | Abhängigkeiten | IP / MAC | Status |
| --- | --- | --- | --- | --- | --- | --- | --- |
| | | | | | | | ☐ |

---

