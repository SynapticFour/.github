# Related public repositories

The map with the public status labels is [profile/README.md](README.md). This page keeps the longer role notes. GA4GH, used below, is a set of shared interfaces for genomic and health data. A product `main` may be ahead of a pin. A reader composes repositories by pin: the tag or the commit a pin file names. Each repository keeps its own version and its own licence.

## Stranger path (~30 min)

Not a certificate and not a clinical pilot. Commands, the expected Helix line, and the `:18080` versus `:8080` difference: [org profile](README.md#try-it).

1. Helix `make fetch`, then `make prove`, then `make verify-drs`. No Docker. The sibling HelixTest checkout is the SHA in Helix `VERSIONS.lock`, not a tag used in place of that SHA.
2. [Ferrum-GA4GH-Demo](https://github.com/SynapticFour/Ferrum-GA4GH-Demo) `make up` (that is `./run`). Docker. Ferrum pin v0.3.2. That pin is not Ferrum's default branch.
3. Optional: HelixTest tag v0.1.3 against `http://127.0.0.1:18080`. That tag is not HelixTest's default branch. Longer pack: [Showcase](https://github.com/SynapticFour/SynapticFour-Showcase) `make up`.

## Status words

The public status words are Prototype, Early use, In use, and Independently reviewed. Active (beta) and Early access are the same stage as Early use. They are not a second label beside it. Reference / demo describes a walkthrough. It is not a public status label. When the claims registry has no stage, the profile table leaves the status empty.

The phrases below are the older words this file used. They stay so a reader of an older copy can match them.

| Older phrase | What it meant here |
| --- | --- |
| **Active (beta)** | Maintained. CI is a technical signal, not GA4GH certification. The public label for that stage is Early use, where a claim records it. |
| **Early access** | Public source; ready to try. Expect gaps. The public label for that stage is Early use, where a claim records it. |
| **Reference / demo** | Local walkthrough of a pinned product so a person can see it run. Not a public status label. |

## The ten repositories

| Repository | Role | Licence | Public status |
| --- | --- | --- | --- |
| [Ferrum](https://github.com/SynapticFour/Ferrum) | GA4GH data and compute plane (DRS, WES, TES, TRS, Beacon v2, htsget, Crypt4GH). Passports are not one of those seven. | BUSL-1.1 | Early use |
| [ga4gh-infra](https://github.com/SynapticFour/ga4gh-infra) | Identity plane (OIDC broker, Passports/visas, DUO, ADS, service registry). **Compose is the supported deploy.** Helm is a sketch. | Apache-2.0 | Early use |
| [Solum](https://github.com/SynapticFour/Solum) | Clinical compliance layer (consent, audit chain, FHIR interchange, field crypto) | BUSL-1.1 | Early use |
| [BioResearch Assistant](https://github.com/SynapticFour/bioresearch-assistant) | Researcher workbench (literature, phenopackets, local DRS/WES, optional HTTP joins) | BUSL-1.1 | Early use |
| [Ferrum Lab Kit](https://github.com/SynapticFour/Ferrum-Lab-Kit) | Generate Compose / Helm / systemd around a SHA-pinned Ferrum image | BUSL-1.1 | Early use |
| [ferrum-meta](https://github.com/SynapticFour/ferrum-meta) | LinkML schema and archive profiles. `export` copies a committed fixture (`shutil.copyfile`). | Apache-2.0 |  |
| [HELIOS](https://github.com/SynapticFour/HELIOS) | Signed pipeline and audit evidence. Reads export JSON from disk. Distinct from [Helix](https://github.com/SynapticFour/Helix) / [HelixTest](https://github.com/SynapticFour/HelixTest) (API checks). | Apache-2.0 | Early use |
| [Ferrum-GA4GH-Demo](https://github.com/SynapticFour/Ferrum-GA4GH-Demo) | Laptop pipeline walkthrough of tagged Ferrum (DRS / WES / TES) | Apache-2.0 |  |
| [Solum-Demo](https://github.com/SynapticFour/Solum-Demo) | Local Stage-1 walkthrough of tagged Solum (`dev-local.toml`) | Apache-2.0 |  |
| [SynapticFour-Showcase](https://github.com/SynapticFour/SynapticFour-Showcase) | Evidence pack and pin checkout across products | Apache-2.0 |  |

[HelixTest](https://github.com/SynapticFour/HelixTest) already runs. It is the GA4GH interface check against a running target. The public label is Early use. A green job is a technical signal, not GA4GH certification. Helix is that suite as the `helix` command.

Evaluator entry points live in `docs/FOR-EVALUATORS.md` on Ferrum, ga4gh-infra, Solum, BioResearch Assistant, HELIOS, and Helix.

## Also public

These repositories are public and are not part of the ten-repository pin join above. The profile table lists them with the others. An empty public status means the claims registry has no stage.

The service named in sc-specs, sc-transport, and Synaptic-Core-Demo is not a public repository. This page does not link it.

| Repository | Role | Notes |
| --- | --- | --- |
| [Helix](https://github.com/SynapticFour/Helix) | VERIFY CLI. HelixTest already runs; this repository is that suite as a standalone command. Conformance, security behaviour, benchmark. Distinct from HELIOS. | No public status is recorded |
| [helix-action](https://github.com/SynapticFour/helix-action) | GitHub Action around `helix verify` | No public status is recorded |
| [helixtest-action](https://github.com/SynapticFour/helixtest-action) | GitHub Action around HelixTest release binaries (default **v0.1.3**) | That tag is not HelixTest's default branch. No public status is recorded |
| [Open-Source-GA4GH-Stack](https://github.com/SynapticFour/Open-Source-GA4GH-Stack) | Upstream OSS Compose/Helm kit, for comparison with Lab Kit | No public status is recorded |
| [gatk-rs](https://github.com/SynapticFour/gatk-rs) | Independent GATK 4 HaplotypeCaller spine: a Rust caller for germline short variants | No public status is recorded. A version number is not a status |
| [technical-reports](https://github.com/SynapticFour/technical-reports) | SF-TR series | Publications. No public status is recorded |
| [S4MP](https://github.com/SynapticFour/S4MP) | Heuristic Java-to-Rust port maps. `certify` records a confirmed review, not semantic equivalence. | No public status is recorded |
| [cognitive-landscape-research-programme](https://github.com/SynapticFour/cognitive-landscape-research-programme) | Research programme constitution. Not diagnostic. | No public status is recorded |
| [cognitive-landscape-model](https://github.com/SynapticFour/cognitive-landscape-model) | CLM modelling library. Not diagnostic. | No public status is recorded |
| [perceptual-cognitive-mapping-system](https://github.com/SynapticFour/perceptual-cognitive-mapping-system) | PCMS research instrument. Public questionnaire. Not diagnostic. | No public status is recorded |
| [Synaptic-Core-Demo](https://github.com/SynapticFour/Synaptic-Core-Demo) | Laptop harness. The service it talks to is not a public repository. Compute is a busybox echo, not a scientific pipeline. | No public status is recorded |
| [sc-specs](https://github.com/SynapticFour/sc-specs) | API specifications for object identity, tasks, workflows, discovery, and provenance | The service is not a public repository |
| [sc-transport](https://github.com/SynapticFour/sc-transport) | Transport crates for telemetry of that same service | The service is not a public repository |
| [SecureCollab](https://github.com/SynapticFour/SecureCollab) | A proof piece: multi-party statistics on homomorphically encrypted datasets. Not for patient data. | No public status is recorded |
| [vibecheck](https://github.com/SynapticFour/vibecheck) | Local scan of a codebase. The scan stays on the machine that runs it. | No public status is recorded |
| [.github](https://github.com/SynapticFour/.github) | This organisation profile | The map is `profile/README.md` |

Questions: [contact@synapticfour.com](mailto:contact@synapticfour.com).
