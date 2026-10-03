# 🔑 REST-API-Authentifizierung schaltbar

| | |
| --- | --- |
| **Status** | ⚰️ Deprecated |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Alle (zum Nachlesen) |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Frühere Lösung, um die Authentifizierung der openHAB REST API bei Bedarf an- und auszuschalten.

---

## Ist-Stand

* Über das Exec Binding und die openHAB-Karaf-Konsole (`bundle:start/stop org.openhab.core.io.rest.auth`) wurde die REST-Authentifizierung per Switch umgeschaltet.
* Diente als Workaround, als ältere Clients ohne Token auf die REST API zugreifen mussten.
* Heute besser: **API-Token** verwenden (die REST-Clients des Labors unterstützen das) und die Authentifizierung aktiviert lassen.

---

## Offene Aufgaben

* [ ] Prüfen, ob der Workaround noch irgendwo aktiv ist, und entfernen
* [ ] Clients auf Token-Authentifizierung umstellen

---

## Hinweise und Risiken

* Die Notiz enthielt das Karaf-Standardpasswort `habopen` im Klartext – Konsolenpasswort ändern.
* Grundlagen: [HTTP & REST](https://github.com/Michdo93/Informatik/blob/main/Netzwerk/HTTP%20%26%20REST.md), [Authentifizierung & Autorisierung](https://github.com/Michdo93/Informatik/blob/main/Zugriffskontrolle/Authentifizierung%20%26%20Autorisierung.md)

---

