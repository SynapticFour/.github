# Synaptic Four

Synaptic Four is a sole proprietorship in Stuttgart. It publishes the software and the reports in the table below, so a reader can see which repository does which job.

For a person who arrived from the [website](https://synapticfour.com/en/), and for a person who opened a repository directly.

Start here: this page. The technical hub: [German](https://synapticfour.com/de/technik/), [English](https://synapticfour.com/en/technical/), [French](https://synapticfour.com/fr/technique/). About the company: [English](https://synapticfour.com/en/ueber-synaptic-four/).

The same pages exist in German under `/de/` and in French under `/fr/`.

Each repository's public status is in the table. This profile has no separate stage. An empty status means the claims registry records no stage.

## Try it

About 30 minutes. Not a certificate and not a clinical pilot. A HelixTest run is not certification from GA4GH, a set of shared interfaces for genomic and health data. Registry: FERRUM-MATURITY-001, HELIXTEST-MATURITY-001.

1. In this set of repositories, with no extra services: [Helix](https://github.com/SynapticFour/Helix) and a sibling [HelixTest](https://github.com/SynapticFour/HelixTest) checkout at `HELIXTEST_SHA` in Helix `VERSIONS.lock`. The commands are `make fetch`, then `make prove`, then `make verify-drs`. Expect the line `Helix prove OK (in-process fixtures; not Ferrum, not certification).` The steps are in [Helix getting started](https://github.com/SynapticFour/Helix/blob/main/docs/GETTING-STARTED.md). `make fetch` needs a network. `make prove` does not need Docker or Ferrum.
2. With Docker: [Ferrum-GA4GH-Demo](https://github.com/SynapticFour/Ferrum-GA4GH-Demo) at Ferrum pin **v0.3.2**. Registry: WEB-VERSION-001. `make up` is `./run`. Expect `results/RUN_MANIFEST.json`. The gateway listens on `http://127.0.0.1:18080`. hap.py F1 of 0 on that synthetic slice is expected. The pin is not Ferrum's default branch.

Optional, with the demo still up: HelixTest tag **v0.1.3**. That tag is the release pin. It is not HelixTest's default branch. `GATEWAY_BASE=http://127.0.0.1:18080 helixtest --all --mode ferrum --only drs`. The default Ferrum profile in HelixTest uses port 8080. This demo uses port 18080. The report is a technical signal, not a certificate.

A longer pack, Demo and HELIOS together, is [SynapticFour-Showcase](https://github.com/SynapticFour/SynapticFour-Showcase) `make up`. It needs Docker and the sibling checkouts named in that repository's pin file.

## Repositories

One row per public repository. Early use is the public label where the registry records Active (beta), Early access, or early use. The claim ids are FERRUM-MATURITY-001, SOLUM-MATURITY-001, BRA-MATURITY-001, HELIXTEST-MATURITY-001, HELIOS-MATURITY-001, GA4GH-INFRA-MATURITY-001, and TOOL-LAB-KIT-STATUS-001. An empty status is not a guess.

| Repository | Kind | One sentence | Status | Website |
| --- | --- | --- | --- | --- |
| [Ferrum](https://github.com/SynapticFour/Ferrum) | product | Ferrum keeps genomic research files on an institution's own computers and serves them through shared interfaces. | Early use | [Product page](https://synapticfour.com/en/ferrum/) |
| [Solum](https://github.com/SynapticFour/Solum) | product | Solum records consent, checks whether access to a field is allowed, and writes an audit log beside software a manufacturer already ships. | Early use | [Product page](https://synapticfour.com/en/solum/) |
| [bioresearch-assistant](https://github.com/SynapticFour/bioresearch-assistant) | product | BioResearch Assistant is the working environment where a research team collects publications and asks questions of that collection, with the language model on its own computer by default. | Early use | [Product page](https://synapticfour.com/en/bioresearch-assistant/) |
| [Helix](https://github.com/SynapticFour/Helix) | tool | Helix checks a genomic HTTP service that is already running, and it records what was tested, what was left out, and what must not be claimed. |  | [Open tools](https://synapticfour.com/en/offene-werkzeuge/) |
| [HelixTest](https://github.com/SynapticFour/HelixTest) | tool | HelixTest checks a service that is already running against shared genomic interfaces, and it does not start that service. | Early use | [Open tools](https://synapticfour.com/en/offene-werkzeuge/) |
| [helix-action](https://github.com/SynapticFour/helix-action) | tool | helix-action runs `helix verify` in a GitHub job and fails that job only when a check goes from pass to fail. |  | [Open tools](https://synapticfour.com/en/offene-werkzeuge/) |
| [helixtest-action](https://github.com/SynapticFour/helixtest-action) | tool | helixtest-action downloads published HelixTest `v0.1.3` and runs it against an HTTP service the job already started. |  | [Open tools](https://synapticfour.com/en/offene-werkzeuge/) |
| [HELIOS](https://github.com/SynapticFour/HELIOS) | tool | HELIOS writes a signed check trail for a pipeline whose export is already a file on disk, and it does not run that pipeline. | Early use | [Open tools](https://synapticfour.com/en/offene-werkzeuge/) |
| [ga4gh-infra](https://github.com/SynapticFour/ga4gh-infra) | tool | ga4gh-infra connects an institute's own sign-in to Passports, visas, and access decisions, and it does not replace that sign-in. | Early use | [Open tools](https://synapticfour.com/en/offene-werkzeuge/) |
| [Ferrum-Lab-Kit](https://github.com/SynapticFour/Ferrum-Lab-Kit) | tool | Ferrum Lab Kit writes the start files for a Ferrum service that is already built, around a pinned image. | Early use | [Ferrum](https://synapticfour.com/en/ferrum/) |
| [ferrum-meta](https://github.com/SynapticFour/ferrum-meta) | tool | ferrum-meta is a form for the facts a Ferrum node keeps about a study, a sample, and a file. |  | [Ferrum](https://synapticfour.com/en/ferrum/) |
| [gatk-rs](https://github.com/SynapticFour/gatk-rs) | tool | gatk-rs is a Rust caller for germline short variants on an interval that is already sequenced. |  | [Open tools](https://synapticfour.com/en/offene-werkzeuge/) |
| [Open-Source-GA4GH-Stack](https://github.com/SynapticFour/Open-Source-GA4GH-Stack) | tool | This kit runs upstream GA4GH services side by side, so a lab can compare that arrangement with an integrated lab kit. |  | [Open code](https://synapticfour.com/en/technical/code/) |
| [S4MP](https://github.com/SynapticFour/S4MP) | tool | S4MP suggests Java-to-Rust correspondences from names and tokens, and its certify command records a confirmed review rather than semantic equivalence. |  | [Technical hub](https://synapticfour.com/en/technical/) |
| [sc-specs](https://github.com/SynapticFour/sc-specs) | tool | sc-specs publishes API specifications for object identity, tasks, workflows, discovery, and provenance, for a service whose repository is not public. |  | [Technical hub](https://synapticfour.com/en/technical/) |
| [sc-transport](https://github.com/SynapticFour/sc-transport) | tool | sc-transport is delivery code for telemetry of a service whose repository is not public. |  | [Technical hub](https://synapticfour.com/en/technical/) |
| [vibecheck](https://github.com/SynapticFour/vibecheck) | tool | vibecheck scans a codebase on the machine that runs it, and that scan does not leave the machine. |  | [Technical hub](https://synapticfour.com/en/technical/) |
| [Ferrum-GA4GH-Demo](https://github.com/SynapticFour/Ferrum-GA4GH-Demo) | demo | This demonstration runs tagged Ferrum v0.3.2 on a laptop so a person can see file ingest, a workflow, and a task finish. |  | [Ferrum](https://synapticfour.com/en/ferrum/) |
| [Solum-Demo](https://github.com/SynapticFour/Solum-Demo) | demo | This demonstration runs pinned Solum v0.1.0 on a laptop so a person can see Stage-1 consent, an access check, and an audit log. |  | [Solum](https://synapticfour.com/en/solum/) |
| [SynapticFour-Showcase](https://github.com/SynapticFour/SynapticFour-Showcase) | demo | This showcase is a guided path through pinned product revisions, so a reader can see those revisions run together. |  | [Open code](https://synapticfour.com/en/technical/code/) |
| [Synaptic-Core-Demo](https://github.com/SynapticFour/Synaptic-Core-Demo) | demo | A laptop harness checks adapters of a service whose repository is not public, using a busybox echo rather than a scientific pipeline. |  | [Technical hub](https://synapticfour.com/en/technical/) |
| [perceptual-cognitive-mapping-system](https://github.com/SynapticFour/perceptual-cognitive-mapping-system) | research | PCMS is a public questionnaire that asks how a person focuses, senses, and organises, and shows the answers as positions on continuous scales rather than as a label. |  | [The map](https://synapticfour.com/en/offene-forschung/karte/) |
| [cognitive-landscape-model](https://github.com/SynapticFour/cognitive-landscape-model) | research | CLM is a library that represents ways of thinking as positions on continuous scales, separate from the questionnaire that collects answers. |  | [The base](https://synapticfour.com/en/offene-forschung/unterbau/) |
| [cognitive-landscape-research-programme](https://github.com/SynapticFour/cognitive-landscape-research-programme) | research | CLRP is the open foundation for describing differences in thinking as positions on continuous scales, without turning those positions into a diagnosis. |  | [The programme](https://synapticfour.com/en/offene-forschung/forschungsprogramm/) |
| [SecureCollab](https://github.com/SynapticFour/SecureCollab) | research | A proof piece about encryption, not for patient data. |  | [Open code](https://synapticfour.com/en/technical/code/) |
| [technical-reports](https://github.com/SynapticFour/technical-reports) | report | This repository is the source of the SF-TR series, citable reports on how the software is built. |  | [Publications](https://synapticfour.com/en/publications/) |

This repository, `.github`, is the page GitHub shows for the organisation. It is not one of the five kinds.

## Limits

- An empty status cell means the claims registry has no stage for that repository. This page does not invent Prototype, Early use, In use, or Independently reviewed.
- The 30-minute path is not a certificate and not a clinical pilot. A green run is a technical signal.
- Helix and HelixTest check interfaces. HELIOS signs a file that is already on disk. Those are not the same job. HelixTest already runs. Helix is that suite as the `helix` command.
- Passports are not one of Ferrum's seven interfaces. ga4gh-infra is where an institute's own sign-in is connected to them.
- A private repository is not linked. The service behind Synaptic-Core-Demo, sc-specs, and sc-transport is not a public repository.
- The limits of one repository stay in that repository. This page does not shorten them.
- There is no `CITATION.cff` in this repository.

## Documentation

### Tutorial

- [Try it](#try-it) on this page.

### How-to guides

- Each repository in the table has its own guide. This page does not copy those commands, apart from the path above.

### Reference

- The table on this page.
- [LICENSE](../LICENSE) — Creative Commons Attribution 4.0 International for the text in this repository.

### Explanation

- [Longer role notes](SUITE-OVERVIEW.md). The public status labels are the table on this page.
- [Index](../docs/README.md) of the documents, grouped by kind.

## Licence

The text in this repository is Creative Commons Attribution 4.0 International. Share it and adapt it, with attribution. The file is [LICENSE](../LICENSE). Each software repository keeps its own licence. Those licences are unchanged on this page.

## Contact

[contact@synapticfour.com](mailto:contact@synapticfour.com)
