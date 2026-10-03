# 👤 Gesichter zählen (Multimediabox)

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Bad, Multimedia |
| **Geeignet für** | Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Eine Kamera an einer Windows-/Linux-Box zählt Gesichter bzw. Personen und meldet das an openHAB – verwandt mit dem People Counter, aber kamerabasiert auf einem PC.

---

## Ist-Stand

* Frühere Projektidee mit einer „Multimediabox“ (PC), auf der eine Gesichtserkennung lief; Steuerung des PCs über SSH/Wake-on-LAN.
* Überschneidet sich stark mit dem [People Counter](../Geräteintegration/People-Counter.md) (Tiefenkamera) – hier eher Webcam + Gesichtserkennung.

---

## Offene Aufgaben

* [ ] Klären, ob diese Variante neben dem People Counter nötig ist
* [ ] Falls ja: aktuelle Gesichtserkennung (OpenCV) nutzen, Ergebnis per MQTT an openHAB
* [ ] Datenschutz klären: Gesichtserkennung ist personenbezogen – Zweck, Speicherung, Einwilligung

---

## Abhängigkeiten

* [People Counter](../Geräteintegration/People-Counter.md)

---

## Hinweise und Risiken

* **Datenschutz:** Gesichtserkennung erfasst personenbezogene/biometrische Daten. Vor dem Einsatz Zulässigkeit und Hinweispflichten klären.

---

