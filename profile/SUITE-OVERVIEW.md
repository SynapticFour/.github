# Related public repositories

These public repositories are maintained by the same organisation (Synaptic Four) and are designed to work together. They are **not** a bundle SKU. Each repository keeps its own version and license.

Composition is pin-based: consumers declare which tag or SHA of another repository they use. That join is not sold as one SKU. HelixTest is a related Apache conformance CLI; it is not one of these ten repositories.

**Released join:** this map describes tagged/SHA pins, not `main`. A product `main` may be ahead of the join. A green laptop run against a pin is not proof of that product’s `main`.

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

Evaluator entry points live in `docs/FOR-EVALUATORS.md` on Ferrum, ga4gh-infra, Solum, BioResearch Assistant, and HELIOS.

## What this is not

- Not GA4GH certification.
- Not a third-party security audit.
- Not a medical device.
- Not legal advice (GDPR, EHDS, HIPAA, or otherwise).
- Not a combo SKU or a suite discount.

Questions can be sent to [contact@synapticfour.com](mailto:contact@synapticfour.com).
