# 📺 Sprachsteuerung für Multimedia-Geräte

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Multimedia |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
<!-- /TOC -->

## Ziel

Kodi, PlayStation und Xbox One lassen sich per Sprache (über Alexa bzw. die geräteeigenen Mittel) steuern.

---

## Ist-Stand

* Drei frühere Hiwi-Aufgaben: **Kodi** (über die kodi-cli), **PlayStation 4** (PS4-Sprachsteuerung) und **Xbox One** (über Alexa).
* Bisher nur Anleitungen gesammelt, nicht im Labor integriert.
* Verwandt: Die PS4 lässt sich auch über ein openHAB-PS4-Binding einbinden (Doku vorhanden); die Xbox One über das Exec Binding ein-/ausschalten (`openHAB-xbox-remote-power`).

---

## Offene Aufgaben

* [ ] Pro Gerät entscheiden, ob die Steuerung über Alexa, ein Binding oder Exec/SSH läuft
* [ ] Kodi über die kodi-cli bzw. das Kodi-Binding anbinden
* [ ] PS4 testen (Binding), Xbox One testen (Exec)
* [ ] Sprachbefehle in die [Alexa-Sprachsteuerung](../openHAB/Sprachsteuerung-Alexa.md) aufnehmen

---

## Abhängigkeiten

* [Sprachsteuerung über Alexa](../openHAB/Sprachsteuerung-Alexa.md)
* [Xbox-Controller und Xbox-Konsole](Xbox-Steuerung.md)

---

