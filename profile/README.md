<div align="center">

# Compliance-to-Architecture Framework™

**Open spec · machine-readable · Apache-2.0**

[![License](https://img.shields.io/badge/license-Apache--2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Status](https://img.shields.io/badge/status-public%20OSS-brightgreen.svg)](https://github.com/Compliance-to-Architecture)
[![Spec](https://img.shields.io/badge/spec-v0.1-orange.svg)](https://github.com/Compliance-to-Architecture/framework)
[![Website](https://img.shields.io/badge/site-compliancetoarchitecture.com-1F6FEB.svg)](https://compliancetoarchitecture.com)
[![Frameworks](https://img.shields.io/badge/frameworks-25-success.svg)](https://github.com/Compliance-to-Architecture/framework)
[![Sector packs](https://img.shields.io/badge/sector%20packs-3-success.svg)](https://github.com/Compliance-to-Architecture/sector-packs)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#contributing)

</div>

---

## What this org publishes

The **Compliance-to-Architecture Framework™** is an open, machine-readable bridge from regulation to software architecture. It is a public Apache-2.0 spec. The repos below are the canonical artefacts; the commercial implementation lives separately under [ReguNav](https://github.com/ReguNav).

| Repo | What it ships | License |
| --- | --- | --- |
| [`framework`](https://github.com/Compliance-to-Architecture/framework) | 25 framework dictionaries (EU AI Act, ISO 42001, ISO 27001, ISO 27701, GDPR, UK GDPR, HIPAA, SOC 2, SOC 1, PCI DSS, NIST AI RMF, NIST CSF, DORA, NIS2, EU CRA, CCPA, LGPD, DPDP India, PIPL China, APPI Japan, Privacy Act AU, HF model-card), crosswalks, policy-as-code compile targets | Apache-2.0 |
| [`ontology`](https://github.com/Compliance-to-Architecture/ontology) | JSON-LD ontology, schemas, IaC examples (AWS · GCP · Azure · Cloudflare), SPEC.md, METHODOLOGY.md | Apache-2.0 |
| [`sector-packs`](https://github.com/Compliance-to-Architecture/sector-packs) | Vertical bundles — maritime, legal, oil & gas. Frameworks + rule packs + evidence templates per sector | Apache-2.0 |
| [`dictionaries`](https://github.com/Compliance-to-Architecture/dictionaries) | Canonical taxonomies — actor-role, evidence-type, control-category, obligation-category, evidence-frequency, reason-code, authority-category, architecture-capability | Apache-2.0 |
| [`playbooks`](https://github.com/Compliance-to-Architecture/playbooks) | Skill files + worked examples for building compliance-engine integrations | Apache-2.0 |

---

## The 12-layer model

```
  L1  Authority         — who issues the obligation (regulator, board, contract)
  L2  Jurisdiction      — where the obligation applies (geo, sector, asset class)
  L3  Risk              — the harm the obligation protects against
  L4  Obligation        — the canonical "must" / "shall" statement
  L5  Control           — the technical / procedural mitigation
  L6  Mitigation        — the residual-risk treatment
  L7  Architecture      — the system surface that bears the control
  L8  Policy-as-Code    — Cerbos / OPA / Cedar / Rego that enforces the control
  L9  Workflow          — the operational procedure
  L10 Evidence          — the artefact produced
  L11 Audit-Trail       — the immutable record of every decision
  L12 Audit-Pack        — the auditor-ready bundle
```

Each layer is a typed node class in the [ontology](https://github.com/Compliance-to-Architecture/ontology). Edges between layers are TYPED — crosswalks across frameworks are first-class graph entities, queryable via GraphQL / SPARQL.

---

## Why this exists

[![Why](https://img.shields.io/badge/Why-this%20exists-1F6FEB.svg)](https://compliancetoarchitecture.com)

Boards adopt policies. Auditors sample controls quarterly. Engineers ship daily. The artefacts the four groups exchange — screenshots, spreadsheets, emails — are produced after the fact, refreshed manually, never reconciled. The Compliance-to-Architecture Framework™ is the **machine-readable bridge** between the four ontologies so each role works against the same canonical model.

---

## How to use

| You are | Start here |
| --- | --- |
| **Regulator / standards body** | Publish your obligations as JSON-LD nodes ([ontology](https://github.com/Compliance-to-Architecture/ontology)). Issue updates as graph deltas. |
| **Compliance team** | Adopt the [framework](https://github.com/Compliance-to-Architecture/framework) crosswalk graph; map your controls once, get every framework. |
| **Auditor** | Walk the framework graph instead of sampling spreadsheets. Tamper-evident audit-trail by construction. |
| **Security architect** | Reference control IDs by URI in your diagrams; auto-generate from [ontology](https://github.com/Compliance-to-Architecture/ontology). |
| **Platform engineer** | Compile policy-as-code (Cerbos · OPA · Cedar) from the [dictionaries](https://github.com/Compliance-to-Architecture/dictionaries) control catalogue. |
| **Executive / board** | One risk register, multiple authorities. Composite index drills down to obligation → control → evidence. |

---

## Contributing

[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#)
[![Code of conduct](https://img.shields.io/badge/code%20of%20conduct-Contributor%20Covenant-purple.svg)](https://www.contributor-covenant.org/)

By contributing you agree your contribution is Apache-2.0. Open a PR against the relevant repo:

- New framework or crosswalk update → [`framework`](https://github.com/Compliance-to-Architecture/framework)
- Ontology schema change → [`ontology`](https://github.com/Compliance-to-Architecture/ontology)
- New sector pack → [`sector-packs`](https://github.com/Compliance-to-Architecture/sector-packs)
- Dictionary term addition → [`dictionaries`](https://github.com/Compliance-to-Architecture/dictionaries)
- Skill / worked example → [`playbooks`](https://github.com/Compliance-to-Architecture/playbooks)

Larger / cross-repo proposals: open an issue under `framework` with a `proposal:` prefix and CC the relevant repo maintainers.

---

## Provenance

Upstream master: [ReguNav/app](https://github.com/ReguNav/app) (private, commercial SaaS). The five public repos here are mirrored from `packages/*` of that monorepo on each release.

Trademark: "Compliance-to-Architecture Framework", "Compliance-to-Architecture Graph", "ReguNav", "Code Constitution" are trademarks of Regunav Inc. The framework spec and ontology are Apache-2.0; the trademarks are not licensed (no consumer of the spec gets a trademark licence — the marks identify the original publishers).

---

<div align="center">

[![Site](https://img.shields.io/badge/compliancetoarchitecture.com-→-1F6FEB.svg?style=for-the-badge)](https://compliancetoarchitecture.com)
[![Framework](https://img.shields.io/badge/github-framework-181717.svg?logo=github&style=for-the-badge)](https://github.com/Compliance-to-Architecture/framework)

</div>
