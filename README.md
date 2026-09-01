# Materiality Map — ESG Disclosure Engine for Utilities

**Live app → [sattvitripathy.github.io/materiality-map](https://sattvitripathy.github.io/materiality-map/)**

A deterministic, traceable disclosure engine for sustainability reporting. Describe a company's operations and Materiality Map scopes the **material sustainability topics** and the **specific disclosures** that apply to it — turning "which standards do we report against?" into a clear, sourced answer.

---

## What it does

- **Guided four-step flow** — from a company profile to a scoped set of disclosures, no ESG expertise required.
- **Multi-standard coverage** — maps material topics and disclosures across **GRI, SASB, ISSB, ESRS, BRSR, and CDP**.
- **Curated knowledge graph** — draws on **111 indicators across 7 standards**, so every result is traceable back to a source.
- **Deterministic & auditable** — the same inputs always produce the same mapping; nothing is left to a black box.
- **Excel export** — download the scoped disclosure set as a spreadsheet for your reporting workflow.
- **Runs in the browser** — no backend, no account; your inputs stay on your device.

## Who it's for

Sustainability and ESG teams at utilities (and utility-adjacent companies) who need to figure out *which* disclosures apply before they start reporting — cutting the manual cross-referencing of overlapping frameworks.

## Built with

React · JavaScript · SheetJS (Excel export) · a hand-curated ESG standards knowledge graph. Static single-page app hosted on GitHub Pages.

## Run it locally

Any static file server works — the app compiles JSX in the browser:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

---

<sub>Part of my [portfolio](https://sattvitripathy.github.io/portfolio/) · Built with AI assistance</sub>
