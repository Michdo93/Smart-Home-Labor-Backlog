# 🌅 Morgenroutine

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🔴 Hoch |
| **Raum** | Mehrere Räume |
| **Geeignet für** | Labormitarbeitende |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Ideen und Szenarien](#ideen-und-szenarien)
<!-- /TOC -->

## Ziel

Die Morgenroutine ist eine der zentralen Labor-Demos. Sie soll zeitlich korrekt und zuverlässig ablaufen – langfristig als **Python-3-Rule**, mit einer funktionierenden **DSL-Rule** als Rückfallebene.

---

## Ist-Stand

* Die Morgenroutine lief früher als **Jython-2.7-Rule** und als **DSL-Rule** fehlerfrei.
* Die Migration auf **Python 3 Scripting** ist noch nicht abgeschlossen: Die Routine läuft **zeitlich nicht korrekt** ab.
* Vermutete Ursache: Nebenläufigkeit und Threads werden in Python 3 Scripting anders behandelt. Unklar ist, ob nur `sleep`-Aufrufe das Problem sind oder Codeabschnitte, die bewusst blockierend nacheinander ausgeführt werden sollen.
* Eine überarbeitete Python-3-Version (auf Basis der funktionierenden Jython- und DSL-Rule) liegt vor und muss getestet werden.

---

## Offene Aufgaben

* [ ] Überarbeitete Python-3-Rule testen
* [ ] Funktionierende DSL-Rule als **Notfallplan** bereithalten und testen
* [ ] Bei Erfolg: Ursache des Timing-Problems dokumentieren (für andere Rules mit Wartezeiten)
* [ ] Newspaper Projector in den Ablauf integrieren (siehe unten)
* [ ] Rollladen-Ablauf anpassen: erst hochfahren, wenn die Person im Bad ist

---

## Abhängigkeiten

* [Newspaper Projector](../Geräteintegration/Newspaper-Projector.md)
* [Rules-Migration](../openHAB/Rules-Migration.md)

---

## Hinweise und Risiken

* Der Wechsel auf Jython bzw. Python 3 hatte zwei Gründe: mehr Flexibilität und schnelleres Booten von openHAB, weil Python-Rules parallel geladen werden.
* Eine einzelne DSL-Rule-Datei parallel zu den Python-Rules stört das restliche System nicht. Etwas mehr RAM und eine längere Boot-Zeit sind vertretbar.

---

## Ideen und Szenarien

* **Newspaper Projector:** einschalten, sobald der Wecker per Wandtaster quittiert wird; ausschalten, sobald die Person im Bad ist.
* Der Rollladen bleibt geschlossen, solange die Zeitung projiziert wird (bessere Sichtbarkeit), und fährt hoch, sobald die Person im Bad ist.
* Wie präzise der Wechsel klappt, hängt vom Bewegungsmelder ab.

---

