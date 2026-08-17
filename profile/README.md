# Synaptic Four

Customer-sovereign infrastructure for genomics and clinical research. Stuttgart. Independent products, pin-based composition — not a bundle SKU.

**Start here:** [Ferrum / GA4GH suite overview](https://github.com/SynapticFour/Ferrum/blob/main/docs/SUITE-OVERVIEW.md) · [Products](https://synapticfour.com/products) · [Ferrum getting started](https://github.com/SynapticFour/Ferrum/blob/main/docs/GETTING-STARTED.md) (`make prove`, then `make eval`)

## GA4GH suite (ten public repositories)

These repositories can be composed. Each keeps its own version and license. Suite consumers pin Ferrum **v0.3.2**. A green laptop run against that pin is not proof of Ferrum `main`.

| Repository | Role | Maturity |
|------------|------|----------|
| [Ferrum](https://github.com/SynapticFour/Ferrum) | GA4GH data/compute plane | Active (beta) |
| [ga4gh-infra](https://github.com/SynapticFour/ga4gh-infra) | Identity plane. Compose is the supported deploy; Helm is a sketch. | Active (beta) |
| [Solum](https://github.com/SynapticFour/Solum) | Clinical compliance layer | Early access |
| [BioResearch Assistant](https://github.com/SynapticFour/bioresearch-assistant) | Researcher workbench | Early access |
| [Ferrum Lab Kit](https://github.com/SynapticFour/Ferrum-Lab-Kit) | Compose / Helm / systemd around the Ferrum image | Early access |
| [ferrum-meta](https://github.com/SynapticFour/ferrum-meta) | LinkML schema and archive profiles | Early access |
| [HELIOS](https://github.com/SynapticFour/HELIOS) | Signed pipeline/audit evidence (file ingest; no Ferrum/Solum APIs) | Early access |
| [Ferrum-GA4GH-Demo](https://github.com/SynapticFour/Ferrum-GA4GH-Demo) | Laptop smoke of tagged Ferrum | Reference / demo |
| [Solum-Demo](https://github.com/SynapticFour/Solum-Demo) | Local Stage-1 walkthrough of tagged Solum | Reference / demo |
| [SynapticFour-Showcase](https://github.com/SynapticFour/SynapticFour-Showcase) | Evidence pack across pinned products | Reference / demo |

Related, not one of the ten: [HelixTest](https://github.com/SynapticFour/HelixTest) — GA4GH OpenAPI tests against a running target. A green HelixTest job is a technical signal, not GA4GH certification.

Evaluator entry points live in `docs/FOR-EVALUATORS.md` (Ferrum, ga4gh-infra, Solum, BRA, HELIOS).

## Also in this organisation

| Repository | Role |
|------------|------|
| [gatk-rs](https://github.com/SynapticFour/gatk-rs) | Rust GATK4 haplotype caller (parity work) |
| [Open-Source-GA4GH-Stack](https://github.com/SynapticFour/Open-Source-GA4GH-Stack) | Pointers to the public stack |
| [Mycelium](https://github.com/SynapticFour/Mycelium) / [SecureCollab](https://github.com/SynapticFour/SecureCollab) | Mesh / collaboration |
| [cognitive-landscape-model](https://github.com/SynapticFour/cognitive-landscape-model) | Research programme code |

Not a medical device. Not legal advice. Not a third-party security audit.

Contact: [contact@synapticfour.com](mailto:contact@synapticfour.com)
