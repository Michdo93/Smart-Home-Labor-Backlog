# 🖐️ Multitouchtisch & HTC Vive

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Multimedia |
| **Geeignet für** | Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Der Multitouchtisch und der VR-Rechner (HTC Vive) lassen sich aus openHAB heraus bedienen: Rechner per Wake-on-LAN wecken, Anwendungen (Steam/SteamVR, VR-Spiele) starten.

---

## Ist-Stand

* Erprobt: VR-Rechner per Wake-on-LAN wecken, per OpenSSH + PsExec Steam-Apps starten (`-applaunch <id>`), Eingaben per xdotool.
* Liste von VR-Apps vorhanden (SteamVR, The Lab, Beat Saber, Rec Room u. a.).
* Multitouchtisch mit Pepper's-Ghost-Pyramide im IoT-Raum (siehe [Hologram Fan Projector](Hologram-Fan-Projector.md) zur Abgrenzung).

---

## Offene Aufgaben

* [ ] Rechner per WoL und geregeltes Herunterfahren einbinden
* [ ] Start einzelner VR-Apps über openHAB testen
* [ ] Als Demo aufbereiten (z. B. Vive-Bild per HDMI/Capture auf den Beamer, siehe Wireless HDMI Matrix)

---

## Abhängigkeiten

* [Anwendungen auf PCs fernsteuern](../Infrastruktur/Remote-Anwendungssteuerung.md)
* [VR und AR](VR-AR.md)

---

## Hinweise und Risiken

* Setzt die [Anwendungs-Fernsteuerung](../Infrastruktur/Remote-Anwendungssteuerung.md) voraus.

---

## Repositories

* [openHAB-Steam-HTC-Vive](https://github.com/Michdo93/openHAB-Steam-HTC-Vive)

---
