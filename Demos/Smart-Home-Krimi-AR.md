# 🕵️ Smart-Home-Krimi (AR-Spiel)

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Alle Räume |
| **Geeignet für** | Studienprojekt, Abschlussarbeit |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Ein interaktives Krimi-/Escape-Erlebnis im Labor: Mit HoloLens und Unity löst man einen „Mordfall“, befragt die Roboter Pepper und Nao sowie Alexa und bedient dabei echte Smart-Home-Geräte über openHAB.

---

## Ist-Stand

* Sehr ausführlich ausgearbeitete Projektidee (WiSe 22/23): virtuelle Hinweise in AR, befragbare Roboter mit Behaviours, Alexa mit „Fake-Logtagebuch“, Spielfortschritt über openHAB-Switches.
* Baut auf mehreren anderen Themen auf: AR/HoloLens, Roboter-Steuerung, Sprachassistenten, Spielelogik.
* Verwandt mit dem bereits vorhandenen [Escape-Room-Workshop](Escape-Room-Workshop.md) (dort Node-RED).

---

## Offene Aufgaben

* [ ] Umfang festlegen – als Abschlussarbeit oder mehrteiliges Studienprojekt; eine kleine Demo-Variante zuerst
* [ ] Unity-Anwendung (HoloLens) mit MQTT-Anbindung an openHAB
* [ ] Roboter-Behaviours für Befragungen; Alexa-Trigger und TTS-Antworten
* [ ] Spielzustände als openHAB-Switches, angepasste Regeln im Spielmodus

---

## Abhängigkeiten

* [Pepper-Concierge](Pepper-Concierge.md)
* [Escape-Room-Workshop](Escape-Room-Workshop.md)

---

## Hinweise und Risiken

* Großer Umfang – sinnvoll in Teilprojekte zerlegen (AR, Roboter, Alexa, Spiellogik).
* Könnte als eigenständige Idee ins Repo [SmartHome-Ideen](https://github.com/Michdo93/SmartHome-Ideen) wandern.

---

