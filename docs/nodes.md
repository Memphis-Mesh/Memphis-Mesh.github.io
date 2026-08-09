---
sidebar_position: 2
---

# Nodes

## Medical District v3 MemphisMesh.com (medi)

[View !27ef756b on meshmap.net](https://meshmap.net/#670004587).

| [![Medical District Node](../static/img/med_district_1.jpg)](../static/img/med_district_1.jpg) | [![Medical District Installation](../static/img/med_district_2.jpg)](../static/img/med_district_2.jpg) |
| --- | --- |

This node provides great coverage in the medical district, downtown, and in the neighborhoods nearby. The closer you get to the I-240 loop, the more marginal performance becomes, though rooftop nodes can consistently get connections.

This node is configured for MediumFast preset and the default channel 0 with key `AQ==`.

### Hardware

This node is built using the guts of a NEBRA miner and is centered around a Raspberry Pi. It is powered via PoE and housed in a metal enclosure. The system features a 1W LoRa HAT for increased transmission power and includes a GPS module for location services, along with a SIM card slot for potential cellular connectivity.

A key component is the Airframes cavity filter, tuned to the MediumFast modem preset, which helps reduce interference and improve signal quality. The node is connected to a Diamond 900 MHz antenna, optimized for performance in the 900 MHz band, providing reliable omnidirectional coverage.

### Connectivity

This node is configured to uplink to the official Meshtastic MQTT server on the `msh/US/memphismesh.com` topic.

#### AI-enabled bot

This node also is setup running the [meshing-around](https://github.com/SpudGunMan/meshing-around) bot, which provides basic ping/pong, web search, weather alert, weather forecast, and ask AI capabilities powered by a local Ollama and the [Llama 3.2 3B model](https://ollama.com/library/llama3.2:3b). Try it out by DMing the node "cmd"!

## EXOpace Heltec V4 — Millington / North Memphis (`exo`)

[View !1ba349d8 on meshmap.net](https://meshmap.net/#463686104).

Fixed station node at Millington / north-Memphis area (~35.35°N, 89.84°W). Intended as a local-area participant on the Memphis MediumFast mesh and as an MQTT bridge into a home ground-station COP (observe-only).

This node is configured for MediumFast preset and the default channel 0 with key `AQ==`.

### Hardware

- **Radio:** Heltec Wireless Tracker / V4 expansion kit (ESP32-S3 + SX1262)
- **Role:** client / fixed position (facility Wi‑Fi when available; RF primary)
- **Location:** fixed position near Millington, TN (Memphis metro north)

### Connectivity

- Region: United States
- Preset: Medium Range — Fast
- Ok to MQTT: enabled
- Map Report: enabled
- Root topic: `msh/US/memphismesh.com` (Memphis Mesh uplink path)
- Local station also bridges status onto a private LAN MQTT for ops telemetry (not a public map source)

### Notes

- Node ID: `!1ba349d8` (decimal `463686104`)
- Short/long names may be updated in firmware as the station stabilizes
- Contact via GitHub: [Breaux-cpu](https://github.com/Breaux-cpu)
