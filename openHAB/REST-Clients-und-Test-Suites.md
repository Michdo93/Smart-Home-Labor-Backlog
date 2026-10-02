# 🧪 openHAB REST-Clients und Test Suites

| | |
| --- | --- |
| **Status** | 🔍 Test ausstehend |
| **Priorität** | 🟠 Mittel |
| **Raum** | – |
| **Geeignet für** | Hiwi, Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Hinweise und Risiken](#hinweise-und-risiken)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Die eigenen REST-Clients und Test Suites für openHAB funktionieren in allen acht Sprachen mit der aktuellen openHAB-Version.

---

## Ist-Stand

* REST-Clients gibt es für **Python, JavaScript (Browser), Node.js, Java, C#, C++, C und Android/Kotlin**.
* Dazu passende **Test Suites** in denselben Sprachen sowie eine umfassende Python-Testbibliothek (`openhab-test-suite`).
* Die Clients werden im Labor genutzt, z. B. `js-openhab-rest-client` in den eigenen Dashboards und `python-openhab-rest-client` in Python-Projekten.
* Ältere Python-Bibliotheken (`python-openhab`, `python-openhab-crud` u. a.) sind durch `python-openhab-rest-client` abgelöst.

---

## Offene Aufgaben

* [ ] Alle Test Suites gegen die aktuelle openHAB-Version (openHAB 5) laufen lassen und Ergebnisse festhalten
* [ ] Abweichungen der REST API zwischen den Sprachvarianten angleichen (gleiche Funktionen, gleiche Namen)
* [ ] READMEs vereinheitlichen: Installation, Beispiel, unterstützte openHAB-Version
* [ ] Beschreibungen (About) und Topics der Repos auf GitHub ergänzen – bisher haben die meisten keine Beschreibung
* [ ] Prüfen, ob sich die Tests automatisiert ausführen lassen (CI, z. B. GitHub Actions gegen eine Test-Instanz)

---

## Hinweise und Risiken

* Hilfreich zum Testen: die Postman-Collections (`openhab_postman_templates`) und die statischen Beispiel-Items (`openhab_static_examples`).
* Grundlagen: [HTTP & REST](https://github.com/Michdo93/Informatik/blob/main/Netzwerk/HTTP%20%26%20REST.md)

---

## Repositories

* [python-openhab-rest-client](https://github.com/Michdo93/python-openhab-rest-client)
* [js-openhab-rest-client](https://github.com/Michdo93/js-openhab-rest-client)
* [nodejs-openhab-rest-client](https://github.com/Michdo93/nodejs-openhab-rest-client)
* [java-openhab-rest-client](https://github.com/Michdo93/java-openhab-rest-client)
* [csharp-openhab-rest-client](https://github.com/Michdo93/csharp-openhab-rest-client)
* [cpp-openhab-rest-client](https://github.com/Michdo93/cpp-openhab-rest-client)
* [c-openhab-rest-client](https://github.com/Michdo93/c-openhab-rest-client)
* [android-openhab-rest-client](https://github.com/Michdo93/android-openhab-rest-client)
* [openhab-test-suite](https://github.com/Michdo93/openhab-test-suite)
* [js-openhab-test-suite](https://github.com/Michdo93/js-openhab-test-suite)
* [nodejs-openhab-test-suite](https://github.com/Michdo93/nodejs-openhab-test-suite)
* [java-openhab-test-suite](https://github.com/Michdo93/java-openhab-test-suite)
* [csharp-openhab-test-suite](https://github.com/Michdo93/csharp-openhab-test-suite)
* [cpp-openhab-test-suite](https://github.com/Michdo93/cpp-openhab-test-suite)
* [c-openhab-test-suite](https://github.com/Michdo93/c-openhab-test-suite)
* [android-openhab-test-suite](https://github.com/Michdo93/android-openhab-test-suite)
* [openhab_postman_templates](https://github.com/Michdo93/openhab_postman_templates)
* [openhab_static_examples](https://github.com/Michdo93/openhab_static_examples)

---
