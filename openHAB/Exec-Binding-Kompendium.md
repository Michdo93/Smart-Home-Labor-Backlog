# 🧰 Exec-Binding-Kompendium

| | |
| --- | --- |
| **Status** | 💡 Idee |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Hiwi |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
<!-- /TOC -->

## Ziel

Eine Sammlung erprobter Einsatzmöglichkeiten des openHAB **Exec Bindings** – als Nachschlagewerk für Hiwis, was man damit (sicher) tun kann.

---

## Ist-Stand

* Idee aus einer Hiwi-Aufgabe: Das Exec Binding führt Kommandozeilenbefehle aus und eröffnet viele Möglichkeiten (SSH, sshpass, Wake-on-LAN, Systeminfos, Netzwerkscans, Anwendungen in diversen Sprachen starten).
* Es existieren umfangreiche Beispielskripte (ping, dnscheck, portcheck, speedtest, sslcert, uptime) und Dienst-/PID-Abfragen über `systemctl status` + `awk`.
* Der frühere Compendium-Ansatz (`Exec-Binding-and-Exec-Action-Compendium`) ist deprecated.

---

## Offene Aufgaben

* [ ] Beispiele sammeln und nach Themen ordnen (System, Netzwerk, Remote-Steuerung, Anwendungen)
* [ ] Jedes Beispiel mit **Whitelist-Eintrag** und Sicherheitshinweis versehen
* [ ] Veraltete/gefährliche Beispiele (pauschales `sudo %2$s`) aussortieren
* [ ] Als Markdown-Dokument statt als loses Repo pflegen (ggf. ins Kompendium Informatik)

---

## Hinweise und Risiken

* Statt alles über das Exec Binding zu lösen, ist für viele Fälle **MQTT** oder ein kleiner Dienst sauberer und sicherer.
* Grundlagen und Sicherheitsregeln: [Exec Binding & Remote-Ausführung](https://github.com/Michdo93/Informatik/blob/main/Best%20Practices/Exec-Binding%20%26%20Remote-Ausführung.md)

---

