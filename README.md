# 🗂️ Smart-Home-Labor-Backlog

Dieses Repository sammelt alles, was im **Smart Home Labor der Hochschule Furtwangen (HFU)** noch **umgesetzt, getestet, repariert, migriert oder ausprobiert** werden soll – von der Fehlerbehebung in einer Labor-Demo über den Umzug von VMs bis zu Experimenten mit offenem Ausgang.

Es ist bewusst **keine Roadmap mit Terminen**, sondern ein **Backlog**: eine gepflegte, priorisierte Liste offener Vorhaben. Zu jedem Vorhaben gibt es eine eigene Datei mit Ziel, Ist-Stand, offenen Aufgaben, Hinweisen und den zugehörigen Repositories.

<!-- TOC -->
## Inhaltsverzeichnis

- [Wofür ist dieses Repository?](#wofür-ist-dieses-repository)
- [Repository-Übersicht](#repository-übersicht)
- [Legende](#legende)
  - [Status](#status)
  - [Priorität](#priorität)
- [Demos](#demos)
- [Geräteintegration](#geräteintegration)
- [Infrastruktur](#infrastruktur)
- [openHAB](#openhab)
- [Experimente](#experimente)
- [Gute Einstiegsaufgaben](#gute-einstiegsaufgaben)
- [Mitarbeit](#mitarbeit)
  - [Ein Vorhaben übernehmen und abschließen](#ein-vorhaben-übernehmen-und-abschließen)
  - [Ein neues Vorhaben anlegen](#ein-neues-vorhaben-anlegen)
  - [Konventionen](#konventionen)
<!-- /TOC -->

## Wofür ist dieses Repository?

* **Aufgaben finden:** Praktikantinnen und Praktikanten, Hiwis und Studierende sehen hier, woran sie arbeiten können – mit Einschätzung, für wen sich ein Vorhaben eignet.
* **Überblick:** Was ist im Labor offen, was blockiert, was ist fast fertig, was wurde verworfen?
* **Übergabe:** Wer ein Vorhaben übernimmt, findet den aktuellen Stand und die nächsten Schritte, ohne E-Mails durchsuchen zu müssen.
* **Gedächtnis:** Auch verworfene Ansätze und Erkenntnisse bleiben erhalten (z. B. warum ein Weg nicht funktioniert hat).

Rahmenbedingungen und Voraussetzungen für eine Mitarbeit stehen im Repository [Praktika im Smart Home Labor](https://github.com/Michdo93/Praktika-Smart-Home-Labor), das nötige Hintergrundwissen im Kompendium [Informatik](https://github.com/Michdo93/Informatik).

> **Abgrenzung:** Dieses Backlog sammelt konkrete Arbeit am **bestehenden Labor**. Ausgearbeitete Themen für **Abschlussarbeiten** mit Anforderungen und Architekturvorschlag stehen im Repository [SmartHome-Ideen](https://github.com/Michdo93/SmartHome-Ideen). Vorhaben, die hier als „Abschlussarbeit“ markiert sind, können dort zu einer eigenen Idee ausgearbeitet werden.

---

## Repository-Übersicht

Die **[Repository-Übersicht](Repositories.md)** listet alle Repositories rund um das Labor – **integriert**, **mit Nacharbeit**, **noch zu integrieren**, **ungetestet**, **gescheitert** und **deprecated** – mit Beschreibung, Sprache, zugehörigem Vorhaben und Checklisten zum Abhaken.

---

## Legende

### Status

| Status | Bedeutung |
| --- | --- |
| 💡 Idee | Nur eine Idee oder ein Szenario, noch nichts umgesetzt |
| 🧪 Experiment | Erste Ansätze oder Prototypen vorhanden, Ausgang offen |
| 🚧 In Arbeit | Wird umgesetzt, Teile funktionieren bereits |
| 🔍 Test ausstehend | Umgesetzt, muss noch getestet oder abgenommen werden |
| ⛔ Blockiert | Wartet auf etwas (Hardware, Lieferung, Fehlerursache) |
| ✅ Erledigt | Abgeschlossen – bleibt zur Dokumentation erhalten |

### Priorität

| Priorität | Bedeutung |
| --- | --- |
| 🔴 Hoch | Betrifft Labor-Demos oder den laufenden Betrieb |
| 🟠 Mittel | Wichtig für den Ausbau des Labors |
| 🟢 Niedrig | Für zwischendurch, „nice to have“ |

---

## Demos

Labor-Demos und Workshops, die Besuchern gezeigt werden.

| Vorhaben | Status | Priorität | Geeignet für |
| --- | --- | --- | --- |
| [🌅 Morgenroutine](Demos/Morgenroutine.md) | 🚧 In Arbeit | 🔴 Hoch | Labormitarbeitende |
| [🤖 Pepper-Concierge](Demos/Pepper-Concierge.md) | 🚧 In Arbeit | 🔴 Hoch | Labormitarbeitende, Praxissemester |
| [🤳 Pepper-Selfie](Demos/Pepper-Selfie.md) | 🚧 In Arbeit | 🟠 Mittel | Hiwi, Praxissemester |
| [🔐 Smart-Home-Escape-Room-Workshop](Demos/Escape-Room-Workshop.md) | 🚧 In Arbeit | 🟠 Mittel | Labormitarbeitende, Studienprojekt |

---

## Geräteintegration

Geräte, deren Einbindung begonnen hat oder weitgehend fertig ist.

| Vorhaben | Status | Priorität | Geeignet für |
| --- | --- | --- | --- |
| [📽️ BenQ MH856UST (Beamer)](Ger%C3%A4teintegration/BenQ-MH856UST.md) | 🔍 Test ausstehend | 🔴 Hoch | Hiwi |
| [📰 Newspaper Projector](Ger%C3%A4teintegration/Newspaper-Projector.md) | 🚧 In Arbeit | 🔴 Hoch | Hiwi, Praxissemester |
| [📷 PTZ-IP-Kamera PremiumBlue PIPC-011](Ger%C3%A4teintegration/IP-Kamera-PIPC-011.md) | ⛔ Blockiert | 🟠 Mittel | Hiwi |
| [👥 People Counter](Ger%C3%A4teintegration/People-Counter.md) | 🔍 Test ausstehend | 🟠 Mittel | Hiwi, Studienprojekt |
| [📻 Sonos und Webradio](Ger%C3%A4teintegration/Sonos-und-Webradio.md) | 🚧 In Arbeit | 🟠 Mittel | Hiwi |
| [🔔 Doorbird D101 (Türsprechanlage)](Ger%C3%A4teintegration/Doorbird-D101.md) | 🔍 Test ausstehend | 🟢 Niedrig | Hiwi |
| [🎶 Lichtorgel (Sonos + Hue)](Ger%C3%A4teintegration/Music-Light-Organ.md) | 🚧 In Arbeit | 🟢 Niedrig | Hiwi |
| [🔳 QR-Code-Steuerung](Ger%C3%A4teintegration/QR-Code-Steuerung.md) | 🔍 Test ausstehend | 🟢 Niedrig | Hiwi |

---

## Infrastruktur

Server, Proxmox, Docker, Netzwerk, Wartung und Hardware-Installation.

| Vorhaben | Status | Priorität | Geeignet für |
| --- | --- | --- | --- |
| [🐳 Container in der Docker-VM](Infrastruktur/Docker-VM.md) | 🚧 In Arbeit | 🔴 Hoch | Hiwi, Praxissemester |
| [🚚 VMs in Proxmox umziehen](Infrastruktur/Proxmox-VM-Umzug.md) | 🚧 In Arbeit | 🔴 Hoch | Labormitarbeitende, Praxissemester |
| [⚙️ Ansible](Infrastruktur/Ansible.md) | 🚧 In Arbeit | 🟠 Mittel | Hiwi, Praxissemester |
| [☎️ Intercom (Asterisk)](Infrastruktur/Intercom-Asterisk.md) | ⛔ Blockiert | 🟠 Mittel | Hiwi |
| [🧰 Backup- und Wartungsskripte](Infrastruktur/Backups-und-Wartungsskripte.md) | 🔍 Test ausstehend | 🟠 Mittel | Hiwi |
| [🦄 Python-Webanwendungen auf Gunicorn umstellen](Infrastruktur/Gunicorn-Migration.md) | 🚧 In Arbeit | 🟠 Mittel | Hiwi |
| [🔌 Raspberry Pis als USB/IP-Server](Infrastruktur/USB-IP-Server.md) | 🚧 In Arbeit | 🟠 Mittel | Hiwi |
| [📦 VMs in LXC-Container umwandeln](Infrastruktur/Proxmox-VM-zu-LXC.md) | 💡 Idee | 🟠 Mittel | Labormitarbeitende, Praxissemester |
| [📱 Wand-Tablets im Kiosk-Modus](Infrastruktur/Tablets-und-Kiosk.md) | 🚧 In Arbeit | 🟠 Mittel | Hiwi |
| [🖥️ Remote-Zugriff (Guacamole, WOLverine)](Infrastruktur/Remote-Zugriff-Guacamole.md) | 🔍 Test ausstehend | 🟢 Niedrig | Hiwi |
| [📡 MQTT Live Monitor](Infrastruktur/MQTT-Live-Monitor.md) | 🚧 In Arbeit | 🟢 Niedrig | Hiwi |
| [🪟 Windows-Systeme automatisch aktualisieren](Infrastruktur/Windows-Systeme-aktualisieren.md) | 🚧 In Arbeit | 🟢 Niedrig | Hiwi |

---

## openHAB

Konfiguration, Rules, Oberflächen und Erweiterungen von openHAB.

| Vorhaben | Status | Priorität | Geeignet für |
| --- | --- | --- | --- |
| [📜 Migration der Rules](openHAB/Rules-Migration.md) | 🚧 In Arbeit | 🔴 Hoch | Labormitarbeitende, Praxissemester |
| [🖥️ Eigene HTML-Dashboards](openHAB/Dashboards.md) | 🚧 In Arbeit | 🟠 Mittel | Hiwi, Studienprojekt |
| [🏷️ Semantisches Modell und Tags](openHAB/Semantisches-Modell.md) | 🚧 In Arbeit | 🟠 Mittel | Hiwi |
| [🐍 Python-3-Migration älterer openHAB-Projekte](openHAB/Python-3-Migration-Altprojekte.md) | 🚧 In Arbeit | 🟠 Mittel | Hiwi, Praxissemester |
| [🗑️ Abfallkalender](openHAB/Abfallkalender.md) | ⛔ Blockiert | 🟢 Niedrig | Hiwi |
| [🗂️ Things und Items als Textdateien](openHAB/Things-und-Items.md) | 🚧 In Arbeit | 🟢 Niedrig | Hiwi |
| [📅 Google-Bridge (Gmail und Kalender)](openHAB/Google-Bridge.md) | 🚧 In Arbeit | 🟢 Niedrig | Hiwi |
| [🔧 Kleinere Optimierungen](openHAB/Optimierungen.md) | 💡 Idee | 🟢 Niedrig | Hiwi |
| [🔗 ROS 2 und openHAB](openHAB/ROS2-Bridge.md) | 🧪 Experiment | 🟢 Niedrig | Studienprojekt, Abschlussarbeit |
| [🔄 Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md) | 🚧 In Arbeit | 🟢 Niedrig | Hiwi |
| [🧭 Sitemaps und MainUI](openHAB/Sitemaps-und-MainUI.md) | 🚧 In Arbeit | 🟢 Niedrig | Hiwi |

---

## Experimente

Geräte und Ideen, die erst noch erprobt werden.

| Vorhaben | Status | Priorität | Geeignet für |
| --- | --- | --- | --- |
| [📶 ESP32-CSI-Präsenzsensor](Experimente/ESP32-CSI-Sensor.md) | 🧪 Experiment | 🟠 Mittel | Studienprojekt, Abschlussarbeit |
| [🎥 Interaktion mit Kinect-Kameras](Experimente/Kinect-Interaktion.md) | 🧪 Experiment | 🟠 Mittel | Studienprojekt, Abschlussarbeit |
| [☎️ Beschwerde-Hotline](Experimente/Beschwerde-Hotline.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi |
| [🖨️ Brother VC-500W (Etikettendrucker)](Experimente/Brother-VC-500W.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi, Studienprojekt |
| [🗣️ Lokale Sprachassistenten (LIVA, Spracherkennungs-App)](Experimente/Lokale-Sprachassistenten.md) | 🧪 Experiment | 🟢 Niedrig | Studienprojekt, Abschlussarbeit |
| [🏋️ NAO Gym Instructor](Experimente/NAO-Gym-Instructor.md) | 🧪 Experiment | 🟢 Niedrig | Studienprojekt, Abschlussarbeit |
| [🏷️ NFC/RFID](Experimente/NFC-RFID.md) | 🚧 In Arbeit | 🟢 Niedrig | Hiwi, Studienprojekt |
| [🛡️ Smart Home Security Lab](Experimente/Smart-Home-Security-Lab.md) | 🧪 Experiment | 🟢 Niedrig | Studienprojekt, Abschlussarbeit |
| [⚖️ Withings Home Kamera und Personenwaage](Experimente/Withings.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi |
| [🌀 3D Hologram Fan Projector](Experimente/Hologram-Fan-Projector.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi |
| [🚙 7Links Home Security Rover](Experimente/7Links-Home-Security-Rover.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi, Studienprojekt |
| [💡 Beam Labs Beam (Projektor-Lampen)](Experimente/Beam-Labs-Beam.md) | 🧪 Experiment | 🟢 Niedrig | Studienprojekt |
| [📸 ESP32-Cam](Experimente/ESP32-Cam.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi |
| [👋 Gestensteuerung mit ToF-Sensoren](Experimente/ToF-Gestensteuerung.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi, Studienprojekt |
| [📶 IR-USB-HID-Transceiver](Experimente/IR-USB-HID-Transceiver.md) | ⛔ Blockiert | 🟢 Niedrig | Hiwi |
| [📻 Imperial Dabman i250 (Internetradio)](Experimente/Imperial-Dabman-i250.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi |
| [✋ Leap Motion](Experimente/Leap-Motion.md) | 🔍 Test ausstehend | 🟢 Niedrig | Hiwi |
| [🎤 Philips AEA3000/00 (Mikrofone)](Experimente/Philips-AEA3000.md) | 💡 Idee | 🟢 Niedrig | Studienprojekt |
| [📺 Samsung SmartTV](Experimente/Samsung-SmartTV.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi, Studienprojekt |
| [🫖 Smarter SMK20-EU (Wasserkocher)](Experimente/Smarter-SMK20-Wasserkocher.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi |
| [🚪 Türdurchgangszähler (TF-Luna)](Experimente/Door-Traffic-Counter.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi, Studienprojekt |
| [🥽 VR und AR (HoloLens, HTC Vive)](Experimente/VR-AR.md) | 🧪 Experiment | 🟢 Niedrig | Studienprojekt |
| [📡 WebTV](Experimente/WebTV.md) | 🔍 Test ausstehend | 🟢 Niedrig | Hiwi |
| [🎮 Xbox-Controller und Xbox-Konsole](Experimente/Xbox-Steuerung.md) | 🧪 Experiment | 🟢 Niedrig | Hiwi |
| [⚽ adidas miCoach Smart Ball](Experimente/adidas-miCoach-Smart-Ball.md) | 🧪 Experiment | 🟢 Niedrig | Studienprojekt |

---

## Gute Einstiegsaufgaben

Vorhaben, die sich für Hiwis und den Einstieg ins Praxissemester eignen und nicht blockiert sind:

* [🤳 Pepper-Selfie](Demos/Pepper-Selfie.md) – 🚧 In Arbeit
* [📽️ BenQ MH856UST (Beamer)](Ger%C3%A4teintegration/BenQ-MH856UST.md) – 🔍 Test ausstehend
* [📰 Newspaper Projector](Ger%C3%A4teintegration/Newspaper-Projector.md) – 🚧 In Arbeit
* [👥 People Counter](Ger%C3%A4teintegration/People-Counter.md) – 🔍 Test ausstehend
* [📻 Sonos und Webradio](Ger%C3%A4teintegration/Sonos-und-Webradio.md) – 🚧 In Arbeit
* [🔔 Doorbird D101 (Türsprechanlage)](Ger%C3%A4teintegration/Doorbird-D101.md) – 🔍 Test ausstehend
* [🎶 Lichtorgel (Sonos + Hue)](Ger%C3%A4teintegration/Music-Light-Organ.md) – 🚧 In Arbeit
* [🔳 QR-Code-Steuerung](Ger%C3%A4teintegration/QR-Code-Steuerung.md) – 🔍 Test ausstehend
* [🐳 Container in der Docker-VM](Infrastruktur/Docker-VM.md) – 🚧 In Arbeit
* [⚙️ Ansible](Infrastruktur/Ansible.md) – 🚧 In Arbeit
* [🧰 Backup- und Wartungsskripte](Infrastruktur/Backups-und-Wartungsskripte.md) – 🔍 Test ausstehend
* [🦄 Python-Webanwendungen auf Gunicorn umstellen](Infrastruktur/Gunicorn-Migration.md) – 🚧 In Arbeit
* [🔌 Raspberry Pis als USB/IP-Server](Infrastruktur/USB-IP-Server.md) – 🚧 In Arbeit
* [📱 Wand-Tablets im Kiosk-Modus](Infrastruktur/Tablets-und-Kiosk.md) – 🚧 In Arbeit
* [🖥️ Remote-Zugriff (Guacamole, WOLverine)](Infrastruktur/Remote-Zugriff-Guacamole.md) – 🔍 Test ausstehend
* [📡 MQTT Live Monitor](Infrastruktur/MQTT-Live-Monitor.md) – 🚧 In Arbeit
* [🪟 Windows-Systeme automatisch aktualisieren](Infrastruktur/Windows-Systeme-aktualisieren.md) – 🚧 In Arbeit
* [🖥️ Eigene HTML-Dashboards](openHAB/Dashboards.md) – 🚧 In Arbeit
* [🏷️ Semantisches Modell und Tags](openHAB/Semantisches-Modell.md) – 🚧 In Arbeit
* [🐍 Python-3-Migration älterer openHAB-Projekte](openHAB/Python-3-Migration-Altprojekte.md) – 🚧 In Arbeit
* [🗂️ Things und Items als Textdateien](openHAB/Things-und-Items.md) – 🚧 In Arbeit
* [📅 Google-Bridge (Gmail und Kalender)](openHAB/Google-Bridge.md) – 🚧 In Arbeit
* [🔧 Kleinere Optimierungen](openHAB/Optimierungen.md) – 💡 Idee
* [🔄 Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md) – 🚧 In Arbeit
* [🧭 Sitemaps und MainUI](openHAB/Sitemaps-und-MainUI.md) – 🚧 In Arbeit
* [☎️ Beschwerde-Hotline](Experimente/Beschwerde-Hotline.md) – 🧪 Experiment
* [🖨️ Brother VC-500W (Etikettendrucker)](Experimente/Brother-VC-500W.md) – 🧪 Experiment
* [🏷️ NFC/RFID](Experimente/NFC-RFID.md) – 🚧 In Arbeit
* [⚖️ Withings Home Kamera und Personenwaage](Experimente/Withings.md) – 🧪 Experiment
* [🌀 3D Hologram Fan Projector](Experimente/Hologram-Fan-Projector.md) – 🧪 Experiment
* [🚙 7Links Home Security Rover](Experimente/7Links-Home-Security-Rover.md) – 🧪 Experiment
* [📸 ESP32-Cam](Experimente/ESP32-Cam.md) – 🧪 Experiment
* [👋 Gestensteuerung mit ToF-Sensoren](Experimente/ToF-Gestensteuerung.md) – 🧪 Experiment
* [📻 Imperial Dabman i250 (Internetradio)](Experimente/Imperial-Dabman-i250.md) – 🧪 Experiment
* [✋ Leap Motion](Experimente/Leap-Motion.md) – 🔍 Test ausstehend
* [📺 Samsung SmartTV](Experimente/Samsung-SmartTV.md) – 🧪 Experiment
* [🫖 Smarter SMK20-EU (Wasserkocher)](Experimente/Smarter-SMK20-Wasserkocher.md) – 🧪 Experiment
* [🚪 Türdurchgangszähler (TF-Luna)](Experimente/Door-Traffic-Counter.md) – 🧪 Experiment
* [📡 WebTV](Experimente/WebTV.md) – 🔍 Test ausstehend
* [🎮 Xbox-Controller und Xbox-Konsole](Experimente/Xbox-Steuerung.md) – 🧪 Experiment

Besonders gut zum Kennenlernen: **ungetestete Repositories testen** (siehe [Repository-Übersicht](Repositories.md#ungetestet-und-noch-nicht-integriert)) und **deprecated Repositories kennzeichnen und archivieren**.

---

## Mitarbeit

### Ein Vorhaben übernehmen und abschließen

1. Vorhaben auswählen und mit den Labormitarbeitenden abstimmen.
2. Im **Projekt-Repository** arbeiten (Branch, Pull Request); Code gehört nicht in dieses Backlog.
3. Hier im Vorhaben erledigte Aufgaben abhaken (`- [x]`) und Erkenntnisse unter **Ist-Stand** ergänzen.
4. Status und Priorität **in der Datei und in der Tabelle oben** anpassen; bei Repositories auch die [Repository-Übersicht](Repositories.md) aktualisieren.
5. Abgeschlossene Vorhaben nicht löschen, sondern auf ✅ setzen.

### Ein neues Vorhaben anlegen

1. [VORLAGE.md](VORLAGE.md) in den passenden Ordner kopieren und sprechend benennen (`Geräte-Name.md`, keine Leerzeichen).
2. Ziel, Ist-Stand und offene Aufgaben ausfüllen.
3. In der passenden Tabelle oben eintragen.

### Konventionen

* Die Arbeitsweise im Labor (feste IPs, SSH, Zertifikate, MQTT, Ansible, Dokumentation, Web-Server) ist im Kompendium [Informatik](https://github.com/Michdo93/Informatik) unter [Best Practices](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/README.md) beschrieben.
* Keine Passwörter, Tokens oder personenbezogenen Daten in dieses Repository.

---
