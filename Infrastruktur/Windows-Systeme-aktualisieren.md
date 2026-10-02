# 🪟 Windows-Systeme automatisch aktualisieren

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Labor-PCs, Windows-VMs |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Windows-Rechner und -VMs im Labor halten Software, Treiber und System automatisch aktuell.

---

## Ist-Stand

* Ein PowerShell-Werkzeug aktualisiert Software, Treiber und Systemdateien über **winget** und **Get-WindowsUpdate**.
* Es ist vorhanden, muss aber auf einigen Systemen noch **dauerhaft eingerichtet** werden.

---

## Offene Aufgaben

* [ ] Liste der Windows-Systeme erstellen (inkl. der Windows-VM für den People Counter)
* [ ] Auf jedem System als geplante Aufgabe (Aufgabenplanung) einrichten
* [ ] Zeitpunkt so wählen, dass keine Demo oder Lehrveranstaltung betroffen ist
* [ ] Protokollierung prüfen

---

## Repositories

* [Free-Windows-Software-Driver-and-System-Upgrader](https://github.com/Michdo93/Free-Windows-Software-Driver-and-System-Upgrader)

---
