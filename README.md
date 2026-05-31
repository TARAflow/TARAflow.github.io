<div align="center">

# TARAflow

### Graph-based Threat Analysis &amp; Risk Assessment for OT, embedded &amp; cyber-physical systems

[![Status](https://img.shields.io/badge/status-in%20development-36e2b4)](https://github.com/TARAflow)
[![License: GPL v3](https://img.shields.io/badge/license-GPLv3-1ea7d6)](https://www.gnu.org/licenses/gpl-3.0)
[![Standards](https://img.shields.io/badge/IEC%2062443%20%C2%B7%20ISO%2021434%20%C2%B7%20CRA-aligned-6b7787)](#standards--regulatory-alignment)

**Map threats. Trace risk. Flow to mitigation.**

[Landing page](https://taraflow.github.io) · [Roadmap](#roadmap) · [Contributing](#contributing)

</div>

---

> **🚧 Pre-release.** This repository is the future public home of TARAflow. The codebase is currently developed privately and will be transferred here once it reaches a stable milestone. Star or watch the repo to follow along.

---

## What is TARAflow?

TARA — **Threat Analysis and Risk Assessment** — is a cornerstone of modern product security. TARAflow makes it **graph-based and traceable**: every threat links back to the asset it endangers and forward to the control that mitigates it.

Starting from a **data-flow diagram (DFD)**, TARAflow derives protection goals, generates STRIDE-based threats per element and per interaction, scores risk as **impact × likelihood**, and tracks each mitigation through to verification.

The result is a *living* assessment — not a static spreadsheet — that holds up in audits and evolves with your system.

```
  Asset & DFD  →  Protection goals  →  Threats (STRIDE)  →  Risk = I × L  →  Mitigation & verify ✓
```

## Why

Most TARA work today lives in sprawling spreadsheets where the link between an asset, the threats against it, and the controls that mitigate them is implicit at best. That makes assessments hard to maintain, hard to audit, and easy to inflate.

TARAflow treats the assessment as a **connected graph** so that traceability is a property of the model, not a manual bookkeeping exercise. It is built for engineers and security consultants who need defensible, standards-aligned results without the spreadsheet sprawl.

## Features

- **Graph-based modeling** — assets, data flows and threats live in a connected graph; relationships are first-class.
- **DFD-driven threat generation** — draw or import a data-flow diagram; STRIDE threats are proposed per element and per interaction.
- **Quantified risk** — impact × likelihood scoring with configurable factor sets (OWASP, ETSI, EN 50742) and threshold-based risk levels.
- **Native safety–security integration** — physical impact and safety-override rules feed directly into the risk model.
- **Asset-aware impact** — per-criterion impact ratings flow from assets into the risk assessment.
- **Mitigation &amp; verification tracking** — link controls to threats, track implementation progress, tie each mitigation to a verification.
- **Audit-ready documentation** — generate output that maps cleanly to the standards below.

## Standards &amp; regulatory alignment

| Standard / Regulation | Domain |
|---|---|
| IEC 62443 | Industrial automation &amp; control systems (OT/ICS) |
| ISO/SAE 21434 | Automotive cybersecurity engineering |
| EU Cyber Resilience Act (CRA) | Products with digital elements |
| EN 50742 | Attacker-potential / risk methodology |
| STRIDE | Threat categorization |
| CIANAAA | Protection-goal model (C/I/A + N/AuthN/AuthZ/Acc) |

## Where it's used

- **Industrial &amp; OT** — PLCs, machinery and ICS environments under IEC 62443 and the Machinery Regulation.
- **Embedded &amp; IoT** — connected devices and firmware facing the EU Cyber Resilience Act.
- **Automotive** — cyber-physical components requiring ISO/SAE 21434 TARA workflows.
- **Medical &amp; safety-critical** — systems where safety and security must be assessed together, not in isolation.

## Tech stack

| Layer | Technology |
|---|---|
| Runtime | [Electron](https://www.electronjs.org/) (cross-platform desktop) |
| UI | [React](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/) |
| Diagramming | draw.io / mxGraph integration for DFD editing |
| Visualization | D3.js (attack trees &amp; graph views) |
| Documentation export | Markdown / AsciiDoc / PDF |
| i18n | Namespaced translation files (EN / DE) |

> The stack is documented here for transparency; the source itself follows once transferred.

## Roadmap

> Indicative and subject to change as the project matures.

- [ ] **Public code transfer** — move the stable codebase into this repository
- [ ] **First tagged release** — installable desktop builds
- [ ] **Reference example** — end-to-end worked case (DFD → threats → risk → mitigation)
- [ ] **Documentation site** — methodology guide and user manual
- [ ] **Standards mapping appendix** — explicit clause-level references for IEC 62443 / ISO 21434 / CRA
- [ ] **Import/export interoperability** — exchange formats for existing TARA tooling

## Contributing

The repository is **not yet open for code contributions** — there is no source here to build against until the transfer is complete.

In the meantime you can:

- **Watch / star** this repository to be notified when the code lands.
- **Open an issue** to share feedback on the methodology, suggest features, or describe a use case you'd like supported. Early input is genuinely valued and helps shape the public release.

Once the codebase is transferred, contribution guidelines, a code of conduct, and a development setup guide will be added here.

## License

TARAflow will be released under the **GNU General Public License v3.0**. See [`LICENSE`](LICENSE) once the code is published.

GPLv3 in short: you are free to use, study, share and modify the software; derivative works must remain under the same license and keep their source available.

## Contact

- **Issues &amp; feature ideas:** [GitHub Issues](https://github.com/TARAflow/TARAflow/issues)
- **Project home:** [taraflow.github.io](https://taraflow.github.io)

---

<div align="center">
<sub>TARAflow · threat modeling and risk assessment for the systems that run the physical world.</sub>
</div>
