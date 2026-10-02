# 🧰 Backup- und Wartungsskripte

| | |
| --- | --- |
| **Status** | 🔍 Test ausstehend |
| **Priorität** | 🟠 Mittel |
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

Die vorhandenen Backup- und Wartungsskripte laufen zuverlässig, sind dokumentiert und folgen den Best Practices.

---

## Ist-Stand

* Integriert sind u. a.: Bash-Backup-Skripte, ein Skript für manuelle **HomeMatic**-Backups, ein Python-Virenscan-Skript, ein Skript zum Umstellen von Proxmox auf das **No-Subscription-Repository**.
* Einige dieser Repositories sind auf GitHub nicht öffentlich auffindbar (privat oder umbenannt).

---

## Offene Aufgaben

* [ ] Alle Skripte inventarisieren: Wo laufen sie, wann (Cron/systemd-Timer), wohin schreiben sie?
* [ ] HomeMatic-Backup automatisieren statt manuell
* [ ] Prüfen, ob Backups regelmäßig erfolgreich sind und sich **wiederherstellen** lassen
* [ ] Skripte mit ShellCheck prüfen und an den Strict Mode anpassen
* [ ] Sichtbarkeit der Repos klären (öffentlich/privat) und in der Übersicht nachtragen

---

## Hinweise und Risiken

* Grundlagen: [Backup-Strategien](https://github.com/Michdo93/Informatik/blob/main/Backup-Strategien/README.md), [Bash-Skripte](https://github.com/Michdo93/Informatik/blob/main/Linux%20%26%20Werkzeuge/Bash-Skripte.md), [Cron & systemd-Timer](https://github.com/Michdo93/Informatik/blob/main/Linux%20%26%20Werkzeuge/Cron%20%26%20systemd-Timer.md)

---

## Repositories

* [homematic-backup](https://github.com/Michdo93/homematic-backup)
* [proxmox-no-subscription-bash](https://github.com/Michdo93/proxmox-no-subscription-bash)
* [python-homematic-netfinder](https://github.com/Michdo93/python-homematic-netfinder)

---
