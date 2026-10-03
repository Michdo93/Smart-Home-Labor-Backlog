# 🕹️ Anwendungen auf PCs fernsteuern

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Multimedia, Konferenz |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Über openHAB lassen sich Anwendungen auf den Labor-PCs starten, schließen und bedienen (Kodi, Steam/VR, VMs) – per SSH und Fernsteuerwerkzeugen.

---

## Ist-Stand

* Erprobt: Linux-PCs per **sshpass + SSH** steuern (Kodi starten/stoppen, VMs über vmplayer), Windows-PCs per **OpenSSH-Server + PsTools (PsExec)** und **xdotool** für Tastatureingaben.
* Wake-on-LAN zum Einschalten, geregeltes Herunterfahren per `sudo`-Regel (nur bestimmte Befehle).
* Teil des Gesamtbilds mit [WOLverine](Remote-Zugriff-Guacamole.md) und [Multitouchtisch/Vive](../Experimente/Multitouchtisch-Vive.md).

---

## Offene Aufgaben

* [ ] Einheitliches Vorgehen dokumentieren (Linux: SSH-Key statt sshpass-Passwort; Windows: OpenSSH + PsExec)
* [ ] `sudo`-Regeln auf die nötigen Befehle beschränken (poweroff, reboot, killall)
* [ ] Exec-Aufrufe in die Whitelist aufnehmen
* [ ] Wake-on-LAN auf allen Zielrechnern aktivieren und testen

---

## Abhängigkeiten

* [Remote-Zugriff (Guacamole, WOLverine)](Remote-Zugriff-Guacamole.md)

---

## Hinweise und Risiken

* **Sicherheit:** In den alten Notizen stehen Klartext-Passwörter in den Befehlen (sshpass -p, PsExec -p). Das ist zu vermeiden: SSH-Keys, `sshpass -f`/`-e`, Windows-Anmeldung ohne Passwort im Klartext. Siehe [SSH](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/SSH.md) und [Benutzer, Gruppen & Rechte](https://github.com/Michdo93/Informatik/blob/main/Linux%20%26%20Werkzeuge/Benutzer%2C%20Gruppen%20%26%20Rechte.md).
* Grundlagen: [Exec Binding & Remote-Ausführung](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/Exec-Binding%20%26%20Remote-Ausführung.md)

---

