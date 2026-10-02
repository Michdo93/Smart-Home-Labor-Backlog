# 🗂️ Things und Items als Textdateien

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Things und Items sind textbasiert konfiguriert und damit versioniert und im Git-Backup enthalten.

---

## Ist-Stand

* ✅ Alle Things aus der UI gelöscht und als `.things`-Dateien neu angelegt. Neue Geräte werden künftig ebenfalls per `.things`-Datei konfiguriert.
* ✅ Doppelte Items (Inkonsistenzen zwischen UI- und `.items`-Konfiguration) gelöscht.
* Die Datei `Things.json` unter `/var/lib/openhab/jsondb/` wird zusätzlich in einem eigenen Repository für `/var/lib/openhab` gesichert.
* Die `.things`-Dateien werden mit einem eigenen Exporter erzeugt (`openhab-things-exporter`).
* Bekannte Fehler des Exporters: teilweise falsches Binding-Präfix vor Channel-Typen und überflüssige Leerzeichen um den Doppelpunkt der Thing-UID. Vorgehen: zuerst alle exportierten Dateien von Hand korrigieren, danach den Exporter.

---

## Offene Aufgaben

* [ ] Konvention „neue Geräte nur per Textdatei“ in der Labordokumentation festhalten
* [ ] Exportierte `.things`-Dateien auf die bekannten Fehler prüfen und korrigieren
* [ ] Fehler im Exporter beheben und mit allen Bindings des Labors testen

---

## Repositories

* [openhab-things-exporter](https://github.com/Michdo93/openhab-things-exporter)

---
