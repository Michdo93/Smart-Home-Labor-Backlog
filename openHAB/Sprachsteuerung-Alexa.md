# 🗣️ Sprachsteuerung über Alexa

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟠 Mittel |
| **Raum** | Alle Räume |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Möglichst viele Funktionen des Labors lassen sich per Sprache über Alexa auslösen – nicht nur Geräte ein/aus, sondern auch Szenen und Anwendungen.

---

## Ist-Stand

* Alexa kann im Zusammenspiel mit openHAB vor allem **Switch-Items** schalten; der Ablauf ist: Sprachbefehl → Alexa-Routine → Switch in openHAB → Regel.
* Pro Aktion braucht es mindestens zwei Spracheingaben (an/aus), und sinnvollerweise mehrere Formulierungen pro Schalter.
* Ein Switch kann auch ein **virtuelles (unbound) Item** sein, das über eine Regel Beliebiges auslöst (Szene, Anwendung starten, Farbe setzen).
* Sprachausgabe über Alexa läuft über den **TTS-Buffer** je Echo (Regeln je Raum vorhanden).
* Die TTS-Regeln nutzen `Thread::sleep` – beim Übertragen auf Python 3 Scripting auf das Timing achten (siehe Rules-Migration).

---

## Offene Aufgaben

* [ ] Liste der gewünschten Sprachbefehle erstellen (Geräte, Szenen, Anwendungen)
* [ ] Switch-Items (real und virtuell) mit passender Semantik anlegen und als `switchable` markieren
* [ ] Alexa-Routinen zu den Switches einrichten; mehrere Formulierungen hinterlegen
* [ ] TTS-Regeln prüfen und ggf. migrieren
* [ ] Dokumentieren, welche Sprachbefehle es gibt (für Nutzer und Demos)

---

## Abhängigkeiten

* [Migration der Rules](Rules-Migration.md)

---

## Hinweise und Risiken

* **Abhängigkeit vom Alexa-Skill/Binding:** Amazons Richtlinien ändern sich; der openHAB-Alexa-Skill war zeitweise nicht verfügbar. Vor größerem Ausbau prüfen, ob die Anbindung noch unterstützt wird (siehe Idee „Sprachassistent“ für eine lokale Alternative).
* Eignet sich auch als Bachelorthesis: „Evaluierung von Sprachassistenz im Smart Home am Beispiel openHAB und Alexa“.
* Alexa-Sound-Library, Speechcons und SSML sind bereits vorhanden ([Repos migrierter Projekte aktualisieren](Repos-migrierter-Projekte-aktualisieren.md)).

---

