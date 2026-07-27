## Jan Kučera

Systems and protocol engineer in Ostrava, Czechia. I build the layer underneath — consensus,
cryptography, storage engines, P2P networking — and the tooling that keeps large estates observable.
Twelve years of Python, increasingly Rust.

### Protocols

**[bismuth](https://github.com/hclivess/bismuth)** — the first blockchain protocol and platform
written from scratch in Python. In development since 2015, fair-launched on 1 May 2017 with no ICO
and no premine, in continuous production ever since. Full node stack: P2P networking, SQLite ledger
with schema migrations, block and transaction validation, mining, wallets, explorers, REST APIs —
plus the Hypernode second layer and the "Crystals" plugin system behind on-chain tokens, aliases,
a DEX, and cross-chain bridges to Ethereum and BSC.

**[nado](https://github.com/hclivess/nado)** — a phone-mineable, fair-launch, post-quantum chain.
Proof-of-work's hash race is replaced by a deterministic, beacon-keyed weighted draw: one hash
decides each block's producer, so faster hardware confers no advantage and there is nothing to
grind. ML-DSA-44 (NIST FIPS 204) signatures in pure Python with a byte-compatible JavaScript
implementation, so a zero-install browser page — wallet, miner, explorer, and alias manager at once —
reproduces every address and transaction ID bit-for-bit. A STARK-proven execution layer
(field-native zkVM) carries on-chain games, shielded transfers, and end-to-end-encrypted messaging.

> **Testnet-stage alpha — not mainnet-launched.** The alphanet rerolls as consensus changes land.
> Run it at your own risk; don't secure value of consequence with it yet.

### Research

- Kučera, J., Hovland, G. — [Tail Removal Block Validation: Implementation and Analysis](https://doi.org/10.4173/mic.2018.3.1).
  *Modeling, Identification and Control* 39(3), 2018. First author; deployed to the live Bismuth
  mainnet, cutting block times over 190 s from 5.4% to under 1% of blocks.
- Hovland, G., Kučera, J. — [Nonlinear Feedback Control and Stability Analysis of a Proof-of-Work Blockchain](https://doi.org/10.4173/mic.2017.4.1).
  *MIC* 38(4), 2017. Cited in IBM patent US 10,880,073.

### Tools

| | |
|---|---|
| [speech-splitter](https://github.com/hclivess/speech-splitter) | Whisper + YAMNet pipeline turning raw recordings into Hugging Face-ready TTS training datasets. Produced the Czech corpora behind the [Chatterbox-TTS-Czech](https://huggingface.co/Thomcles/Chatterbox-TTS-Czech) fine-tune. |
| [ollama-batch-processor](https://github.com/hclivess/ollama-batch-processor) | Qt GUI for batch LLM pipelines — translation, chunking, chained operations. |
| [videer](https://github.com/hclivess/videer) | FFmpeg/AviSynth+ encoding GUI with QTGMC deinterlacing and CUDA. |
| [dynatrace-mass-management](https://github.com/hclivess/dynatrace-mass-management) | Self-hosted Tornado portal for bulk operations across many Dynatrace tenants via the API. |
| [screen-monitor](https://github.com/hclivess/screen-monitor) · [mandatum](https://github.com/hclivess/mandatum) | Rust client/server systems for Windows fleets: live screen monitoring and remote task execution. |
| [sshauto](https://github.com/hclivess/sshauto) | Automate repetitive SSH tasks — a lightweight alternative to Ansible. |

### Running in production

- [firmostat.cz](https://firmostat.cz) — Czech companies database aggregating 1M+ records from ARES
  and the Commercial & Insolvency Registers into PostgreSQL; scrapers plus REST API.
- [slopinky.cz](https://slopinky.cz) — auto-translated Czech current-events encyclopedia, built on an
  RSS/Trends ingestion and headless-Claude editorial pipeline (draft / review / translate).

### Elsewhere

Eight-plus years of enterprise observability engineering for global manufacturing and government
clients — Dynatrace, CheckMK, Nimsoft/Ekara across estates of roughly 15,000 hosts.

[bismuth.cz](https://bismuth.cz) · [nadochain.com](https://nadochain.com) · [LinkedIn](https://www.linkedin.com/in/kucerjan) · kucera@protonmail.com
