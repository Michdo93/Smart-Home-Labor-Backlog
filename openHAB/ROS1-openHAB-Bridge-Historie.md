# 🤖 ROS-1-Bridge zwischen openHAB und ROS

| | |
| --- | --- |
| **Status** | ⚰️ Deprecated |
| **Priorität** | 🟢 Niedrig |
| **Raum** | – |
| **Geeignet für** | Alle (zum Nachlesen), Studienprojekt |

<!-- TOC -->
## Inhaltsverzeichnis

- [Ziel](#ziel)
- [Ist-Stand](#ist-stand)
- [Offene Aufgaben](#offene-aufgaben)
- [Abhängigkeiten](#abhängigkeiten)
- [Ideen und Szenarien](#ideen-und-szenarien)
- [Repositories](#repositories)
<!-- /TOC -->

## Ziel

Dokumentation der früheren Verbindung zwischen ROS 1 und openHAB – Grundlage für die geplante ROS-2-Anbindung.

---

## Ist-Stand

* **Bridges:** `openhab_bridge` (Bridge zwischen openHAB und ROS), `HABApp-ROS-openHAB-Bridge` (über HABApp), `iot_bridge` (ROS ↔ openHAB 3).
* **ROS-Pakete der Bridge:** `openhab_bridge_publisher` (Commands an openHAB), `openhab_bridge_subscriber` (States von openHAB), `openhab_bridge_image_listener` (Bild-Topics als Command an openHAB), `openhab_bridge_map_listener` (Karten-Topic als Bild an openHAB), `openhab_bridge_plot_publisher`, `openhab_bridge_plotter`, `openhab_msgs` (Nachrichtentypen).
* **Bildübertragung:** `base64_publisher`, `base64_subscriber`, `opencv_node` sowie die Python-Konvertierungen Bytes ↔ Base64 ↔ Bild (`Python-Bytes-Image-Conversion`, `Python-Base64-Image-Conversion`, `Python-Bytes-Image-To-Base64-Image-Conversion`, `Python-Base64-Image-To-Bytes-Image-Conversion`).
* **Nachfolger:** `ros2_openhab_ws` (ungetestet) sowie die browserbasierten ROS-Clients.

---

## Offene Aufgaben

* [ ] Erkenntnisse (Nachrichtentypen, Bildübertragung als Base64 an Image-Items) in die ROS-2-Anbindung übernehmen
* [ ] Repos kennzeichnen und archivieren

---

## Abhängigkeiten

* Nachfolger: [ROS 2 und openHAB](ROS2-Bridge.md)

---

## Ideen und Szenarien

* Die Idee, **Kamerabilder und Karten eines Roboters** als Image-Item in openHAB anzuzeigen, ist weiterhin interessant – z. B. die SLAM-Karte eines mobilen Roboters im Smart-Home-Dashboard.

---

## Repositories

* [openhab_bridge](https://github.com/Michdo93/openhab_bridge)
* [HABApp-ROS-openHAB-Bridge](https://github.com/Michdo93/HABApp-ROS-openHAB-Bridge)
* [iot_bridge](https://github.com/Michdo93/iot_bridge)
* [openhab_bridge_publisher](https://github.com/Michdo93/openhab_bridge_publisher)
* [openhab_bridge_subscriber](https://github.com/Michdo93/openhab_bridge_subscriber)
* [openhab_bridge_image_listener](https://github.com/Michdo93/openhab_bridge_image_listener)
* [openhab_bridge_map_listener](https://github.com/Michdo93/openhab_bridge_map_listener)
* [openhab_bridge_plot_publisher](https://github.com/Michdo93/openhab_bridge_plot_publisher)
* [openhab_bridge_plotter](https://github.com/Michdo93/openhab_bridge_plotter)
* [openhab_msgs](https://github.com/Michdo93/openhab_msgs)
* [base64_publisher](https://github.com/Michdo93/base64_publisher)
* [base64_subscriber](https://github.com/Michdo93/base64_subscriber)
* [opencv_node](https://github.com/Michdo93/opencv_node)
* [Python-Bytes-Image-Conversion](https://github.com/Michdo93/Python-Bytes-Image-Conversion)
* [Python-Base64-Image-Conversion](https://github.com/Michdo93/Python-Base64-Image-Conversion)
* [Python-Bytes-Image-To-Base64-Image-Conversion](https://github.com/Michdo93/Python-Bytes-Image-To-Base64-Image-Conversion)
* [Python-Base64-Image-To-Bytes-Image-Conversion](https://github.com/Michdo93/Python-Base64-Image-To-Bytes-Image-Conversion)

---
