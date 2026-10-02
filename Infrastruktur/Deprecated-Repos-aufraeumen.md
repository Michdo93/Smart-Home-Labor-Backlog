# 🗄️ Deprecated Repositories kennzeichnen und archivieren

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Alle nicht mehr gepflegten Repositories sind auf GitHub eindeutig als **deprecated** erkennbar, verweisen auf ihren Nachfolger und sind archiviert. Im Labor laufen keine Reste mehr davon.

---

## Ist-Stand

* In der [Repository-Übersicht](../Repositories.md#deprecated-und-entfernt) sind 54 Repositories als deprecated bzw. entfernt gelistet, teilweise mit Nachfolger.
* Die meisten haben noch keinen Deprecated-Hinweis und sind nicht archiviert.

---

## Offene Aufgaben

* [ ] Für jedes Repository: Nachfolger bestätigen oder „kein Nachfolger“ eintragen
* [ ] Deprecated-Hinweis oben in die README (Vorlage siehe Hinweise)
* [ ] Beschreibung (About) mit `[DEPRECATED]` beginnen
* [ ] Im Labor prüfen, ob noch etwas davon läuft (systemd-Services, Cron-Jobs, Container, Einträge in `misc/exec.whitelist`) und entfernen
* [ ] Repository archivieren
* [ ] In der Repository-Übersicht abhaken

---

## Hinweise und Risiken

* Die `Beam-Remote-Decompiled`-Repos **nicht löschen**: Sie sind die Quelle für `beamctl`.
* Im Zweifel archivieren, nicht löschen.
* Vorlage und Vorgehen: [Repositories pflegen & archivieren](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/Repositories%20pflegen%20%26%20archivieren.md)

---

