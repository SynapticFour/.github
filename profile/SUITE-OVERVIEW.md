# Related public repositories

These public repositories are maintained by Synaptic Four and are designed to work together. Each keeps its own version and license. You compose them by pin: declare which tag or SHA of another repository you use.

**Released join:** the tables below describe tagged and SHA pins. A product `main` may be ahead of the join.

## Maturity labels

| Label | Meaning |
|-------|---------|
| **Active (beta)** | Maintained. CI is a technical signal, not GA4GH certification. |
| **Early access** | Public source; ready to try. Expect gaps. |
| **Reference / demo** | Local walkthrough of a pinned product so you can see it run. |

## The ten repositories

| Repository | Role | License | Maturity |
|------------|------|---------|----------|
| [Ferrum](https://github.com/SynapticFour/Ferrum) | GA4GH data/compute plane (DRS, WES, TES, TRS, Beacon v2, htsget, Passports, Crypt4GH) | BUSL-1.1 | Active (beta) |
| [ga4gh-infra](https://github.com/SynapticFour/ga4gh-infra) | Identity plane (OIDC broker, Passports/visas, DUO, ADS, service registry). **Compose is the supported deploy.** Helm is a sketch. | Apache-2.0 | Active (beta) — Compose path |
| [Solum](https://github.com/SynapticFour/Solum) | Clinical compliance layer (consent, audit chain, FHIR interchange, field crypto) | BUSL-1.1 | Early access |
| [BioResearch Assistant](https://github.com/SynapticFour/bioresearch-assistant) | Researcher workbench (literature, phenopackets, local DRS/WES, optional HTTP joins) | BUSL-1.1 | Early access |
| [Ferrum Lab Kit](https://github.com/SynapticFour/Ferrum-Lab-Kit) | Generate Compose / Helm / systemd around a SHA-pinned Ferrum image | BUSL-1.1 | Early access |
| [ferrum-meta](https://github.com/SynapticFour/ferrum-meta) | LinkML schema and archive profiles. `export` copies a committed fixture (`shutil.copyfile`). | Apache-2.0 | Early access |
| [HELIOS](https://github.com/SynapticFour/HELIOS) | Signed pipeline and audit evidence. Reads export JSON from disk. Distinct from [Helix](https://github.com/SynapticFour/Helix) / [HelixTest](https://github.com/SynapticFour/HelixTest) (API checks). | Apache-2.0 | Early access |
| [Ferrum-GA4GH-Demo](https://github.com/SynapticFour/Ferrum-GA4GH-Demo) | Laptop pipeline walkthrough of tagged Ferrum (DRS / WES / TES) | Apache-2.0 | Reference / demo |
| [Solum-Demo](https://github.com/SynapticFour/Solum-Demo) | Local Stage-1 walkthrough of tagged Solum (`dev-local.toml`) | Apache-2.0 | Reference / demo |
| [SynapticFour-Showcase](https://github.com/SynapticFour/SynapticFour-Showcase) | Evidence pack and pin checkout across products | Apache-2.0 | Reference / demo |

Related: [HelixTest](https://github.com/SynapticFour/HelixTest) — GA4GH OpenAPI tests against a running target. A green job is a technical signal, not GA4GH certification.

Evaluator entry points live in `docs/FOR-EVALUATORS.md` on Ferrum, ga4gh-infra, Solum, BioResearch Assistant, HELIOS, and Helix.

## Also public

These repositories are public and are **not** part of the ten-repo released join.

| Repository | Role | Notes |
|------------|------|-------|
| [Helix](https://github.com/SynapticFour/Helix) | VERIFY CLI. HelixTest becoming a standalone product. Conformance, security behaviour, benchmark. Distinct from HELIOS. | Early access |
| [helix-action](https://github.com/SynapticFour/helix-action) | GitHub Action around `helix verify` | Wrapper |
| [helixtest-action](https://github.com/SynapticFour/helixtest-action) | GitHub Action around HelixTest release binaries (default **v0.1.3**) | Wrapper |
| [Open-Source-GA4GH-Stack](https://github.com/SynapticFour/Open-Source-GA4GH-Stack) | Upstream OSS Compose/Helm kit, for comparison with Lab Kit | Teaching / comparison |
| [gatk-rs](https://github.com/SynapticFour/gatk-rs) | Independent GATK4 HaplotypeCaller spine research | Research / Alpha |
| [technical-reports](https://github.com/SynapticFour/technical-reports) | SF-TR series | Publications |
| [S4MP](https://github.com/SynapticFour/S4MP) | Heuristic Java↔Rust port maps. `certify` records review policy, not semantic equivalence. | Tooling |
| [cognitive-landscape-research-programme](https://github.com/SynapticFour/cognitive-landscape-research-programme) | Research programme constitution. Not diagnostic. | Research |
| [cognitive-landscape-model](https://github.com/SynapticFour/cognitive-landscape-model) | CLM modelling library. Not diagnostic. | Research |
| [perceptual-cognitive-mapping-system](https://github.com/SynapticFour/perceptual-cognitive-mapping-system) | PCMS research instrument. Live demo. Not diagnostic. | Research |
| [Synaptic-Core-Demo](https://github.com/SynapticFour/Synaptic-Core-Demo) | Laptop harness against Synaptic Core | Demo / harness |
| [sc-specs](https://github.com/SynapticFour/sc-specs) | OpenAPI/AsyncAPI text for Synaptic Core | Specs |
| [sc-transport](https://github.com/SynapticFour/sc-transport) | Transport crates for Synaptic Core | Library |
| [SecureCollab](https://github.com/SynapticFour/SecureCollab) | Multi-party statistics on homomorphically encrypted datasets | Research |
| [vibecheck](https://github.com/SynapticFour/vibecheck) | Local scanner for AI-generated codebases | Tooling |
| [.github](https://github.com/SynapticFour/.github) | This organisation profile | Map you are reading |

Questions: [contact@synapticfour.com](mailto:contact@synapticfour.com).
