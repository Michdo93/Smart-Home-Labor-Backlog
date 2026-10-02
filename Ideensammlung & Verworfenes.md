# 💭 Ideensammlung & Verworfenes

Aus früheren **Projektarbeiten** (Studierendengruppen, u. a. WiSe 22/23) stammt eine Reihe von Ideen. Viele davon sind inzwischen umgesetzt, in andere Vorhaben eingeflossen oder als eigene Repositories vorhanden. Dieses Dokument hält fest, **was daraus geworden ist** – und welche Ideen wir bewusst **nicht weiterverfolgen**. So sehen Hiwis und Praktikanten, was es gab, und können daran anknüpfen.

<!-- TOC -->
## Inhaltsverzeichnis

- [Als Vorhaben übernommen](#als-vorhaben-übernommen)
- [Bereits umgesetzt oder in anderen Vorhaben enthalten](#bereits-umgesetzt-oder-in-anderen-vorhaben-enthalten)
- [Bewusst nicht weiterverfolgt](#bewusst-nicht-weiterverfolgt)
- [Pepper und Nao: viele Repositories](#pepper-und-nao-viele-repositories)
<!-- /TOC -->

## Als Vorhaben übernommen

| Projektidee (WiSe 22/23) | Vorhaben | Status |
| --- | --- | --- |
| Android State Publisher | [Android State Publisher](Experimente/Android-State-Publisher.md) | 💡 Idee |
| Pflanzenüberwachung | [Pflanzenüberwachung](Experimente/Pflanzenueberwachung.md) | 💡 Idee |
| MySensors openHAB | [MySensors / DIY-Funksensoren](Experimente/MySensors-DIY-Sensoren.md) | 💡 Idee |
| REST API für Barcodes / QR-Codes | [Geräteerkennung per QR-Code](Experimente/QR-Code-Geraeteerkennung.md) | 💡 Idee |
| Wireless HDMI Matrix | [Wireless HDMI Matrix](Experimente/Wireless-HDMI-Matrix.md) | 💡 Idee |
| AR Smart Home Spiel | [Smart-Home-Krimi (AR-Spiel)](Demos/Smart-Home-Krimi-AR.md) | 💡 Idee |
| Nao/Pepper Controller (diverse Sprachen), behaviourManager | [Roboter-Controller in mehreren Sprachen](Experimente/Roboter-Controller-Sammlung.md) | 🔍 Test ausstehend |
| NAOqi Ethical Hacking | [Sicherheit der NAO-/Pepper-Roboter](Experimente/NAOqi-Sicherheit.md) | ⚰️ Deprecated |

## Bereits umgesetzt oder in anderen Vorhaben enthalten

| Projektidee | Wo es heute steht |
| --- | --- |
| MagicMirror MQTT | Teil des Smart-Home-Betriebs; der MagicMirror besitzt eine eigene Sprachsteuerung. Die Idee, **alle** openHAB-Commands einzutragen, ist mit mehreren tausend Items unverhältnismäßig – besser gezielt die wenigen benötigten. |
| Pepper/Nao Smart Home Integration | [Pepper-Concierge](Demos/Pepper-Concierge.md), [Roboter-Controller](Experimente/Roboter-Controller-Sammlung.md) |
| ROS roslibjs Turtlebot | [ROS 2 und openHAB](openHAB/ROS2-Bridge.md) bzw. die browserbasierten ROS-Clients |
| Hololens Smart Home Labor / Unity HTC Vive 3D-Labor | [VR und AR](Experimente/VR-AR.md); Idee [AR-Steuerung](https://github.com/Michdo93/SmartHome-Ideen) |
| Text Based Adventures / Geocaching mit Alexa | Spiel-/Lernideen rund um Alexa – nur umsetzbar, solange der openHAB-Alexa-Skill verfügbar ist (unsicher, siehe Idee „Sprachassistent“) |
| openHAB Doku anhand REST API | Durch das Kompendium [Informatik](https://github.com/Michdo93/Informatik) und die openHAB Design Patterns weitgehend abgedeckt |

---

## Bewusst nicht weiterverfolgt

Diese Ideen würde ich **streichen oder zurückstellen** – mit Begründung, damit die Überlegung nachvollziehbar bleibt:

| Idee | Einschätzung |
| --- | --- |
| **Airdroid Python** | Steuert Apps auf Android per Fernsteuerung über das Exec Binding. Fragiler Workaround (hängt an einer bestimmten App und deren Protokoll), Sicherheits- und Datenschutzfragen, geringer Mehrwert. Für Tablet-Steuerung sind Kiosk-Modus und MQTT der bessere Weg. |
| **Android x86 Touch Monitor Spiel** | Android-x86 in einer VirtualBox, um ein Touch-Spiel zu zeigen. Android-x86 wird kaum noch gepflegt; für ein Touchscreen-Spiel am Multitouchtisch ist eine normale Anwendung (Web/Unity) sinnvoller. |
| **Android MQTT Explorer** | Eigene Android-App als MQTT-Explorer. Dafür gibt es ausgereifte Werkzeuge (MQTT Explorer, MQTT.fx/MQTTX) und im Labor bereits den [MQTT Live Monitor](Infrastruktur/MQTT-Live-Monitor.md). Eigenentwicklung lohnt nicht. |
| **Android/Unity 3D Labor, Unity Touch Game** | Als eigenständige Themen zu vage. Sinnvoller gebündelt im [Smart-Home-Krimi](Demos/Smart-Home-Krimi-AR.md) bzw. in [VR und AR](Experimente/VR-AR.md). |
| **openHAB Cloud (eigene Instanz)** | Eine eigene openHAB-Cloud zu betreiben ist aufwendig und sicherheitskritisch. Nur nötig, wenn Fernzugriff oder der Alexa-Skill zwingend gebraucht werden – sonst über VPN oder Reverse Proxy lösen. |
| **Kühlschranküberwachung** | Als eigenes Thema zu dünn (nur Stichwort). Geht in allgemeiner Sensorik auf ([MySensors / DIY-Funksensoren](Experimente/MySensors-DIY-Sensoren.md): Tür-/Temperatursensor). |
| **Neato Botvac Hacking** | Reverse Engineering eines alten Saugroboters über die serielle Schnittstelle. Interessant als Lernobjekt, aber abhängig von genau diesem Altgerät und mit wenig Bezug zum restlichen Labor. Nur, wenn das Gerät vorhanden ist und jemand gezielt Interesse hat – dann über [Reverse Engineering](https://github.com/Michdo93/Informatik/blob/main/Workarounds%20%26%20Hacks/Reverse%20Engineering.md). |

> Diese Einschätzungen sind ein Vorschlag. Wenn jemand (Hiwi, Praktikum, Studienprojekt) besonderes Interesse an einem der Punkte hat, kann daraus trotzdem ein Vorhaben werden – der Lerneffekt zählt.

---

## Pepper und Nao: viele Repositories

Rund um die humanoiden Roboter gibt es sehr viele Repositories: die **SDKs** in mehreren Versionen (`pynaoqi-*`, `naoqi-sdk-*`, `java-naoqi-sdk-*`, `jnaoqi*`), **Beispiel-Controller** in verschiedenen Sprachen, **ROS-Pakete** und Hilfsmittel. Für den Überblick:

* Was im Betrieb zählt: [Pepper-Concierge](Demos/Pepper-Concierge.md), [Pepper-Selfie](Demos/Pepper-Selfie.md), [NAO Gym Instructor](Experimente/NAO-Gym-Instructor.md).
* Lern- und Beispielmaterial: [Roboter-Controller in mehreren Sprachen](Experimente/Roboter-Controller-Sammlung.md).
* Die SDK-Repos sind **Ablagen** der offiziellen SoftBank-SDKs (NAOqi) für verschiedene Betriebssysteme und Python-/Java-Versionen – sie werden nicht weiterentwickelt, sondern als Archiv vorgehalten, weil SoftBank sie nicht mehr anbietet.

---
