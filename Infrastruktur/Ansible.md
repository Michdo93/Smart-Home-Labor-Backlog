# ⚙️ Ansible

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟠 Mittel |
| **Raum** | Server / alle Systeme |
| **Geeignet für** | Hiwi, Praxissemester |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Updates, Upgrades und Backups aller Laborsysteme laufen so weit wie möglich **automatisiert** über Ansible.

---

## Ist-Stand

* Ansible ist eingerichtet und teilweise konfiguriert.
* Automatische Updates/Upgrades aktiv für: **openHAB-Server**, **Proxmox Virtual Environment**, **Proxmox Backup Server**.
* Vorbereitet (noch auskommentiert): verschiedene Linux-VMs, Raspberry Pis u. a. – noch nicht getestet bzw. noch ohne feste IP.
* **Git-Backup** für openHAB: drei Dateien bzw. Verzeichnisse werden seit Wochen jeden **Sonntag** gesichert – zusätzlich zu den VM-Backups über Proxmox.

---

## Offene Aufgaben

* [ ] Allen vorbereiteten Systemen eine feste IP geben (DHCP-Reservierung)
* [ ] Systeme einzeln testen und im Inventar aktivieren
* [ ] Gruppen und wiederverwendbare Rollen nach den Best Practices strukturieren
* [ ] Weitere Konfigurationen per Git sichern

---

## Hinweise und Risiken

* Best Practices: [Ansible](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/Ansible.md), [DHCP](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/DHCP.md), [Git als Backup](https://github.com/Michdo93/Informatik/blob/main/Backup-Strategien/Git%20als%20Backup.md)

---

