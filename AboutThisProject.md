# Multiplayer Framework

- This project was made for my Computer Science A level code project, and took roughly 4 months.
- Most of the theory was learned from various online lectures and websites, the most prominent being Unite's lecture on their multiplayer system in the [Unity sample fps](https://www.youtube.com/watch?v=k6JTaFE7SYI)
- To learn the most useful skills from this project, I opted for a stubby frontend in favour of prioritising complete and highly complete and modular underlying systems. I also focused entirely on the UDP networking elements, so the handshaking is highly rudimentary.

## Features
- Functional basis for realtime multiplayer run on IPv4/UDP protocol for Unity C#
- 'Snapshot' based solution for packet loss/reordering/anomalous latency
- RTT measurement, snapshot buffers and introductory rollback system allows high time precision actions to be tracked accurately (e.g. shooting players with higher latencies).
- Delta based compression allows large numbers of server entities be tracked with minimal bandwidth usage.
- Asynchronous connection/disconnection process designed to handle connection errors gracefully
- Modular and adaptable: uses scriptable objects to allow the system to be integrated into a game without editing the networking scripts directly.

### [Demonstration video](https://www.youtube.com/watch?v=274FwnwSj10)
### [Itch.io link to builds](https://bobby-greathead.itch.io/multiplayer-system-builds)