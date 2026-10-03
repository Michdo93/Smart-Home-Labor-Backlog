# 📚 Repository-Übersicht

Alle Repositories rund um das Smart Home Labor auf einen Blick – vom laufenden Betrieb bis zu verworfenen Ansätzen. Jedes Repository ist einem **Vorhaben** in diesem Backlog zugeordnet; dort stehen Ist-Stand, offene Aufgaben und Hintergründe.

Auch **abgeschlossene** und **deprecated** Projekte bleiben bewusst sichtbar: Sie zeigen, was im Labor schon entstanden ist, und sind oft ein guter Ausgangspunkt für eigene Ideen – wer an etwas anknüpfen möchte, findet hier den Einstieg.

<!-- TOC -->
## Inhaltsverzeichnis

- [So arbeitest du mit dieser Übersicht](#so-arbeitest-du-mit-dieser-übersicht)
- [Integriert und in Betrieb](#integriert-und-in-betrieb)
  - [Geräte](#geräte)
  - [openHAB](#openhab)
  - [Bibliotheken](#bibliotheken)
  - [Robotik](#robotik)
  - [Sensorik](#sensorik)
  - [Infrastruktur](#infrastruktur)
  - [Hilfswerkzeuge](#hilfswerkzeuge)
- [Integriert, aber Nacharbeit nötig](#integriert-aber-nacharbeit-nötig)
- [Noch zu integrieren](#noch-zu-integrieren)
- [Ungetestet und noch nicht integriert](#ungetestet-und-noch-nicht-integriert)
- [Nicht zum Laufen gebracht](#nicht-zum-laufen-gebracht)
- [Deprecated und entfernt](#deprecated-und-entfernt)
<!-- /TOC -->

## So arbeitest du mit dieser Übersicht

* **Aufgabe übernehmen:** Ein offener Punkt (☐) in den Checklisten unten oder im verlinkten Vorhaben. Kurz mit den Labormitarbeitenden abstimmen, damit nicht zwei Personen dasselbe tun.
* **Im Projekt-Repository arbeiten:** Code, README und Konfiguration werden **im jeweiligen Repository** angepasst – über einen Branch und einen Pull Request (bzw. direkt, wenn du Schreibrechte hast).
* **Hier abhaken:** Nach Abschluss den Punkt in dieser Datei und im Vorhaben abhaken (`- [x]`), ggf. das Repository in die passende Kategorie verschieben und den Status des Vorhabens anpassen.
* **Erkenntnisse festhalten:** Auch wenn etwas nicht klappt – kurz unter *Ist-Stand* im Vorhaben notieren, warum.

| Kategorie | Anzahl |
| --- | --- |
| Integriert und in Betrieb | 63 |
| Noch zu integrieren | 16 |
| Ungetestet und noch nicht integriert | 31 |
| Nicht zum Laufen gebracht | 2 |
| Deprecated und entfernt | 54 |
| **Gesamt** | **166** |

| Symbol | Bedeutung |
| --- | --- |
| 🔒 | Repository ist öffentlich nicht auffindbar (privat, umbenannt oder gelöscht) – Sichtbarkeit klären |
| ☐ / ☑ | Offen / erledigt |

Stand der Angaben (Sprache, Beschreibung): GitHub, Oktober 2026.

---

## Integriert und in Betrieb

Diese Repositories sind im Labor im Einsatz.

### Geräte

| Repository | Beschreibung | Sprache | Vorhaben |
| --- | --- | --- | --- |
| [openhab-qr-code-scanner-webapp](https://github.com/Michdo93/openhab-qr-code-scanner-webapp) | Web-App: QR-Code mit Group-Item-Namen scannen und Bedienung öffnen | Python | [QR-Code-Steuerung](Ger%C3%A4teintegration/QR-Code-Steuerung.md) |
| [newspaperprojector](https://github.com/Michdo93/newspaperprojector) | Projektor (BeagleBone Black + DLPDLCR2000EVM) zeigt täglich die aktuelle Zeitung | HTML | [Newspaper Projector](Ger%C3%A4teintegration/Newspaper-Projector.md) |
| [newspaperprojector-gesture-control](https://github.com/Michdo93/newspaperprojector-gesture-control) | Gestensteuerung des Newspaper Projectors mit Kinect und Raspberry Pi | Python | [Newspaper Projector](Ger%C3%A4teintegration/Newspaper-Projector.md) |
| [PremiumBlue-PIPC-011-Python](https://github.com/Michdo93/PremiumBlue-PIPC-011-Python) | Python-Steuerung der PTZ-IP-Kamera PremiumBlue PIPC-011 | Python | [PTZ-IP-Kamera PremiumBlue PIPC-011](Ger%C3%A4teintegration/IP-Kamera-PIPC-011.md) |
| [webtv-openhab](https://github.com/Michdo93/webtv-openhab) | HTML5-Dashboard für WebTV (REST API + SSE) | JavaScript | [WebTV](Experimente/WebTV.md) |
| [people-counter](https://github.com/Michdo93/people-counter) | Personenzähler mit ASUS Xtion Pro | Python | [People Counter](Ger%C3%A4teintegration/People-Counter.md) |
| [webradio-openhab](https://github.com/Michdo93/webradio-openhab) | HTML-Dashboard für Webradio inkl. Items und Python-3-Rules | JavaScript | [Sonos und Webradio](Ger%C3%A4teintegration/Sonos-und-Webradio.md) |
| [BenQ-RS232-TCP](https://github.com/Michdo93/BenQ-RS232-TCP) | Steuerung des BenQ-Beamers per RS232 über TCP (LAN) | Python | [BenQ MH856UST (Beamer)](Ger%C3%A4teintegration/BenQ-MH856UST.md) |
| [Labor-Smart-Home-Konferenz-Kamera](https://github.com/Michdo93/Labor-Smart-Home-Konferenz-Kamera) | Konferenzkamera und -lautsprecher automatisch per USB/IP einbinden | Shell | [Raspberry Pis als USB/IP-Server](Infrastruktur/USB-IP-Server.md) |
| [Somfy-TaHoma-Developer-Mode-Postman-Collection](https://github.com/Michdo93/Somfy-TaHoma-Developer-Mode-Postman-Collection) | Postman-Collection für die lokale API von Somfy-TaHoma-Gateways | – | [Somfy TaHoma (lokale API)](Ger%C3%A4teintegration/Somfy-TaHoma.md) |

### openHAB

| Repository | Beschreibung | Sprache | Vorhaben |
| --- | --- | --- | --- |
| [openhab-design-patterns-examples](https://github.com/Michdo93/openhab-design-patterns-examples) | Beispiele der openHAB Design Patterns (Rules DSL, JavaScript, Python 3) | Python | [Migration der Rules](openHAB/Rules-Migration.md) |
| [openhab-things-exporter](https://github.com/Michdo93/openhab-things-exporter) | Exportiert openHAB-Things in `.things`-Dateien | Python | [Things und Items als Textdateien](openHAB/Things-und-Items.md) |
| [openhab-semantic-tags](https://github.com/Michdo93/openhab-semantic-tags) | Liste der semantischen Tags von openHAB 5 | – | [Semantisches Modell und Tags](openHAB/Semantisches-Modell.md) |
| [openhab-semantic-model-viewer](https://github.com/Michdo93/openhab-semantic-model-viewer) | Viewer für das semantische Modell | Python | [Semantisches Modell und Tags](openHAB/Semantisches-Modell.md) |
| [oh-ai-bridge](https://github.com/Michdo93/oh-ai-bridge) | Middleware: openHAB als Endpunkt für Open WebUI (semantisches Modell + TF-IDF) | Python | [Semantisches Modell und Tags](openHAB/Semantisches-Modell.md) |
| [openHAB5-Test](https://github.com/Michdo93/openHAB5-Test) | Tests mit openHAB 5 und GraalPy | – | [Migration der Rules](openHAB/Rules-Migration.md) |
| [HABApp-MQTT-Event-Bus](https://github.com/Michdo93/HABApp-MQTT-Event-Bus) | MQTT-Event-Bus für openHAB mit HABApp | Python | [Python-3-Migration älterer openHAB-Projekte](openHAB/Python-3-Migration-Altprojekte.md) |
| [openHABSpeechRecognizer](https://github.com/Michdo93/openHABSpeechRecognizer) | Android-App: erkannter Text → STT-Puffer-Item | Java | [Lokale Sprachassistenten (LIVA, Spracherkennungs-App)](Experimente/Lokale-Sprachassistenten.md) |
| [openhab_static_examples](https://github.com/Michdo93/openhab_static_examples) | Statische Beispiel-Items für jeden Item-Typ | HTML | [Weitere Hilfswerkzeuge](openHAB/Hilfswerkzeuge.md) |
| [openhab_postman_templates](https://github.com/Michdo93/openhab_postman_templates) | Postman-Collections für die REST API von openHAB und openHAB Cloud | – | [Weitere Hilfswerkzeuge](openHAB/Hilfswerkzeuge.md) |
| [openHAB-Alexa-Sound-Library](https://github.com/Michdo93/openHAB-Alexa-Sound-Library) | Alexa Skills Kit Sound Library über das Amazon Echo Control Binding | – | [Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md) |
| [openHAB-Alexa-Speechcons](https://github.com/Michdo93/openHAB-Alexa-Speechcons) | Deutsche Speechcons über das Amazon Echo Control Binding | – | [Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md) |
| [openHAB-Alexa-SSML](https://github.com/Michdo93/openHAB-Alexa-SSML) | Deutsche SSML-Beispiele über das Amazon Echo Control Binding | – | [Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md) |
| [openHAB-tagesschau-feed](https://github.com/Michdo93/openHAB-tagesschau-feed) | Tagesschau-Newsfeed über das Feed Binding | – | [Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md) |
| [openHAB-virtual-alarm-clock](https://github.com/Michdo93/openHAB-virtual-alarm-clock) | Virtueller Wecker mit openHAB | – | [Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md) |

### Bibliotheken

| Repository | Beschreibung | Sprache | Vorhaben |
| --- | --- | --- | --- |
| [android-openhab-test-suite](https://github.com/Michdo93/android-openhab-test-suite) | openHAB Test Suite (Android/Kotlin) | Kotlin | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [c-openhab-test-suite](https://github.com/Michdo93/c-openhab-test-suite) | openHAB Test Suite (C) | C | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [cpp-openhab-test-suite](https://github.com/Michdo93/cpp-openhab-test-suite) | openHAB Test Suite (C++) | C++ | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [csharp-openhab-test-suite](https://github.com/Michdo93/csharp-openhab-test-suite) | openHAB Test Suite (C#) | C# | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [nodejs-openhab-test-suite](https://github.com/Michdo93/nodejs-openhab-test-suite) | openHAB Test Suite (Node.js) | JavaScript | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [js-openhab-test-suite](https://github.com/Michdo93/js-openhab-test-suite) | openHAB Test Suite (JavaScript) | HTML | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [java-openhab-test-suite](https://github.com/Michdo93/java-openhab-test-suite) | openHAB Test Suite (Java) | Java | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [openhab-test-suite](https://github.com/Michdo93/openhab-test-suite) | Testbibliothek zum Prüfen von openHAB-Installationen (Python) | Python | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [android-openhab-rest-client](https://github.com/Michdo93/android-openhab-rest-client) | REST-Client für openHAB (Android/Kotlin) | Kotlin | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [c-openhab-rest-client](https://github.com/Michdo93/c-openhab-rest-client) | REST-Client für openHAB (C) | C | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [js-openhab-rest-client](https://github.com/Michdo93/js-openhab-rest-client) | REST-Client für openHAB (JavaScript, Browser) | HTML | [Eigene HTML-Dashboards](openHAB/Dashboards.md) |
| [nodejs-openhab-rest-client](https://github.com/Michdo93/nodejs-openhab-rest-client) | REST-Client für openHAB (Node.js) | JavaScript | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [java-openhab-rest-client](https://github.com/Michdo93/java-openhab-rest-client) | REST-Client für openHAB (Java) | Java | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [cpp-openhab-rest-client](https://github.com/Michdo93/cpp-openhab-rest-client) | REST-Client für openHAB (C++) | C++ | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [csharp-openhab-rest-client](https://github.com/Michdo93/csharp-openhab-rest-client) | REST-Client für openHAB (C#) | C# | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |
| [python-openhab-rest-client](https://github.com/Michdo93/python-openhab-rest-client) | REST-Client für openHAB (Python) | Python | [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md) |

### Robotik

| Repository | Beschreibung | Sprache | Vorhaben |
| --- | --- | --- | --- |
| [ros2-browser-client](https://github.com/Michdo93/ros2-browser-client) | Browserbasierter Fernsteuerungs- und Diagnose-Client für ROS 2 | JavaScript | [ROS 2 und openHAB](openHAB/ROS2-Bridge.md) |
| [ros1-browser-client](https://github.com/Michdo93/ros1-browser-client) | Browserbasierter Fernsteuerungs- und Diagnose-Client für ROS 1 | JavaScript | [ROS 2 und openHAB](openHAB/ROS2-Bridge.md) |
| [Pepper-Concierge-Python](https://github.com/Michdo93/Pepper-Concierge-Python) | Pepper stellt das Smart Home Labor vor (NAOqi 2.5, Python 2.7) | Python | [Pepper-Concierge](Demos/Pepper-Concierge.md) |
| [PepperSelfie](https://github.com/Michdo93/PepperSelfie) | Pepper-Fotoanwendung (Java, NAOqi 2.5) | Java | [Pepper-Selfie](Demos/Pepper-Selfie.md) |
| [leap_control](https://github.com/Michdo93/leap_control) | ROS-2-Node: Roboter mit Ultraleap per `cmd_vel` steuern | Python | [Leap Motion](Experimente/Leap-Motion.md) |
| [Pepper_ConciergeShortSSH](https://github.com/Michdo93/Pepper_ConciergeShortSSH) | Kurzvariante des Concierge über SSH (Java) | Java | [Pepper-Concierge](Demos/Pepper-Concierge.md) |

### Sensorik

| Repository | Beschreibung | Sprache | Vorhaben |
| --- | --- | --- | --- |
| [esp32-csi-heatmap](https://github.com/Michdo93/esp32-csi-heatmap) | Echtzeit-Visualisierung von WLAN-CSI am ESP32 (Heatmap, Präsenzerkennung) | Python | [ESP32-CSI-Präsenzsensor](Experimente/ESP32-CSI-Sensor.md) |

### Infrastruktur

| Repository | Beschreibung | Sprache | Vorhaben |
| --- | --- | --- | --- |
| [ubuntu-tablet-kiosk-mode-installer](https://github.com/Michdo93/ubuntu-tablet-kiosk-mode-installer) | Kiosk-Modus mit Chromium auf Linux-Tablets einrichten | Shell | [Wand-Tablets im Kiosk-Modus](Infrastruktur/Tablets-und-Kiosk.md) |
| [asterisk-smarthome](https://github.com/Michdo93/asterisk-smarthome) | Asterisk-Telefonanlage für das Smart Home (Ubuntu Server auf Proxmox, Piper TTS, Python-Dienst) | Python | [Intercom (Asterisk)](Infrastruktur/Intercom-Asterisk.md) |
| `kiosk-launcher` 🔒 | Kiosk-Launcher | – | [Wand-Tablets im Kiosk-Modus](Infrastruktur/Tablets-und-Kiosk.md) |
| [Apache-Guacamole-1.6.0-Ubuntu-24.04-Install-Script](https://github.com/Michdo93/Apache-Guacamole-1.6.0-Ubuntu-24.04-Install-Script) | Installationsskript für Apache Guacamole 1.6.0 | Shell | [Remote-Zugriff (Guacamole, WOLverine)](Infrastruktur/Remote-Zugriff-Guacamole.md) |
| [USBIP-Configuration](https://github.com/Michdo93/USBIP-Configuration) | Anleitung: USB/IP-Client und -Server konfigurieren | – | [Raspberry Pis als USB/IP-Server](Infrastruktur/USB-IP-Server.md) |
| [Free-Windows-Software-Driver-and-System-Upgrader](https://github.com/Michdo93/Free-Windows-Software-Driver-and-System-Upgrader) | Windows-Software, Treiber und System per winget/Get-WindowsUpdate aktualisieren | PowerShell | [Windows-Systeme automatisch aktualisieren](Infrastruktur/Windows-Systeme-aktualisieren.md) |
| [python-homematic-netfinder](https://github.com/Michdo93/python-homematic-netfinder) | HomeMatic-Netfinder in Python: IP-Adressen von HomeMatic-Zentralen finden | Python | [Backup- und Wartungsskripte](Infrastruktur/Backups-und-Wartungsskripte.md) |
| [homematic-backup](https://github.com/Michdo93/homematic-backup) | HomeMatic-Backup per Shell-Skript (manuell) | Shell | [Backup- und Wartungsskripte](Infrastruktur/Backups-und-Wartungsskripte.md) |
| `bash-backup-scripts` 🔒 | Bash-Backup-Skripte | – | [Backup- und Wartungsskripte](Infrastruktur/Backups-und-Wartungsskripte.md) |
| `python-virus-scan-script` 🔒 | Python-Virenscan-Skript | – | [Backup- und Wartungsskripte](Infrastruktur/Backups-und-Wartungsskripte.md) |
| [proxmox-no-subscription-bash](https://github.com/Michdo93/proxmox-no-subscription-bash) | Proxmox auf das No-Subscription-Repository umstellen | Shell | [Backup- und Wartungsskripte](Infrastruktur/Backups-und-Wartungsskripte.md) |

### Hilfswerkzeuge

| Repository | Beschreibung | Sprache | Vorhaben |
| --- | --- | --- | --- |
| [IEEE-BibTeX-Formatter-JS](https://github.com/Michdo93/IEEE-BibTeX-Formatter-JS) | Zitate im IEEE-Stil aus BibTeX formatieren (JavaScript) | JavaScript | [Weitere Hilfswerkzeuge](openHAB/Hilfswerkzeuge.md) |
| [python-swfr-menu-plan-xml-interface](https://github.com/Michdo93/python-swfr-menu-plan-xml-interface) | Zugriff auf die XML-Schnittstelle des SWFR-Speiseplans | Python | [Weitere Hilfswerkzeuge](openHAB/Hilfswerkzeuge.md) |
| [qr2pdf](https://github.com/Michdo93/qr2pdf) | Mehrere QR-Codes in eine druckbare PDF einfügen | Python | [QR-Code-Steuerung](Ger%C3%A4teintegration/QR-Code-Steuerung.md) |
| [QR-Code-Generator](https://github.com/Michdo93/QR-Code-Generator) | QR-Codes erzeugen und als Bild speichern | Python | [QR-Code-Steuerung](Ger%C3%A4teintegration/QR-Code-Steuerung.md) |

> Die **REST-Clients** und **Test Suites** gibt es für acht Sprachen (Vorhaben: [openHAB REST-Clients und Test Suites](openHAB/REST-Clients-und-Test-Suites.md)).

---

## Integriert, aber Nacharbeit nötig

* [ ] [newspaperprojector-gesture-control](https://github.com/Michdo93/newspaperprojector-gesture-control) – Gestenerkennung noch zu testen → [Newspaper Projector](Ger%C3%A4teintegration/Newspaper-Projector.md)
* [ ] [PremiumBlue-PIPC-011-Python](https://github.com/Michdo93/PremiumBlue-PIPC-011-Python) – Absturz nach Neustart → [PTZ-IP-Kamera PremiumBlue PIPC-011](Ger%C3%A4teintegration/IP-Kamera-PIPC-011.md)
* [ ] [people-counter](https://github.com/Michdo93/people-counter) – Zählgenauigkeit → [People Counter](Ger%C3%A4teintegration/People-Counter.md)
* [ ] [openhab-things-exporter](https://github.com/Michdo93/openhab-things-exporter) – Bekannte Exportfehler → [Things und Items als Textdateien](openHAB/Things-und-Items.md)
* [ ] [Pepper-Concierge-Python](https://github.com/Michdo93/Pepper-Concierge-Python) – muss refactort werden → [Pepper-Concierge](Demos/Pepper-Concierge.md)
* [ ] [PepperSelfie](https://github.com/Michdo93/PepperSelfie) – muss refactort werden → [Pepper-Selfie](Demos/Pepper-Selfie.md)
* [ ] `kiosk-launcher` 🔒 – muss refactort werden → [Wand-Tablets im Kiosk-Modus](Infrastruktur/Tablets-und-Kiosk.md)
* [ ] [Apache-Guacamole-1.6.0-Ubuntu-24.04-Install-Script](https://github.com/Michdo93/Apache-Guacamole-1.6.0-Ubuntu-24.04-Install-Script) – Beschreibung nennt Ubuntu 20.04 → [Remote-Zugriff (Guacamole, WOLverine)](Infrastruktur/Remote-Zugriff-Guacamole.md)
* [ ] [Free-Windows-Software-Driver-and-System-Upgrader](https://github.com/Michdo93/Free-Windows-Software-Driver-and-System-Upgrader) – muss bei einigen Systemen dauerhaft eingerichtet werden → [Windows-Systeme automatisch aktualisieren](Infrastruktur/Windows-Systeme-aktualisieren.md)
* [ ] [HABApp-MQTT-Event-Bus](https://github.com/Michdo93/HABApp-MQTT-Event-Bus) – muss vermutlich geupgradet werden → [Python-3-Migration älterer openHAB-Projekte](openHAB/Python-3-Migration-Altprojekte.md)
* [ ] [homematic-backup](https://github.com/Michdo93/homematic-backup) – Automatisieren → [Backup- und Wartungsskripte](Infrastruktur/Backups-und-Wartungsskripte.md)
* [ ] `bash-backup-scripts` 🔒 – Öffentlich nicht auffindbar → [Backup- und Wartungsskripte](Infrastruktur/Backups-und-Wartungsskripte.md)
* [ ] `python-virus-scan-script` 🔒 – Öffentlich nicht auffindbar → [Backup- und Wartungsskripte](Infrastruktur/Backups-und-Wartungsskripte.md)
* [ ] [Pepper_ConciergeShortSSH](https://github.com/Michdo93/Pepper_ConciergeShortSSH) – muss refactort werden → [Pepper-Concierge](Demos/Pepper-Concierge.md)
* [ ] [openHAB-Alexa-Sound-Library](https://github.com/Michdo93/openHAB-Alexa-Sound-Library) – bereits migriert, Repo nicht aktuell → [Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md)
* [ ] [openHAB-Alexa-Speechcons](https://github.com/Michdo93/openHAB-Alexa-Speechcons) – bereits migriert, Repo nicht aktuell → [Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md)
* [ ] [openHAB-Alexa-SSML](https://github.com/Michdo93/openHAB-Alexa-SSML) – bereits migriert, Repo nicht aktuell → [Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md)
* [ ] [openHAB-tagesschau-feed](https://github.com/Michdo93/openHAB-tagesschau-feed) – bereits migriert, Repo nicht aktuell → [Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md)
* [ ] [openHAB-virtual-alarm-clock](https://github.com/Michdo93/openHAB-virtual-alarm-clock) – bereits migriert, Repo nicht aktuell → [Repositories bereits migrierter Projekte aktualisieren](openHAB/Repos-migrierter-Projekte-aktualisieren.md)

---

## Noch zu integrieren

Code ist vorhanden und (weitgehend) lauffähig, aber noch nicht dauerhaft im Labor in Betrieb.

| Repository | Beschreibung | Sprache | Vorhaben | Hinweis |
| --- | --- | --- | --- | --- |
| [openhab-google-bridge](https://github.com/Michdo93/openhab-google-bridge) | Gmail- und Google-Kalender-Anbindung | Python | [Google-Bridge (Gmail und Kalender)](openHAB/Google-Bridge.md) | – |
| [xbox-360-openhab-controller](https://github.com/Michdo93/xbox-360-openhab-controller) | openHAB mit einem Xbox-360-Controller bedienen | Python | [Xbox-Controller und Xbox-Konsole](Experimente/Xbox-Steuerung.md) | unklar, welcher Code am Ende der richtige war |
| [Leap-Motion-Examples](https://github.com/Michdo93/Leap-Motion-Examples) | Leap-Motion-Beispiele | Python | [Leap Motion](Experimente/Leap-Motion.md) | unklar, welche Codes am Ende korrekt waren |
| [hologram-fan-projector](https://github.com/Michdo93/hologram-fan-projector) | Werkzeuge für den Hologram Fan Projector (Steuerung, MP4 → BIN) | Python | [3D Hologram Fan Projector](Experimente/Hologram-Fan-Projector.md) | – |
| [ESP32-Cam-Viewer](https://github.com/Michdo93/ESP32-Cam-Viewer) | ESP32-Cam-Stream anzeigen | Python | [ESP32-Cam](Experimente/ESP32-Cam.md) | – |
| [liva-jetson-ai](https://github.com/Michdo93/liva-jetson-ai) | Fork: Sprachassistent für Jetson | Python | [Lokale Sprachassistenten (LIVA, Spracherkennungs-App)](Experimente/Lokale-Sprachassistenten.md) | Inhalt sichten |
| [liva-raspberry-va](https://github.com/Michdo93/liva-raspberry-va) | Fork: Sprachassistent für Raspberry Pi | Python | [Lokale Sprachassistenten (LIVA, Spracherkennungs-App)](Experimente/Lokale-Sprachassistenten.md) | Inhalt sichten |
| [WSGI-Server](https://github.com/Michdo93/WSGI-Server) | Anleitung: WSGI-Server für Python-Anwendungen einrichten | – | [Python-Webanwendungen auf Gunicorn umstellen](Infrastruktur/Gunicorn-Migration.md) | das meiste läuft noch unter python3 statt Gunicorn |
| [ControlX](https://github.com/Michdo93/ControlX) | Ohne Beschreibung (HTML) | HTML | [Repositories ohne Beschreibung sichten](Experimente/Unklare-Repositories-sichten.md) | Inhalt sichten |
| [WOLverine](https://github.com/Michdo93/WOLverine) | Flask-Dashboard: Rechner per Wake-on-LAN schalten und überwachen | Python | [Remote-Zugriff (Guacamole, WOLverine)](Infrastruktur/Remote-Zugriff-Guacamole.md) | – |
| [MQTT-Live-Monitor](https://github.com/Michdo93/MQTT-Live-Monitor) | Live-Anzeige von MQTT-Topics und -Nachrichten im Browser | HTML | [MQTT Live Monitor](Infrastruktur/MQTT-Live-Monitor.md) | – |
| [Smart-Home-Escape-Room-Workshop](https://github.com/Michdo93/Smart-Home-Escape-Room-Workshop) | Workshop-Modell mit Node-RED im Smart Home Labor (Fork) | Python | [Smart-Home-Escape-Room-Workshop](Demos/Escape-Room-Workshop.md) | – |
| `GestureControl` 🔒 | Gestensteuerung | – | [Gestensteuerung mit ToF-Sensoren](Experimente/ToF-Gestensteuerung.md) | Öffentlich nicht auffindbar |
| [waste-calendar-downloader](https://github.com/Michdo93/waste-calendar-downloader) | Abfallkalender der HFU per Selenium herunterladen | Python | [Abfallkalender](openHAB/Abfallkalender.md) | muss refactort werden, lief zuletzt nicht mehr |
| [openHAB-Music-Light-Organ](https://github.com/Michdo93/openHAB-Music-Light-Organ) | Lichtorgel: Hue-Lampen folgen der Sonos-Wiedergabe | Python | [Lichtorgel (Sonos + Hue)](Ger%C3%A4teintegration/Music-Light-Organ.md) | – |
| [openHAB-VoiceRSS-Sonos](https://github.com/Michdo93/openHAB-VoiceRSS-Sonos) | Sprachausgabe über VoiceRSS auf Sonos | – | [Python-3-Migration älterer openHAB-Projekte](openHAB/Python-3-Migration-Altprojekte.md) | muss auf Python 3 migriert werden |

**Aufgaben:**

* [ ] [openhab-google-bridge](https://github.com/Michdo93/openhab-google-bridge) integrieren
* [ ] [xbox-360-openhab-controller](https://github.com/Michdo93/xbox-360-openhab-controller) integrieren
* [ ] [Leap-Motion-Examples](https://github.com/Michdo93/Leap-Motion-Examples) integrieren
* [ ] [hologram-fan-projector](https://github.com/Michdo93/hologram-fan-projector) integrieren
* [ ] [ESP32-Cam-Viewer](https://github.com/Michdo93/ESP32-Cam-Viewer) integrieren
* [ ] [liva-jetson-ai](https://github.com/Michdo93/liva-jetson-ai) integrieren
* [ ] [liva-raspberry-va](https://github.com/Michdo93/liva-raspberry-va) integrieren
* [ ] [WSGI-Server](https://github.com/Michdo93/WSGI-Server) integrieren
* [ ] [ControlX](https://github.com/Michdo93/ControlX) integrieren
* [ ] [WOLverine](https://github.com/Michdo93/WOLverine) integrieren
* [ ] [MQTT-Live-Monitor](https://github.com/Michdo93/MQTT-Live-Monitor) integrieren
* [ ] [Smart-Home-Escape-Room-Workshop](https://github.com/Michdo93/Smart-Home-Escape-Room-Workshop) integrieren
* [ ] `GestureControl` 🔒 integrieren
* [ ] [waste-calendar-downloader](https://github.com/Michdo93/waste-calendar-downloader) integrieren
* [ ] [openHAB-Music-Light-Organ](https://github.com/Michdo93/openHAB-Music-Light-Organ) integrieren
* [ ] [openHAB-VoiceRSS-Sonos](https://github.com/Michdo93/openHAB-VoiceRSS-Sonos) integrieren

---

## Ungetestet und noch nicht integriert

Code liegt vor, wurde aber noch nicht (vollständig) getestet. Gute Aufgaben zum Einstieg: testen, dokumentieren, Ergebnis im Vorhaben festhalten.

| Repository | Beschreibung | Sprache | Vorhaben | Hinweis |
| --- | --- | --- | --- | --- |
| [vl53l1x-gesture-toolkit](https://github.com/Michdo93/vl53l1x-gesture-toolkit) | Gestensteuerung mit einem VL53L1X-ToF-Sensor (ESP32, Arduino, RP2040) | C++ | [Gestensteuerung mit ToF-Sensoren](Experimente/ToF-Gestensteuerung.md) | – |
| [door-traffic-counter](https://github.com/Michdo93/door-traffic-counter) | Richtungs-Türzähler mit ESP32 und zwei TF-Luna-LiDAR, per MQTT an openHAB | C++ | [Türdurchgangszähler (TF-Luna)](Experimente/Door-Traffic-Counter.md) | – |
| [vl53l5cx_gesture_experiments](https://github.com/Michdo93/vl53l5cx_gesture_experiments) | Gestenerkennung mit dem VL53L5CX (Python) | Python | [Gestensteuerung mit ToF-Sensoren](Experimente/ToF-Gestensteuerung.md) | – |
| [Nao-Gym-Instructor](https://github.com/Michdo93/Nao-Gym-Instructor) | NAO Gym Instructor: Portierung auf Raspberry Pi mit Kinect V1 | Python | [NAO Gym Instructor](Experimente/NAO-Gym-Instructor.md) | – |
| [openhab-sheets-rules](https://github.com/Michdo93/openhab-sheets-rules) | Ohne Beschreibung (Python) | Python | [Repositories ohne Beschreibung sichten](Experimente/Unklare-Repositories-sichten.md) | Inhalt sichten |
| [pepper_ros2_ws](https://github.com/Michdo93/pepper_ros2_ws) | ROS-2-Workspace für Pepper | Python | [Pepper-Concierge](Demos/Pepper-Concierge.md) | – |
| [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | ROS-2-Workspace für die openHAB-Anbindung | Python | [ROS 2 und openHAB](openHAB/ROS2-Bridge.md) | – |
| [Smart-Home-Security-Lab](https://github.com/Michdo93/Smart-Home-Security-Lab) | Smart Home Security Lab | HTML | [Smart Home Security Lab](Experimente/Smart-Home-Security-Lab.md) | Inhalt sichten |
| [therenect-linux](https://github.com/Michdo93/therenect-linux) | Virtuelles Theremin für die Kinect V1 (Linux-Portierung, GPL) | C++ | [Interaktion mit Kinect-Kameras](Experimente/Kinect-Interaktion.md) | – |
| [NFC-RFID-Examples](https://github.com/Michdo93/NFC-RFID-Examples) | NFC/RFID-Beispiele | Python | [NFC/RFID](Experimente/NFC-RFID.md) | – |
| [invisible-spatial-switch](https://github.com/Michdo93/invisible-spatial-switch) | Unsichtbare Touch-Flächen an Wänden mit Kinect V1 | Python | [Interaktion mit Kinect-Kameras](Experimente/Kinect-Interaktion.md) | – |
| [samsungtv](https://github.com/Michdo93/samsungtv) | Python-Steuerung für Samsung-SmartTVs | Python | [Samsung SmartTV](Experimente/Samsung-SmartTV.md) | – |
| [interactive-projector](https://github.com/Michdo93/interactive-projector) | Interaktive Projektion mit Kinect V2 | Python | [Interaktion mit Kinect-Kameras](Experimente/Kinect-Interaktion.md) | – |
| [Brother-VC-500W](https://github.com/Michdo93/Brother-VC-500W) | Etikettendrucker Brother VC-500W abfragen und ansteuern | Python | [Brother VC-500W (Etikettendrucker)](Experimente/Brother-VC-500W.md) | – |
| [complaints-hotline](https://github.com/Michdo93/complaints-hotline) | Beschwerde-Hotline mit Aufnahme und Stimmverzerrer | Python | [Beschwerde-Hotline](Experimente/Beschwerde-Hotline.md) | – |
| [adidas-miCoach-Smart-Ball-Python](https://github.com/Michdo93/adidas-miCoach-Smart-Ball-Python) | Sensordaten des adidas miCoach Smart Ball per Bluetooth | Python | [adidas miCoach Smart Ball](Experimente/adidas-miCoach-Smart-Ball.md) | – |
| [Philips-AEA3000-00-Noise-Guard](https://github.com/Michdo93/Philips-AEA3000-00-Noise-Guard) | Lautstärkeüberwachung mit Philips-AEA3000-Mikrofonen | Python | [Philips AEA3000/00 (Mikrofone)](Experimente/Philips-AEA3000.md) | – |
| [beamctl](https://github.com/Michdo93/beamctl) | Beam Labs Beam ohne Original-App steuern | Python | [Beam Labs Beam (Projektor-Lampen)](Experimente/Beam-Labs-Beam.md) | – |
| [Smarter-SMK20-EU](https://github.com/Michdo93/Smarter-SMK20-EU) | Smarter Wasserkocher SMK20-EU ansteuern | Python | [Smarter SMK20-EU (Wasserkocher)](Experimente/Smarter-SMK20-Wasserkocher.md) | – |
| [7Links-Home-Security-Rover-Controller](https://github.com/Michdo93/7Links-Home-Security-Rover-Controller) | Steuerung des 7Links Home Security Rover | Python | [7Links Home Security Rover](Experimente/7Links-Home-Security-Rover.md) | – |
| `smart-farm-house` 🔒 | Smart Farm House | – | [Repositories ohne Beschreibung sichten](Experimente/Unklare-Repositories-sichten.md) | Öffentlich nicht auffindbar |
| [arlo-cam-tests](https://github.com/Michdo93/arlo-cam-tests) | Tests mit Arlo-Kameras | – | [Smart Home Security Lab](Experimente/Smart-Home-Security-Lab.md) | – |
| [esp32-csi-presence-sensor](https://github.com/Michdo93/esp32-csi-presence-sensor) | WLAN-CSI-Präsenzsensor mit dem ESP32 | Python | [ESP32-CSI-Präsenzsensor](Experimente/ESP32-CSI-Sensor.md) | – |
| [hololens-viewer](https://github.com/Michdo93/hololens-viewer) | HoloLens-Viewer (JavaScript) | JavaScript | [VR und AR (HoloLens, HTC Vive)](Experimente/VR-AR.md) | – |
| [ESP32-Realtime-System](https://github.com/Michdo93/ESP32-Realtime-System) | Fork: Echtzeit-Wi-Fi-Sensing-Demo | Python | [ESP32-CSI-Präsenzsensor](Experimente/ESP32-CSI-Sensor.md) | – |
| [ir-usb-hid-transreceiver](https://github.com/Michdo93/ir-usb-hid-transreceiver) | DIY-USB-IR-Transceiver, meldet sich als Tastatur an | Python | [IR-USB-HID-Transceiver](Experimente/IR-USB-HID-Transceiver.md) | gelötet und verkabelt, noch nicht geflasht (kein passendes USB-Datenkabel) |
| [openHAB-Application-Checker](https://github.com/Michdo93/openHAB-Application-Checker) | Prüft per Exec Action, ob eine Anwendung läuft | – | [Python-3-Migration älterer openHAB-Projekte](openHAB/Python-3-Migration-Altprojekte.md) | muss zu Python 3 migriert werden |
| [openHAB-RuleManager](https://github.com/Michdo93/openHAB-RuleManager) | Verwaltung von Rules | – | [Python-3-Migration älterer openHAB-Projekte](openHAB/Python-3-Migration-Altprojekte.md) | muss zu Python 3 migriert werden |
| [status-openhab-org](https://github.com/Michdo93/status-openhab-org) | Status von status.openhab.org als Items | Python | [Python-3-Migration älterer openHAB-Projekte](openHAB/Python-3-Migration-Altprojekte.md) | muss zu Python 3 migriert werden |
| [openHAB-Steam-HTC-Vive](https://github.com/Michdo93/openHAB-Steam-HTC-Vive) | Steam/HTC-Vive-Anwendungen auf entferntem Windows-PC starten | – | [VR und AR (HoloLens, HTC Vive)](Experimente/VR-AR.md) | – |
| [openHAB-xbox-remote-power](https://github.com/Michdo93/openHAB-xbox-remote-power) | Xbox One per Exec Binding ein-/ausschalten | – | [Xbox-Controller und Xbox-Konsole](Experimente/Xbox-Steuerung.md) | – |

**Aufgaben:**

* [ ] [vl53l1x-gesture-toolkit](https://github.com/Michdo93/vl53l1x-gesture-toolkit) testen
* [ ] [door-traffic-counter](https://github.com/Michdo93/door-traffic-counter) testen
* [ ] [vl53l5cx_gesture_experiments](https://github.com/Michdo93/vl53l5cx_gesture_experiments) testen
* [ ] [Nao-Gym-Instructor](https://github.com/Michdo93/Nao-Gym-Instructor) testen
* [ ] [openhab-sheets-rules](https://github.com/Michdo93/openhab-sheets-rules) testen
* [ ] [pepper_ros2_ws](https://github.com/Michdo93/pepper_ros2_ws) testen
* [ ] [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) testen
* [ ] [Smart-Home-Security-Lab](https://github.com/Michdo93/Smart-Home-Security-Lab) testen
* [ ] [therenect-linux](https://github.com/Michdo93/therenect-linux) testen
* [ ] [NFC-RFID-Examples](https://github.com/Michdo93/NFC-RFID-Examples) testen
* [ ] [invisible-spatial-switch](https://github.com/Michdo93/invisible-spatial-switch) testen
* [ ] [samsungtv](https://github.com/Michdo93/samsungtv) testen
* [ ] [interactive-projector](https://github.com/Michdo93/interactive-projector) testen
* [ ] [Brother-VC-500W](https://github.com/Michdo93/Brother-VC-500W) testen
* [ ] [complaints-hotline](https://github.com/Michdo93/complaints-hotline) testen
* [ ] [adidas-miCoach-Smart-Ball-Python](https://github.com/Michdo93/adidas-miCoach-Smart-Ball-Python) testen
* [ ] [Philips-AEA3000-00-Noise-Guard](https://github.com/Michdo93/Philips-AEA3000-00-Noise-Guard) testen
* [ ] [beamctl](https://github.com/Michdo93/beamctl) testen
* [ ] [Smarter-SMK20-EU](https://github.com/Michdo93/Smarter-SMK20-EU) testen
* [ ] [7Links-Home-Security-Rover-Controller](https://github.com/Michdo93/7Links-Home-Security-Rover-Controller) testen
* [ ] `smart-farm-house` 🔒 testen
* [ ] [arlo-cam-tests](https://github.com/Michdo93/arlo-cam-tests) testen
* [ ] [esp32-csi-presence-sensor](https://github.com/Michdo93/esp32-csi-presence-sensor) testen
* [ ] [hololens-viewer](https://github.com/Michdo93/hololens-viewer) testen
* [ ] [ESP32-Realtime-System](https://github.com/Michdo93/ESP32-Realtime-System) testen
* [ ] [ir-usb-hid-transreceiver](https://github.com/Michdo93/ir-usb-hid-transreceiver) testen
* [ ] [openHAB-Application-Checker](https://github.com/Michdo93/openHAB-Application-Checker) testen
* [ ] [openHAB-RuleManager](https://github.com/Michdo93/openHAB-RuleManager) testen
* [ ] [status-openhab-org](https://github.com/Michdo93/status-openhab-org) testen
* [ ] [openHAB-Steam-HTC-Vive](https://github.com/Michdo93/openHAB-Steam-HTC-Vive) testen
* [ ] [openHAB-xbox-remote-power](https://github.com/Michdo93/openHAB-xbox-remote-power) testen

---

## Nicht zum Laufen gebracht

Diese Ansätze sind bisher gescheitert. Die Erkenntnisse sind trotzdem wertvoll.

| Repository | Beschreibung | Sprache | Vorhaben | Hinweis |
| --- | --- | --- | --- | --- |
| [Flashing-Asus-RT-AC86U-for-Wi-Fi-Sensing](https://github.com/Michdo93/Flashing-Asus-RT-AC86U-for-Wi-Fi-Sensing) | Asus RT-AC86U für Wi-Fi Sensing flashen | – | [ESP32-CSI-Präsenzsensor](Experimente/ESP32-CSI-Sensor.md) | – |
| [Pepper-Selfie-Python](https://github.com/Michdo93/Pepper-Selfie-Python) | Pepper-Selfie in Python 2.7 / NAOqi 2.5 | Python | [Pepper-Selfie](Demos/Pepper-Selfie.md) | – |

**Aufgaben:**

* [ ] [Flashing-Asus-RT-AC86U-for-Wi-Fi-Sensing](https://github.com/Michdo93/Flashing-Asus-RT-AC86U-for-Wi-Fi-Sensing) Ursache dokumentieren, weiterverfolgen oder archivieren
* [ ] [Pepper-Selfie-Python](https://github.com/Michdo93/Pepper-Selfie-Python) Ursache dokumentieren, weiterverfolgen oder archivieren

---

## Deprecated und entfernt

Diese Repositories werden **nicht mehr weiterentwickelt**; einige sind im Labor bereits entfernt. Sie bleiben als Dokumentation erhalten – die verlinkten Vorhaben erklären, was es war, was daraus geworden ist und woran man anknüpfen kann. Die Spalte *Abgelöst durch* nennt, wo bekannt, den Nachfolger.

| Repository | Beschreibung | Sprache | Abgelöst durch | Vorhaben |
| --- | --- | --- | --- | --- |
| [crestron-roomview](https://github.com/Michdo93/crestron-roomview) | Docker-Container für Crestron RoomView (Flash) im virtuellen Display | Python | [BenQ-RS232-TCP](https://github.com/Michdo93/BenQ-RS232-TCP) | [BenQ MH856UST (Beamer)](Ger%C3%A4teintegration/BenQ-MH856UST.md) |
| [openHAB-Crestron-RoomView-Control](https://github.com/Michdo93/openHAB-Crestron-RoomView-Control) | Crestron-RoomView-Flash-Anwendung mit openHAB steuern | Python | [BenQ-RS232-TCP](https://github.com/Michdo93/BenQ-RS232-TCP) | [BenQ MH856UST (Beamer)](Ger%C3%A4teintegration/BenQ-MH856UST.md) |
| [Somfy-TaHoma-Developer-Mode-Python](https://github.com/Michdo93/Somfy-TaHoma-Developer-Mode-Python) | Python-Skript für die lokale API von Somfy TaHoma | Python | [Somfy-TaHoma-Developer-Mode-Postman-Collection](https://github.com/Michdo93/Somfy-TaHoma-Developer-Mode-Postman-Collection) | [Somfy TaHoma (lokale API)](Ger%C3%A4teintegration/Somfy-TaHoma.md) |
| [webtv_selenium](https://github.com/Michdo93/webtv_selenium) | Login bei deutschen Web-TV-Livestreams per Selenium | Python | [webtv-openhab](https://github.com/Michdo93/webtv-openhab) | [WebTV](Experimente/WebTV.md) |
| [openHAB-VLC-Control](https://github.com/Michdo93/openHAB-VLC-Control) | VLC per Exec Action steuern | Python | [webtv-openhab](https://github.com/Michdo93/webtv-openhab) | [WebTV](Experimente/WebTV.md) |
| [python-german-epg](https://github.com/Michdo93/python-german-epg) | EPG für deutsches Fernsehen per Web-Scraping | Python | [webtv-openhab](https://github.com/Michdo93/webtv-openhab) | [WebTV](Experimente/WebTV.md) |
| [openHAB-Command-Proxy-Jython](https://github.com/Michdo93/openHAB-Command-Proxy-Jython) | Jython/Flask: Commands per GET-Request an Items | Python | openHAB-REST-Clients | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [openHAB-Command-Proxy](https://github.com/Michdo93/openHAB-Command-Proxy) | Flask-API: GET-Request wird als POST an die REST API weitergeleitet | Python | openHAB-REST-Clients | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [digitalstrom-export-csv](https://github.com/Michdo93/digitalstrom-export-csv) | digitalSTROM-Messdaten per Selenium/PyAutoGUI als CSV herunterladen | Python | – | [digitalSTROM-Messdaten exportieren](Ger%C3%A4teintegration/digitalSTROM-Export.md) |
| [vmrc-control](https://github.com/Michdo93/vmrc-control) | VMRC-Verbindung zu einer VM per Skript | Python | – | [Frühere Hilfsskripte](Infrastruktur/Alte-Hilfsskripte.md) |
| [openHAB-QR-Code-Scanner](https://github.com/Michdo93/openHAB-QR-Code-Scanner) | Android-App zum Scannen von QR-Codes für openHAB-Items | Java | [openhab-qr-code-scanner-webapp](https://github.com/Michdo93/openhab-qr-code-scanner-webapp) | [QR-Code-Steuerung](Ger%C3%A4teintegration/QR-Code-Steuerung.md) |
| [openHAB-REST-API-Proxy](https://github.com/Michdo93/openHAB-REST-API-Proxy) | Proxy für die openHAB REST API mit CORS-Headern | Python | openHAB-REST-Clients | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [Smart-Charging-Station](https://github.com/Michdo93/Smart-Charging-Station) | REST-API zum Schalten eines USB-Hubs (uhubctl) nach Akkustand | Python | – | [Smart Charging Station](Experimente/Smart-Charging-Station.md) |
| [openhab-python-rest-api-examples](https://github.com/Michdo93/openhab-python-rest-api-examples) | Beispiele zur openHAB REST API mit Python | Python | [python-openhab-rest-client](https://github.com/Michdo93/python-openhab-rest-client) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [openhab_bridge_publisher](https://github.com/Michdo93/openhab_bridge_publisher) | ROS: Commands an openHAB publizieren | Python | [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [openhab_bridge_subscriber](https://github.com/Michdo93/openhab_bridge_subscriber) | ROS: States von openHAB abonnieren | C++ | [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [openhab_bridge_image_listener](https://github.com/Michdo93/openhab_bridge_image_listener) | ROS: Bild-Topics als Command an openHAB | CMake | [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [HABApp-ROS-openHAB-Bridge](https://github.com/Michdo93/HABApp-ROS-openHAB-Bridge) | ROS-openHAB-Bridge mit HABApp | Python | [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [python-openhab-eventbus](https://github.com/Michdo93/python-openhab-eventbus) | MQTT-Event-Bus für openHAB | Python | [HABApp-MQTT-Event-Bus](https://github.com/Michdo93/HABApp-MQTT-Event-Bus) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [python-openhab-logsaver](https://github.com/Michdo93/python-openhab-logsaver) | openHAB-Logs in eine Datenbank speichern | Python | – | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [python-openhab-itemevents](https://github.com/Michdo93/python-openhab-itemevents) | Item-Events per SSE | Python | [python-openhab-rest-client](https://github.com/Michdo93/python-openhab-rest-client) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [python-openhab-item](https://github.com/Michdo93/python-openhab-item) | Python-Klassen für openHAB-Items | Python | [python-openhab-rest-client](https://github.com/Michdo93/python-openhab-rest-client) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [python-openhab-crud](https://github.com/Michdo93/python-openhab-crud) | CRUD für die openHAB REST API | Python | [python-openhab-rest-client](https://github.com/Michdo93/python-openhab-rest-client) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [openHAB-LogSaver](https://github.com/Michdo93/openHAB-LogSaver) | openHAB-Logs in eine Datenbank speichern | Python | – | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [openHAB-Python-Item](https://github.com/Michdo93/openHAB-Python-Item) | Python-Klassen für openHAB-Items | Python | [python-openhab-rest-client](https://github.com/Michdo93/python-openhab-rest-client) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [openHAB-Python-ItemEvents](https://github.com/Michdo93/openHAB-Python-ItemEvents) | Item-Events per SSE | Python | [python-openhab-rest-client](https://github.com/Michdo93/python-openhab-rest-client) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [openhab_python_crud](https://github.com/Michdo93/openhab_python_crud) | CRUD für die openHAB REST API | Python | [python-openhab-rest-client](https://github.com/Michdo93/python-openhab-rest-client) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [openHAB-web-radio](https://github.com/Michdo93/openHAB-web-radio) | Webradio über das Sonos Binding mit MP3-Livestreams | – | [webradio-openhab](https://github.com/Michdo93/webradio-openhab) | [Sonos und Webradio](Ger%C3%A4teintegration/Sonos-und-Webradio.md) |
| [openHAB-web-tv](https://github.com/Michdo93/openHAB-web-tv) | TV-Streams per Exec Binding und SSH auf entferntem Rechner | – | [webtv-openhab](https://github.com/Michdo93/webtv-openhab) | [WebTV](Experimente/WebTV.md) |
| [Exec-Binding-and-Exec-Action-Compendium](https://github.com/Michdo93/Exec-Binding-and-Exec-Action-Compendium) | Kompendium zu Exec Binding und Exec Action | – | Informatik-Kompendium (Whitelist) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [openHAB-Python-Compendium](https://github.com/Michdo93/openHAB-Python-Compendium) | Python-Kompendium für openHAB | – | Informatik-Kompendium, openHAB Design Patterns | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [openhab_bridge](https://github.com/Michdo93/openhab_bridge) | Bridge zwischen openHAB und ROS (1) | – | [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [openhab_bridge_plot_publisher](https://github.com/Michdo93/openhab_bridge_plot_publisher) | ROS: Plots publizieren | – | [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [openhab_bridge_map_listener](https://github.com/Michdo93/openhab_bridge_map_listener) | ROS: Karten-Topic als Bild an openHAB | Python | [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [Python-Bytes-Image-To-Base64-Image-Conversion](https://github.com/Michdo93/Python-Bytes-Image-To-Base64-Image-Conversion) | Bytes → Base64 | Python | – | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [Python-Base64-Image-To-Bytes-Image-Conversion](https://github.com/Michdo93/Python-Base64-Image-To-Bytes-Image-Conversion) | Base64 → Bytes | Python | – | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [Python-Bytes-Image-Conversion](https://github.com/Michdo93/Python-Bytes-Image-Conversion) | Bytes ↔ Bild | Python | – | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [Python-Base64-Image-Conversion](https://github.com/Michdo93/Python-Base64-Image-Conversion) | Base64 ↔ Bild | Python | – | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [base64_subscriber](https://github.com/Michdo93/base64_subscriber) | ROS: Base64-Bild abonnieren und in OpenCV umwandeln | CMake | – | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [base64_publisher](https://github.com/Michdo93/base64_publisher) | ROS: Base64-Bild publizieren | CMake | – | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [opencv_node](https://github.com/Michdo93/opencv_node) | ROS-Node für OpenCV-Bilder | CMake | – | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [openhab_bridge_plotter](https://github.com/Michdo93/openhab_bridge_plotter) | ROS: Plotter | – | [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [openhab_msgs](https://github.com/Michdo93/openhab_msgs) | ROS-Nachrichtentypen für openHAB | CMake | [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [openhab-ai](https://github.com/Michdo93/openhab-ai) | ML-basierte Regel-Engine (experimentell) | Python | [oh-ai-bridge](https://github.com/Michdo93/oh-ai-bridge), Idee „State Prediction“ | [openhab-ai: ML-basierte Regel-Engine](openHAB/openHAB-AI-Regel-Engine.md) |
| [Beam-Remote-Decompiled3](https://github.com/Michdo93/Beam-Remote-Decompiled3) | Dekompilierte Beam-Remote-App (Smali) | Smali | [beamctl](https://github.com/Michdo93/beamctl) – als Quelle behalten | [Beam Labs Beam (Projektor-Lampen)](Experimente/Beam-Labs-Beam.md) |
| [Beam-Remote-Decompiled2](https://github.com/Michdo93/Beam-Remote-Decompiled2) | Dekompilierte Beam-Remote-App (Java) | Java | [beamctl](https://github.com/Michdo93/beamctl) – als Quelle behalten | [Beam Labs Beam (Projektor-Lampen)](Experimente/Beam-Labs-Beam.md) |
| [Beam-Remote-Decompiled](https://github.com/Michdo93/Beam-Remote-Decompiled) | Dekompilierte Beam-Remote-App (Smali) | Smali | [beamctl](https://github.com/Michdo93/beamctl) – als Quelle behalten | [Beam Labs Beam (Projektor-Lampen)](Experimente/Beam-Labs-Beam.md) |
| [pepper_brute_force](https://github.com/Michdo93/pepper_brute_force) | Verbindungsaufbau zu Pepper per Brute Force (schaltet Roboter im Netz ab) | Python | – | [Sicherheit der NAO-/Pepper-Roboter](Experimente/NAOqi-Sicherheit.md) |
| [python-port-scanner](https://github.com/Michdo93/python-port-scanner) | Einfacher Portscanner | Python | nmap | [Frühere Hilfsskripte](Infrastruktur/Alte-Hilfsskripte.md) |
| [iot_bridge](https://github.com/Michdo93/iot_bridge) | Bridge zwischen ROS und openHAB 3 | Python | [ros2_openhab_ws](https://github.com/Michdo93/ros2_openhab_ws) | [ROS-1-Bridge zwischen openHAB und ROS](openHAB/ROS1-openHAB-Bridge-Historie.md) |
| [rs232](https://github.com/Michdo93/rs232) | Einfacher Python-Handler für RS232-Geräte | Python | [BenQ-RS232-TCP](https://github.com/Michdo93/BenQ-RS232-TCP) | [Frühere Hilfsskripte](Infrastruktur/Alte-Hilfsskripte.md) |
| [openHAB-Helper-Libraries-MQTT-Event-Bus](https://github.com/Michdo93/openHAB-Helper-Libraries-MQTT-Event-Bus) | MQTT-Event-Bus mit den Helper Libraries (openHAB 2/3) | Python | [HABApp-MQTT-Event-Bus](https://github.com/Michdo93/HABApp-MQTT-Event-Bus) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [python-openhab](https://github.com/Michdo93/python-openhab) | Python-Bibliothek für die openHAB REST API | Python | [python-openhab-rest-client](https://github.com/Michdo93/python-openhab-rest-client) | [Frühere Python-Bibliotheken und Proxys für openHAB](openHAB/Python-Bibliotheken-Historie.md) |
| [Pepper_ConciergeShort](https://github.com/Michdo93/Pepper_ConciergeShort) | Kurzvariante des Pepper-Concierge | – | [Pepper_ConciergeShortSSH](https://github.com/Michdo93/Pepper_ConciergeShortSSH) | [Pepper-Concierge](Demos/Pepper-Concierge.md) |

**Aufgaben:**

* [ ] In jedem deprecated Repository oben in der README einen Hinweis ergänzen („Deprecated – abgelöst durch …“)
* [ ] Repositories auf GitHub **archivieren** (Settings → Archive), damit klar ist, dass sie nicht mehr gepflegt werden
* [ ] Prüfen, ob im Labor noch Reste laufen (Services, Cron-Jobs, Container) – und diese entfernen
* [ ] Die Beam-Remote-Decompiled-Repos **nicht löschen**: Sie sind Quelle für `beamctl`

Ausführliche Checkliste pro Repository: [Deprecated Repositories kennzeichnen und archivieren](Infrastruktur/Deprecated-Repos-aufraeumen.md). Vorgehen und Vorlage: [Repositories pflegen und archivieren](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/Repositories%20pflegen%20%26%20archivieren.md) im Kompendium Informatik.

---
