# 📺 Wireless HDMI Matrix

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Multimedia, Konferenz |
| **Geeignet für** | Studienprojekt, Abschlussarbeit |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Eine HDMI-Matrix schaltet Quellen (Konsolen, Kodi, Laptops, HTC Vive) auf Ausgaben (Beamer, Fernseher, Monitore) – kabellos über HDMI-Transmitter/Receiver, per openHAB steuerbar, mit zusätzlichem RTMP-Stream ins Netzwerk.

---

## Ist-Stand

* Ausführlich ausgearbeitete Projektidee (WiSe 22/23) mit Gerätebestand, Materialliste und Kostenschätzung (grob 2000–3000 €).
* Die Matrix wird per **RS232** (USB-zu-RS232) von einem Raspberry Pi gesteuert; openHAB greift per Exec Binding und SSH zu.
* Ein Raspberry Pi erzeugt aus den HDMI-Ausgängen per Capture-Card einen **RTMP-Stream**, den jedes Gerät im Netz empfangen kann.

---

## Offene Aufgaben

* [ ] Entscheiden, ob und in welchem Umfang beschafft wird (4×4 vs. 8×8, Kosten)
* [ ] RS232-Steuerung der Matrix mit PySerial umsetzen
* [ ] openHAB-Items und Regel „Ausgangszustand“ (Standard: Konferenztisch → Beamer)
* [ ] RTMP-Stream aufsetzen und testen
* [ ] Optional Sprachsteuerung („Playstation auf Beamer übertragen“)

---

## Hinweise und Risiken

* Hoher Hardware- und Kostenaufwand – vor dem Start Nutzen und Budget abwägen.
* RS232-Steuerung ähnlich wie beim [BenQ-Beamer](../Geräteintegration/BenQ-MH856UST.md).
* Verwandt: [WebTV](WebTV.md) nutzt ebenfalls Streams für die Anzeige.

---

