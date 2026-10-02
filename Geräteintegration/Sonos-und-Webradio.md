# 📻 Sonos und Webradio

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟠 Mittel |
| **Raum** | Konferenz, Küche, Bad, IoT, Multimedia |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
  - [IP-Adressen der Sonos-Geräte](#ip-adressen-der-sonos-geräte)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Historie](#historie)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

In jedem Raum lässt sich über eine ansprechende Weboberfläche Webradio auf den Sonos-Lautsprechern abspielen. Langfristig sollen alle Lautsprecher **gemeinsam** in einer Zone synchron spielen können.

---

## Ist-Stand

* Alle Sonos-Geräte haben jetzt eine **feste IP** per DHCP-Reservierung (siehe Tabelle). Fortgesetzt wurde bei `.131`, weil `.30` und `.31` aufeinander aufbauen würden.
* **423 Radiostreams** sind getestet (per Skript, jeder Stream manuell bestätigt).
* Webradio-Oberfläche als eigene Webseite unter `/static/webradio/<raum>/` statt Sitemap – zuerst für Konferenz, danach für die übrigen vier Räume.
* In Sonos ist **keine Zone für den Raum „Smart Home“** konfiguriert.

### IP-Adressen der Sonos-Geräte

| IP-Adresse | Thing |
| --- | --- |
| 192.168.0.30 | `tMultimedia_Sonos_Lautsprecher` |
| 192.168.0.131 | `tBad_Sonos_Lautsprecher` ⬆️ Upgrade nötig |
| 192.168.0.132 | `tIoT_Sonos_Lautsprecher` ⬆️ Upgrade nötig |
| 192.168.0.133 | `tKonferenz_Sonos_Subwoofer` |
| 192.168.0.134 | `tKueche_Sonos_Lautsprecher` ⬆️ Upgrade nötig |
| 192.168.0.135 | `tMultimedia_Sonos_Playbar` |
| 192.168.0.136 | `tMultimedia_Sonos_Subwoofer` |
| 192.168.0.137 | `tKonferenz_Sonos_Playbar` |


---

## Offene Aufgaben

* [ ] Webradio-Seiten für alle fünf Räume prüfen
* [ ] Zone für den Raum Smart Home klären
* [ ] Firmware-Upgrade der Lautsprecher `.131` (Bad), `.132` (IoT) und `.134` (Küche), damit alle in eine gemeinsame Zone können
* [ ] In der **Sonos-App am Smartphone** (nicht über die Windows-Anwendung) alle Geräte aus ihren Zonen entfernen und in dieselbe Zone eintragen, Master festlegen
* [ ] Danach eine zusätzliche Ebene „alle Räume“ in der Webradio-Oberfläche

---

## Hinweise und Risiken

* Upgrades haben in der Vergangenheit Probleme gemacht. Schlagen sie fehl, müssen ggf. andere Geräte **downgegradet** oder aus dem System entfernt und neu hinzugefügt werden.
* Deshalb: Upgrades **nie kurz vor einer Labor-Demo**.
* Der Lautsprecher im Multimedia-Raum wird vom [Pepper-Concierge](../Demos/Pepper-Concierge.md) direkt angesprochen.
* Vorgänger `openHAB-web-radio` (Sonos Binding mit MP3-Livestreams) ist deprecated.

---

## Historie

Frühere Ansätze, die inzwischen **deprecated** sind:

* [openHAB-web-radio](https://github.com/Michdo93/openHAB-web-radio) – Webradio über das Sonos Binding mit MP3-Livestreams

---

## Repositories

* [webradio-openhab](https://github.com/Michdo93/webradio-openhab)

---
