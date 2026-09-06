# Related public repositories

These public repositories are maintained by the same organisation (Synaptic Four) and are designed to work together. They are **not** a bundle SKU. Each repository keeps its own version and license.

Composition is pin-based: consumers declare which tag or SHA of another repository they use. That join is not sold as one SKU. HelixTest is a related Apache conformance CLI; it is not one of these ten repositories.

**Released join:** this map describes tagged/SHA pins, not `main`. A product `main` may be ahead of the join. A green laptop run against a pin is not proof of that product’s `main`.

The tables below classify every public, non-archived repository so a stranger is not left guessing.

## Maturity labels

| Label | Meaning |
|-------|---------|
| **Active (beta)** | Maintained. One maintainer. Not a third-party audit. Not GA4GH certification. Not a “production-ready” claim. |
| **Early access** | Public source; evaluation. Expect gaps. |
| **Reference / demo** | Laptop evidence of a pinned product. Not a product, not a pilot, not production proof. |

## The ten repositories

| Repository | Role | License | Maturity |
|------------|------|---------|----------|
| [Ferrum](https://github.com/SynapticFour/Ferrum) | GA4GH data/compute plane (DRS, WES, TES, TRS, Beacon v2, htsget, Passports, Crypt4GH) | BUSL-1.1 | Active (beta) |
| [ga4gh-infra](https://github.com/SynapticFour/ga4gh-infra) | Identity plane (OIDC broker, Passports/visas, DUO, ADS, service registry). **Compose is the supported deploy.** Helm is a sketch. | Apache-2.0 | Active (beta) — Compose path |
| [Solum](https://github.com/SynapticFour/Solum) | Clinical compliance layer (consent, audit chain, FHIR interchange, field crypto) | BUSL-1.1 | Early access |
| [BioResearch Assistant](https://github.com/SynapticFour/bioresearch-assistant) | Researcher workbench (literature, phenopackets, local DRS/WES, optional HTTP joins) | BUSL-1.1 | Early access |
| [Ferrum Lab Kit](https://github.com/SynapticFour/Ferrum-Lab-Kit) | Companion: generate Compose / Helm / systemd around a SHA-pinned Ferrum image. Does not implement GA4GH protocol logic. | BUSL-1.1 | Early access |
| [ferrum-meta](https://github.com/SynapticFour/ferrum-meta) | Companion: LinkML schema and archive profiles. `export` copies a committed fixture (`shutil.copyfile`). | Apache-2.0 | Early access |
| [HELIOS](https://github.com/SynapticFour/HELIOS) | Signed pipeline/audit evidence. Reads export JSON from disk. Does **not** call other product APIs. Not a certification. | Apache-2.0 | Early access |
| [Ferrum-GA4GH-Demo](https://github.com/SynapticFour/Ferrum-GA4GH-Demo) | Laptop pipeline smoke of tagged Ferrum (DRS / WES / TES) | Apache-2.0 | Reference / demo |
| [Solum-Demo](https://github.com/SynapticFour/Solum-Demo) | Local Stage-1 walkthrough of tagged Solum (`dev-local.toml`) | Apache-2.0 | Reference / demo |
| [SynapticFour-Showcase](https://github.com/SynapticFour/SynapticFour-Showcase) | Evidence pack and pin checkout across products | Apache-2.0 | Reference / demo |

Related, not in this table: [HelixTest](https://github.com/SynapticFour/HelixTest) (GA4GH OpenAPI tests against a running target). A green job is a technical signal, not GA4GH certification.

Evaluator entry points live in `docs/FOR-EVALUATORS.md` on Ferrum, ga4gh-infra, Solum, BioResearch Assistant, HELIOS, and Helix.

## Also public (not in the join)

These repositories are public and **not** part of the ten-repo released join. They are not a combo SKU with Ferrum.

| Repository | Role | Status |
|------------|------|----------------|
| [Helix](https://github.com/SynapticFour/Helix) | VERIFY CLI. HelixTest becoming a standalone product. Conformance / security behaviour / benchmark. **Not HELIOS.** Not GA4GH certification. | Untagged early-access |
| [helix-action](https://github.com/SynapticFour/helix-action) | GitHub Action around `helix verify`. Not a product SKU. | Ambassador wrapper |
| [helixtest-action](https://github.com/SynapticFour/helixtest-action) | GitHub Action around HelixTest release binaries. Not a product SKU. Pin may lag the suite tag. | Ambassador wrapper |
| [Open-Source-GA4GH-Stack](https://github.com/SynapticFour/Open-Source-GA4GH-Stack) | Upstream OSS Compose/Helm kit for comparison with Lab Kit. **Not Ferrum.** | Teaching / comparison |
| [gatk-rs](https://github.com/SynapticFour/gatk-rs) | Independent GATK4 HaplotypeCaller spine research. Not Broad. Not required for the Ferrum join. | Research / Alpha |
| [technical-reports](https://github.com/SynapticFour/technical-reports) | SF-TR series. Not GA4GH certification. | Citation archive |
| [S4MP](https://github.com/SynapticFour/S4MP) | Heuristic Java↔Rust port maps. `certify` ≠ semantic equivalence. Not a SKU. | Heuristic tooling |
| [cognitive-landscape-research-programme](https://github.com/SynapticFour/cognitive-landscape-research-programme) | Research programme constitution. Not a product SKU. Not diagnostic. | Research |
| [cognitive-landscape-model](https://github.com/SynapticFour/cognitive-landscape-model) | CLM modelling library. Not a SKU. Not diagnostic. Not Ferrum. | Research |
| [perceptual-cognitive-mapping-system](https://github.com/SynapticFour/perceptual-cognitive-mapping-system) | PCMS research instrument. Not a SKU. Not diagnostic. Not a GDPR certification. | Research; live demo |
| [.github](https://github.com/SynapticFour/.github) | This organisation profile. | Map you are reading |

## Archived / private (do not treat as join)

**Archived (parked, not Ferrum):** [Synaptic-Core-Demo](https://github.com/SynapticFour/Synaptic-Core-Demo), [sc-specs](https://github.com/SynapticFour/sc-specs), [sc-transport](https://github.com/SynapticFour/sc-transport), [SecureCollab](https://github.com/SynapticFour/SecureCollab), [vibecheck](https://github.com/SynapticFour/vibecheck).

**Private:** mycelium-relay is a private bootstrap relay, not a public product.

## What this is not

- Not GA4GH certification.
- Not a third-party security audit.
- Not a medical device.
- Not legal advice (GDPR, EHDS, HIPAA, or otherwise).
- Not a combo SKU or a suite discount.

Questions can be sent to [contact@synapticfour.com](mailto:contact@synapticfour.com).
