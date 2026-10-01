# 📡 WebTV

| | |
| --- | --- |
| **Status** | 🧪 Experiment |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Multimedia |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Ideen und Szenarien](#ideen-und-szenarien)
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

---

## Offene Aufgaben

* [ ] Testen und ggf. anpassen
* [ ] Szenario mit dem Beamer umsetzen

---

## Ideen und Szenarien

* Sender auswählen → Rule schaltet den [Beamer](../Geräteintegration/BenQ-MH856UST.md) ein → Quelle Raspberry Pi → Stream im Vollbild.

---

## Repositories

* [webtv-openhab](https://github.com/Michdo93/webtv-openhab)

---
