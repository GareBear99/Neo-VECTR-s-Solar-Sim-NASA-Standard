# Neo-VECTR Solar Sim (NASA Standard)

**A low-weight 2D-engine (visually 3D) astronomy simulator that renders only proven celestial objects through a deterministic universe graph. Portable offline client with catalog-driven truth packs, orbit visualization, and scalable galaxy-to-planet navigation.**

> 🔐 **Built on [ARC-Core](https://github.com/GareBear99/ARC-Core)** — the authority / event / receipt kernel. Every celestial object, orbit derivation, and scale-tier transition is an ARC-Core-shaped event with provenance-checked receipts. The "NASA Standard" qualifier is enforced by ARC-Core's authority-over-provenance contract.

## 🔭 What it is

Neo-VECTR is a deterministic astronomy simulator built around **truth packs** — catalog-driven manifests of celestial objects whose provenance (observation catalog, identifier, instrument, epoch) is cryptographically verifiable. The simulator will not render an unverified object. If a truth pack says "this planet exists with these orbital parameters from this NASA-standard source," that claim is receipt-backed.

## 🌌 Design principles

- **NASA-standard ingestion** — only celestial objects traceable to a canonical catalog are accepted
- **Truth packs** — self-contained, SHA-256-verifiable bundles of astronomical data
- **Deterministic rendering** — two users with the same truth pack see the same universe bit-for-bit
- **Offline-first** — full operation without a network once truth packs are local
- **Low-weight** — 2D math core projected to 3D visually; runs on modest hardware
- **Scalable navigation** — galaxy → system → planet tier transitions without reloading

## 🏗️ Built on ARC-Core

Neo-VECTR uses the [**ARC-Core**](https://github.com/GareBear99/ARC-Core) authority kernel for:

| Neo-VECTR layer | ARC-Core pattern |
|---|---|
| Truth-pack receipt chain | Every celestial object has a provenance receipt citing its NASA-standard source |
| Event-sourced navigation | Camera, zoom, pan, scale-tier transitions are events; any viewport is reconstructable by replay |
| Authority over "proven" | The NASA-standard qualifier is an authority claim backed by proposal → evidence → receipt flow |
| Deterministic universe-graph replay | Universe graph is derived from truth packs + event log; fully reproducible |
| Offline verification | Receipts are SHA-256-addressable; packs verifiable without a server |
| Object identity | ARC-Core's entity-resolution pattern applied to celestial objects across truth packs |

## 🌐 The ARC Ecosystem

Neo-VECTR is one of several consumer applications built on the ARC governed-AI ecosystem. All share the same author and the same event-and-receipt doctrine:

- [**ARC-Core**](https://github.com/GareBear99/ARC-Core) — authority / event / receipt kernel *(backbone of this project)*
- [**arc-cognition-core**](https://github.com/GareBear99/arc-cognition-core) — model-growth lab
- [**ARC-Neuron-LLMBuilder**](https://github.com/GareBear99/ARC-Neuron-LLMBuilder) — governed AI build loop
- [**arc-language-module**](https://github.com/GareBear99/arc-language-module) — governed lexical truth
- [**omnibinary-runtime**](https://github.com/GareBear99/omnibinary-runtime) — binary mirror / runtime ledger
- [**Arc-RAR**](https://github.com/GareBear99/Arc-RAR) — archive / rollback bundles
- [**arc-lucifer-cleanroom-runtime**](https://github.com/GareBear99/arc-lucifer-cleanroom-runtime) — deterministic operator kernel

Companion consumer repos:

- [Seeded-Universe-Recreation-Engine](https://github.com/GareBear99/Seeded-Universe-Recreation-Engine) — the broader seeded-universe research project
- [Proto-Synth_Grid_Engine](https://github.com/GareBear99/Proto-Synth_Grid_Engine) — the Synth grid runtime
- [RiftAscent](https://github.com/GareBear99/RiftAscent) — action game on the same backbone
- [TizWildinEntertainmentHUB](https://github.com/GareBear99/TizWildinEntertainmentHUB) — audio plugin ecosystem

## 💖 Support

Single funding target for every ARC repo and every consumer application:

**[github.com/sponsors/GareBear99](https://github.com/sponsors/GareBear99)**

## 📜 License

See [LICENSE](./LICENSE).
