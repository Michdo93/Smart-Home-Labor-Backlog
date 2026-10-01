# 🗂️ Smart-Home-Labor-Backlog

Dieses Repository sammelt alles, was im **Smart Home Labor der Hochschule Furtwangen (HFU)** noch **umgesetzt, getestet, repariert oder ausprobiert** werden soll – von der Fehlerbehebung in einer Labor-Demo über die Integration neuer Geräte bis zu Experimenten mit offenem Ausgang.

Es ist bewusst **keine Roadmap mit Terminen**, sondern ein **Backlog**: eine gepflegte, priorisierte Liste offener Vorhaben. Zu jedem Vorhaben gibt es eine eigene Datei mit Ziel, Ist-Stand, offenen Aufgaben, Hinweisen und den zugehörigen Repositories.

<!-- TOC -->
## Inhaltsverzeichnis

- [Wofür ist dieses Repository?](#wofür-ist-dieses-repository)
- [Legende](#legende)
  - [Status](#status)
  - [Priorität](#priorität)
- [Demos](#demos)
- [Geräteintegration](#geräteintegration)
- [Infrastruktur](#infrastruktur)
- [openHAB](#openhab)
- [Experimente](#experimente)
- [Mitarbeit](#mitarbeit)
  - [Ein neues Vorhaben anlegen](#ein-neues-vorhaben-anlegen)
  - [Ein Vorhaben aktualisieren](#ein-vorhaben-aktualisieren)
  - [Konventionen](#konventionen)
<!-- /TOC -->

## Wofür ist dieses Repository?

* **Überblick:** Was ist im Labor offen, was blockiert, was ist fast fertig?
* **Übergabe:** Wer ein Vorhaben übernimmt, findet den aktuellen Stand und die nächsten Schritte, ohne E-Mails durchsuchen zu müssen.
* **Aufgaben für Hiwis, Praxissemester und Studienprojekte:** Jedes Vorhaben ist eingeschätzt, für wen es sich eignet. Rahmenbedingungen und Voraussetzungen stehen im Repository [Praktika im Smart Home Labor](https://github.com/Michdo93/Praktika-Smart-Home-Labor).
* **Gedächtnis:** Auch verworfene Ansätze und Erkenntnisse bleiben erhalten (z. B. warum ein Weg nicht funktioniert hat).

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

Labor-Demos, die Besuchern gezeigt werden.

| Vorhaben | Status | Priorität | Raum |
| --- | --- | --- | --- |
| 🌅 [Morgenroutine](Demos/Morgenroutine.md) | 🚧 In Arbeit | 🔴 Hoch | Mehrere Räume |
| 🤖 [Pepper-Concierge](Demos/Pepper-Concierge.md) | 🚧 In Arbeit | 🔴 Hoch | Multimedia |

---

## Geräteintegration

Geräte, deren Einbindung begonnen hat oder weitgehend fertig ist.

| Vorhaben | Status | Priorität | Raum |
| --- | --- | --- | --- |
| 📰 [Newspaper Projector](Ger%C3%A4teintegration/Newspaper-Projector.md) | 🚧 In Arbeit | 🔴 Hoch | Multimedia |
| 👥 [People Counter](Ger%C3%A4teintegration/People-Counter.md) | 🔍 Test ausstehend | 🟠 Mittel | Zwischen IoT und Multimedia |
| 📽️ [BenQ MH856UST (Beamer)](Ger%C3%A4teintegration/BenQ-MH856UST.md) | 🔍 Test ausstehend | 🔴 Hoch | Multimedia |
| 📷 [PTZ-IP-Kamera PremiumBlue PIPC-011](Ger%C3%A4teintegration/IP-Kamera-PIPC-011.md) | ⛔ Blockiert | 🟠 Mittel | – |
| 🔔 [Doorbird D101 (Türsprechanlage)](Ger%C3%A4teintegration/Doorbird-D101.md) | 🔍 Test ausstehend | 🟢 Niedrig | – |
| 📻 [Sonos und Webradio](Ger%C3%A4teintegration/Sonos-und-Webradio.md) | 🚧 In Arbeit | 🟠 Mittel | Konferenz, Küche, Bad, IoT, Multimedia |

---

## Infrastruktur

Server, Netzwerk, Hardware-Installation im Labor.

| Vorhaben | Status | Priorität | Raum |
| --- | --- | --- | --- |
| ⚙️ [Ansible](Infrastruktur/Ansible.md) | 🚧 In Arbeit | 🟠 Mittel | Server / alle Systeme |
| 📱 [Wand-Tablets im Kiosk-Modus](Infrastruktur/Tablets-und-Kiosk.md) | 🚧 In Arbeit | 🟠 Mittel | Alle Räume |
| ☎️ [Intercom (Asterisk)](Infrastruktur/Intercom-Asterisk.md) | ⛔ Blockiert | 🟠 Mittel | Alle Räume |
| 🔌 [Raspberry Pis als USB/IP-Server](Infrastruktur/USB-IP-Server.md) | 🚧 In Arbeit | 🟠 Mittel | Alle Räume (Konferenz: 2) |

---

## openHAB

Konfiguration, Rules und Oberflächen von openHAB.

| Vorhaben | Status | Priorität | Raum |
| --- | --- | --- | --- |
| 📜 [Migration der Rules](openHAB/Rules-Migration.md) | 🚧 In Arbeit | 🔴 Hoch | – |
| 🗂️ [Things und Items als Textdateien](openHAB/Things-und-Items.md) | ✅ Erledigt | 🟢 Niedrig | – |
| 🧭 [Sitemaps und MainUI](openHAB/Sitemaps-und-MainUI.md) | 🚧 In Arbeit | 🟢 Niedrig | – |
| 🖥️ [Eigene HTML-Dashboards](openHAB/Dashboards.md) | 🚧 In Arbeit | 🟠 Mittel | Alle Räume |
| 🔧 [Kleinere Optimierungen](openHAB/Optimierungen.md) | 💡 Idee | 🟢 Niedrig | – |

---

## Experimente

Geräte und Ideen, die erst noch erprobt werden.

| Vorhaben | Status | Priorität | Raum |
| --- | --- | --- | --- |
| 📻 [Imperial Dabman i250 (Internetradio)](Experimente/Imperial-Dabman-i250.md) | 🧪 Experiment | 🟢 Niedrig | – |
| ⚖️ [Withings Home Kamera und Personenwaage](Experimente/Withings.md) | 🧪 Experiment | 🟢 Niedrig | – |
| 📺 [Samsung SmartTV](Experimente/Samsung-SmartTV.md) | 🧪 Experiment | 🟢 Niedrig | – |
| 🚙 [7Links Home Security Rover](Experimente/7Links-Home-Security-Rover.md) | 🧪 Experiment | 🟢 Niedrig | IoT |
| 📡 [WebTV](Experimente/WebTV.md) | 🧪 Experiment | 🟢 Niedrig | Multimedia |
| 📶 [ESP32-CSI-Präsenzsensor](Experimente/ESP32-CSI-Sensor.md) | 🧪 Experiment | 🟠 Mittel | – |
| 🫖 [Smarter SMK20-EU (Wasserkocher)](Experimente/Smarter-SMK20-Wasserkocher.md) | 🧪 Experiment | 🟢 Niedrig | Küche |
| 💡 [Beam Labs Beam (Projektor-Lampen)](Experimente/Beam-Labs-Beam.md) | 🧪 Experiment | 🟢 Niedrig | – |
| 🎤 [Philips AEA3000/00 (Mikrofone)](Experimente/Philips-AEA3000.md) | 💡 Idee | 🟢 Niedrig | – |
| ⚽ [adidas miCoach Smart Ball](Experimente/adidas-miCoach-Smart-Ball.md) | 🧪 Experiment | 🟢 Niedrig | – |
| 🖨️ [Brother VC-500W (Etikettendrucker)](Experimente/Brother-VC-500W.md) | 🧪 Experiment | 🟢 Niedrig | – |
| 🌀 [3D Hologram Fan Projector](Experimente/Hologram-Fan-Projector.md) | 🧪 Experiment | 🟢 Niedrig | – |
| ✋ [Leap Motion](Experimente/Leap-Motion.md) | 🔍 Test ausstehend | 🟢 Niedrig | Alle Räume |
| 🏷️ [NFC/RFID](Experimente/NFC-RFID.md) | 🚧 In Arbeit | 🟢 Niedrig | – |

---

## Mitarbeit

### Ein neues Vorhaben anlegen

1. [VORLAGE.md](VORLAGE.md) in den passenden Ordner kopieren und sprechend benennen (`Geräte-Name.md`, keine Leerzeichen).
2. Ziel, Ist-Stand und offene Aufgaben ausfüllen.
3. In der passenden Tabelle oben eintragen.

### Ein Vorhaben aktualisieren

* Erledigte Aufgaben abhaken (`- [x]`), neue Erkenntnisse unter **Ist-Stand** ergänzen.
* Status und Priorität **in der Datei und in der Tabelle** anpassen.
* Abgeschlossene Vorhaben nicht löschen, sondern auf ✅ setzen – die Dokumentation des Wegs ist oft genauso wertvoll wie das Ergebnis.
* Code gehört in das jeweilige Projekt-Repository, nicht hierher. Hier stehen nur Stand, Aufgaben und Verweise.

### Konventionen

* Die Arbeitsweise im Labor (feste IPs, SSH, Zertifikate, MQTT, Ansible, Dokumentation) ist im Kompendium [Informatik](https://github.com/Michdo93/Informatik) unter [Best Practices](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/README.md) beschrieben.
* Keine Passwörter, Tokens oder personenbezogenen Daten in dieses Repository.

---
