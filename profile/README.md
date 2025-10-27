# 🛰️ spectra-red

> **Structured Reconnaissance. Global Surface Intelligence.**

Welcome to **spectra-red**, a source-available research initiative focused on building advanced, scalable tooling for port-based exposure analysis and infrastructure intelligence.

---

## 🧠 Our Mission

We build tools that turn **port data** into **context-rich, graph-queryable intelligence**.

Our flagship tool, [`recon`](https://github.com/spectra-red/recon), transforms traditional scanning into structured, high-speed, and AI-enriched reconnaissance.

---

## 🔩 Project: `recon`

`recon` is an all-in-one toolkit for:

- 🌍 **High-speed port scanning** across global target ranges
- 🧠 **AI-assisted analysis** via local or cloud-hosted LLMs
- 🕸️ **Graph modeling** of exposure surfaces in SurrealDB
- 🧬 **Enrichment workflows** with CVEs, Shodan data, banners, DNS, ASN, GeoIP
- 🚨 **Exploit vector surfacing** from known vuln databases

All orchestrated via a **parallel DAG engine** powered by [Restate](https://restate.dev) and visualized through a [Wails](https://wails.io) desktop dashboard.

---

## 🧱 Monorepo Structure (`recon`)

```bash
recon/
├── cmd/
│   ├── recon/             # CLI scanner
│   └── dash/              # Wails-based GUI
│
├── pkg/
│   ├── core/              # Port scanning engine (go-recon)
│   ├── orchestrator/      # Restate workflow logic
│   ├── enrich/            # CVE, DNS, GeoIP, banners, Shodan
│   ├── graphdb/           # SurrealDB schema + querying
│   └── brain/             # LLM triage and summaries
│
├── configs/
│   ├── profiles/          # YAML scan presets
│   └── examples/          # Sample inputs + queries
│
├── LICENSE.md
└── README.md
