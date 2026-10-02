# 📦 VMs in LXC-Container umwandeln

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟠 Mittel |
| **Raum** | Server |
| **Geeignet für** | Labormitarbeitende, Praxissemester |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Dienste, die keine vollständige VM brauchen, sollen künftig in **LXC-Containern** laufen. Das spart RAM, CPU und Speicher, und Container starten und sichern sich schneller.

---

## Ist-Stand

* Einige Dienste laufen derzeit in vollständigen Proxmox-VMs.
* Welche VMs sich eignen, ist noch zu bewerten (siehe Kriterien).

---

## Offene Aufgaben

* [ ] Alle VMs nach den Kriterien unten bewerten und Kandidaten in einer Tabelle festhalten
* [ ] Für jeden Kandidaten: Dienste, Konfigurationsdateien, Daten, Ports, Cron-Jobs und systemd-Services dokumentieren
* [ ] LXC aus einer aktuellen Vorlage erstellen (bevorzugt **unprivilegiert**)
* [ ] Dienste neu installieren – möglichst per **Ansible**, damit es reproduzierbar ist
* [ ] Daten und Konfiguration übertragen (`rsync`, Datenbank-Export/-Import)
* [ ] Parallel testen, dann die IP-Adresse bzw. DHCP-Reservierung umstellen
* [ ] VM stoppen, nach einer Wartezeit sichern und löschen

---

## Abhängigkeiten

* [VMs in Proxmox umziehen](Proxmox-VM-Umzug.md)
* [Ansible](Ansible.md)

---

## Hinweise und Risiken

* Es gibt **keine direkte Konvertierung** VM → LXC. Ein LXC teilt sich den Kernel mit dem Proxmox-Host – man baut den Dienst im Container neu auf und überträgt Daten und Konfiguration.
* **Gut geeignet:** Linux-Dienste ohne besondere Kernel-Anforderungen – Web-Server, MQTT-Broker, Datenbanken, Python-Dienste, Asterisk-ähnliche Server sind meist unkritisch.
* **Ungeeignet oder aufwendig:** Windows, eigene Kernel/Kernel-Module, manche VPN-Lösungen, Dienste mit direktem Hardwarezugriff (USB/IP, GPU) und **Docker** (in LXC nur mit `nesting` und Einschränkungen – die Docker-VM bleibt deshalb sinnvollerweise eine VM).
* Nach dem Umzug ändert sich die MAC-Adresse → DHCP-Reservierung anpassen.
* Grundlagen: [Proxmox: VMs und Container](https://github.com/Michdo93/Informatik/blob/main/Virtualisierung/Proxmox.md)

---

