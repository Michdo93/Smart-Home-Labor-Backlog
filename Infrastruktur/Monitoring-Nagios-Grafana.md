# 📊 Monitoring (Nagios & Grafana)

| | |
| --- | --- |
| **Status** | 🚧 In Arbeit |
| **Priorität** | 🟠 Mittel |
| **Raum** | Server |
| **Geeignet für** | Hiwi, Praxissemester |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Das Labor wird durchgehend überwacht: **Nagios/Icinga** prüft Dienste, Hosts und Netzwerk (läuft oder nicht), **Grafana** stellt Messwerte und Verläufe dar (Zustände, Auslastung). Störungen fallen auf, bevor eine Demo scheitert.

---

## Ist-Stand

* Grafana ist installiert und getestet: Logs über **Loki** (nur aktuelle Logdatei) und Messwerte über die **openHAB Persistence** (Datenbank).
* Grafana-Dashboards lassen sich per Webview in openHAB einbetten.
* Für dauerhafte Logs wurde früher der `OpenHAB-LogSaver` genutzt (schreibt die letzte Logzeile in eine Datenbank) – inzwischen **deprecated**; besser über Loki mit Persistenz bzw. eine Zeitreihen-/Log-Datenbank.
* Netzwerk-/Dienst-Monitoring mit **Nagios** (NRPE, viele `check_*`-Plugins) war ein Projektthema; openHAB kann über das Plugin `check_openhab` Item-States an Nagios liefern, umgekehrt Nagios-Checks über das Exec Binding in openHAB anzeigen.
* Zusätzlich möglich: openHAB-Bindings **network**, **systeminfo**, **snmp**, **ntp** für ein leichtgewichtiges Monitoring ohne Nagios.

---

## Offene Aufgaben

* [ ] Entscheiden, was womit überwacht wird: **Grafana** für Messwerte/Verläufe, **Nagios/Icinga** für Dienst-/Host-Zustände (die beiden ergänzen sich)
* [ ] Grafana als Container in der Docker-VM betreiben, Datenquellen: openHAB-Persistence (InfluxDB) und Loki
* [ ] Dashboards je Raum/Thema anlegen; wichtige in openHAB einbetten
* [ ] Nagios/Icinga aufsetzen (ggf. als Container) und die wichtigsten Checks definieren (Dienste, Platten, Erreichbarkeit, Zertifikatsablauf)
* [ ] Alarmierung einrichten (E-Mail/Push), Schwellwerte sinnvoll setzen
* [ ] Exec-Checks auf die Whitelist `misc/exec.whitelist` beschränken und absichern

---

## Abhängigkeiten

* [Container in der Docker-VM](Docker-VM.md)

---

## Hinweise und Risiken

* Der frühere Nagios-Ansatz nutzte eine sehr umfangreiche Exec-Whitelist mit vielen `check_*`-Kommandos inkl. `sudo` – das ist ein Risiko. Besser **NRPE** auf den Zielsystemen statt Exec-Kommandos mit `sudo` über openHAB.
* Grundlagen: [Zeitreihen & openHAB Persistence](https://github.com/Michdo93/Informatik/blob/main/Datenbanken/Zeitreihen%20%26%20openHAB%20Persistence.md), [Monitoring & Alerting](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/Monitoring%20%26%20Alerting.md), [Whitelist & Blacklist](https://github.com/Michdo93/Informatik/blob/main/Zugriffskontrolle/Whitelist%20%26%20Blacklist.md)

---

## Repositories

* [MQTT-Live-Monitor](https://github.com/Michdo93/MQTT-Live-Monitor)

---
