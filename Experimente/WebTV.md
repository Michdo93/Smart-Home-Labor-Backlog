# 📡 WebTV

| | |
| --- | --- |
| **Status** | 🔍 Test ausstehend |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Multimedia |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Ideen und Szenarien](#ideen-und-szenarien)
- [Historie](#historie)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Fernsehstreams im Smart Home abspielen – lokal oder auf einem entfernten Gerät.

---

## Ist-Stand

* Eigene Lösung mit **MPV** statt VLC (weniger Ressourcenbedarf).
* Die Rule startet den Player entweder lokal oder – bei konfigurierter SSH-Verbindung – auf einem entfernten Gerät.
* Die Items enthalten Metadaten mit **m3u8-Streams** (öffentlich verfügbar, z. B. aus Kodi-Konfigurationen).
* Oberfläche als HTML statt Sitemap.
* Vorgänger sind **deprecated**: `openHAB-web-tv` (Exec Binding + SSH, VLC oder Browser), `openHAB-VLC-Control`, `webtv_selenium` (Login bei Web-TV-Streams), `python-german-epg` (EPG per Web-Scraping).

---

## Offene Aufgaben

* [ ] Testen und ggf. anpassen
* [ ] Szenario mit dem Beamer umsetzen

---

## Ideen und Szenarien

* Sender auswählen → Rule schaltet den [Beamer](../Geräteintegration/BenQ-MH856UST.md) ein → Quelle Raspberry Pi → Stream im Vollbild.

---

## Historie

Frühere Ansätze, die inzwischen **deprecated** sind:

* [openHAB-web-tv](https://github.com/Michdo93/openHAB-web-tv) – TV-Streams per Exec Binding und SSH auf einem entfernten Rechner (VLC oder Browser)
* [openHAB-VLC-Control](https://github.com/Michdo93/openHAB-VLC-Control) – VLC per Exec Action und Python-Skript steuern
* [webtv_selenium](https://github.com/Michdo93/webtv_selenium) – Login bei deutschen Web-TV-Livestreams per Selenium
* [python-german-epg](https://github.com/Michdo93/python-german-epg) – EPG für deutsches Fernsehen per Web-Scraping (TV Spielfilm)

---

## Repositories

* [webtv-openhab](https://github.com/Michdo93/webtv-openhab)

---
