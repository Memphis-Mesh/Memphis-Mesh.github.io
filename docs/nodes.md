# Nodes

## Medical District memphisme.sh v2 (👀)

[View !67812a87 on meshmap.net](https://meshmap.net/#1736518279).

This node provides good coverage in the medical district, downtown, and in the neighborhoods nearby. The closer you get to the I-240 loop, the more marginal performance becomes, though rooftop nodes can consistently get connections.

This node is configured for LongFast preset and the default channel 0 with key `AQ==`.

### Hardware

This node is a [MeshAdv Pi Hat](https://github.com/chrismyers2000/MeshAdv-Pi-Hat) running on top of a Raspberry Pi 5B. The node has a [Callboost 915 MHz Band Pass Filter](https://www.aliexpress.com/i/3256804282645306.html?gatewayAdapt=4itemAdapt) to help reduce adjacent interference, which this site has plenty of between cell, public safety, and hospital paging systems.

The node is inside a 2 post rack adjacent to amateur radio equipment from HamWAN Memphis Metro and Tri-State Repeater Association. From the cabinet to the tower, the site is fed with 30 ft LMR-300. The antenna is a [MikroTik 915 MHz 5.2 dBi antenna](https://mikrotik.com/product/915_omni_antenna).

### Connectivity

This node is configured to uplink to the official Meshtastic MQTT server on the `us/memphisme.sh` topic.

#### AI-enabled bot

This node also is setup running the [meshing-around](https://github.com/SpudGunMan/meshing-around) bot, which provides basic ping/pong, web search, weather alert, weather forecast, and ask AI capabilities powered by a local Ollama and the [Llama 3.2 3B model](https://ollama.com/library/llama3.2:3b). Try it out by DMing the node "cmd"!
