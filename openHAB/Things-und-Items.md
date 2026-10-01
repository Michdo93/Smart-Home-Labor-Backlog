# 🗂️ Things und Items als Textdateien

| | |
| --- | --- |
| **Status** | ✅ Erledigt |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | – |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
<!-- /TOC -->

## Ziel

Things und Items sind textbasiert konfiguriert und damit versioniert und im Git-Backup enthalten.

---

## Ist-Stand

* ✅ Alle Things aus der UI gelöscht und als `.things`-Dateien neu angelegt. Neue Geräte werden künftig ebenfalls per `.things`-Datei konfiguriert.
* ✅ Doppelte Items (Inkonsistenzen zwischen UI- und `.items`-Konfiguration) gelöscht.
* Die Datei `Things.json` unter `/var/lib/openhab/jsondb/` wird zusätzlich in einem eigenen Repository für `/var/lib/openhab` gesichert.

---

## Offene Aufgaben

* [ ] Konvention „neue Geräte nur per Textdatei“ in der Labordokumentation festhalten

---

