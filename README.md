# Materiality Map — ESG Disclosure Engine for Utilities

**Live app → [sattvitripathy.github.io/materiality-map](https://sattvitripathy.github.io/materiality-map/)**

A deterministic, traceable disclosure engine for sustainability reporting. Describe a utility's operations and Materiality Map scopes the **specific disclosures** that apply — then goes a step further than any checklist: it traces each disclosure back to the **exact unit operation that generates the number** and the meter or record that captures it. It turns "which standards do we report against?" into "*here* is the figure, *here* is where it comes from, and *here* is whether it will survive assurance."

---

## What it does

- **Guided four-step flow** — from a company profile to a scoped set of disclosures, no ESG expertise required. A one-click **guided walkthrough** demos the whole pipeline end to end.
- **Two audiences, one engine** — pick a seat on entry: a **disclosing company** (where to collect each number) or an **analyst / assurer** (whether to trust it). The same map, reframed to the reader.
- **Multi-standard coverage** — maps disclosures across **GRI, SASB, ISSB, ESRS, BRSR, and CDP** (111 indicators across 7 standards), then filters by jurisdiction (BRSR for India-listed, ESRS for in-scope EU operators, and so on).
- **Node-level provenance** — every process-mapped disclosure is traced to the unit operation that produces it, carrying its physical **mechanism**, **GHG scope**, **measurement method**, **data-confidence tier** (measured / calculated / estimated), and **materiality weight**.
- **Collect once, report everywhere** — a single measurement (e.g. Scope 1 CO₂ from the combustion node) satisfies the whole family of equivalent codes across six frameworks at once; the overlap analysis makes that explicit.
- **Deterministic & auditable** — the same inputs always produce the same mapping; nothing is left to a black box.
- **Excel export** — download the scoped set as a workbook: a tab per standard, an overlap analysis, a data-collection plan, and a dedicated **node-provenance** tab.
- **Runs in the browser** — no backend, no account; your inputs stay on your device.

## How it goes deeper

Under the hood, each recurring physical step — combustion, the cooling-water circuit, ash handling, grid losses, fugitive gases — is a reusable **unit-operation primitive** that carries the metrics it generates. Archetypes are *composed* from this shared library rather than hand-authored, so the metric knowledge is written and verified once and reused everywhere.

- **25 unit-operation primitives** compose **all 15 utility archetypes** (coal thermal, CCGT, solar, onshore wind, large hydro, nuclear, battery storage, transmission, distribution, retail, integrated, renewable IPP, biomass/WtE, trading, EV charging).
- Because the primitives are shared, the same `combustion` node yields SO₂/particulates for coal and methane-slip for gas from the fuel context alone — no duplicated authoring.
- The disclosures that stay "phase-level" rather than traced are the cross-cutting governance and workforce baselines that belong to the whole organisation, not to a single operation — an honest boundary, not a gap.

## Who it's for

Sustainability and ESG teams at utilities (and utility-adjacent companies) who need to know *which* disclosures apply and *where each number originates* before they start reporting — and the analysts and assurers who have to verify those numbers afterward.

## Built with

React · JavaScript · SheetJS (Excel export) · a hand-curated ESG standards knowledge graph and unit-operation primitive library. Static single-page app hosted on GitHub Pages.

## Run it locally

Any static file server works — the app compiles JSX in the browser:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

---

<sub>Part of my [portfolio](https://sattvitripathy.github.io/portfolio/) · Built with AI assistance</sub>
