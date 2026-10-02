# 📡 MySensors / DIY-Funksensoren

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Studienprojekt, Abschlussarbeit |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Ideen und Szenarien](#ideen-und-szenarien)
<!-- /TOC -->

## Ziel

Mit dem Open-Source-Framework **MySensors** günstige, selbstgebaute Funksensoren (Arduino/ESP + nRF24L01/RFM69) aufbauen und über ein Gateway in openHAB einbinden.

---

## Ist-Stand

* Projektidee (WiSe 22/23); bisher nur Materialsammlung, kein Repository.
* MySensors unterstützt viele Sensortypen (Feuchte, Temperatur, Bewegung, Tür, Licht …) und wird über ein serielles, Ethernet-, ESP8266- oder MQTT-Gateway angebunden.
* Überschneidet sich mit den vorhandenen ESP32-Experimenten – hier geht es um ein **einheitliches Framework** für viele günstige Sensoren.

---

## Offene Aufgaben

* [ ] Entscheiden, ob MySensors oder direkt ESP + MQTT (z. B. ESPHome) das Mittel der Wahl ist
* [ ] Ein Gateway aufbauen (bevorzugt MQTT-Gateway)
* [ ] Ein bis zwei Beispielsensoren bauen und in openHAB einbinden
* [ ] Als Baukasten dokumentieren, damit weitere Sensoren leicht ergänzt werden können

---

## Ideen und Szenarien

* Grundlage für die [Pflanzenüberwachung](Pflanzenueberwachung.md) und weitere günstige Sensoren im Labor.

---

