# Synaptic Four

Customer-sovereign infrastructure for genomics and clinical research. Stuttgart.

**Start here:** [Related repositories](SUITE-OVERVIEW.md) · [Products](https://synapticfour.com/products)

## Try it (~30 min)

Not GA4GH certification. Not a production or clinical pilot.

1. **No Docker** — Helix fixtures: clone [Helix](https://github.com/SynapticFour/Helix) and [HelixTest](https://github.com/SynapticFour/HelixTest) as siblings, then `cd Helix && make prove && make verify-drs` ([FOR-EVALUATORS](https://github.com/SynapticFour/Helix/blob/main/docs/FOR-EVALUATORS.md)). Optional: [HELIOS](https://github.com/SynapticFour/HELIOS) `make prove` (tamper-reject on disk fixtures; no Ferrum).
2. **Docker** — [Ferrum-GA4GH-Demo](https://github.com/SynapticFour/Ferrum-GA4GH-Demo) `./run` (tagged Ferrum **v0.3.2**, gateway `http://127.0.0.1:18080`). Read `results/RUN_MANIFEST.json`. hap.py F1 0 on the synthetic slice is expected.
3. **Optional probe** — with the demo still up: `GATEWAY_BASE=http://127.0.0.1:18080 helixtest --all --mode ferrum --only drs` (HelixTest pin **v0.1.3**). Default HelixTest Ferrum profile is `:8080`; this demo is `:18080`.

Longer pack (Demo + HELIOS together): [SynapticFour-Showcase](https://github.com/SynapticFour/SynapticFour-Showcase) `make up`.

These public repositories are maintained together and designed to compose by pin (tag or SHA). Each keeps its own version and license.

## Products

| Repository | Role | Maturity |
|------------|------|----------|
| [Ferrum](https://github.com/SynapticFour/Ferrum) | GA4GH data/compute plane | Active (beta) |
| [ga4gh-infra](https://github.com/SynapticFour/ga4gh-infra) | Identity plane. Compose is the supported deploy. | Active (beta) |
| [Solum](https://github.com/SynapticFour/Solum) | Clinical compliance layer | Early access |
| [BioResearch Assistant](https://github.com/SynapticFour/bioresearch-assistant) | Researcher workbench | Early access |
| [HELIOS](https://github.com/SynapticFour/HELIOS) | Signed pipeline and audit evidence | Early access |

Companions, demos, [HelixTest](https://github.com/SynapticFour/HelixTest), [Helix](https://github.com/SynapticFour/Helix), research, and tooling are listed in [SUITE-OVERVIEW](SUITE-OVERVIEW.md).

Contact: [contact@synapticfour.com](mailto:contact@synapticfour.com)
