# 🎮 Xbox-Controller und Xbox-Konsole

| | |
| --- | --- |
| **Status** | 🧪 Experiment |
| **Priorität** | 🟢 Niedrig |
| **Raum** | Multimedia |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

openHAB lässt sich mit einem Xbox-360-Controller bedienen; eine Xbox One lässt sich über openHAB ein- und ausschalten.

---

## Ist-Stand

* **xbox-360-openhab-controller:** Python-Code zur Steuerung von openHAB mit einem Xbox-360-Controller – noch zu integrieren. **Unklar ist, welcher Code am Ende der richtige war.**
* **openHAB-xbox-remote-power:** Xbox One per Exec Binding und dem Skript xbox-remote-power ein-/ausschalten – ungetestet.

---

## Offene Aufgaben

* [ ] Code-Stände im Repository sichten und den funktionierenden identifizieren; übrige entfernen oder in einen Ordner `archive/` verschieben
* [ ] Mit aktueller openHAB-Version testen
* [ ] Exec-Aufrufe in die Whitelist aufnehmen bzw. auf MQTT umstellen

---

## Repositories

* [xbox-360-openhab-controller](https://github.com/Michdo93/xbox-360-openhab-controller)
* [openHAB-xbox-remote-power](https://github.com/Michdo93/openHAB-xbox-remote-power)

---
