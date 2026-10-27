<div align="center">

# 🚀 Super91 Engineering
### Next-Generation Distributed Print Commerce & Intelligent Logistics Platform

[![Website](https://img.shields.io/badge/Website-super91.com-0284c7?style=for-the-badge&logo=google-chrome&logoColor=white)](https://super91.com)
[![Platform](https://img.shields.io/badge/Platform-Production%20Active-10b981?style=for-the-badge)](https://super91.com)
[![Twitter](https://img.shields.io/badge/Twitter-@super91__-1da1f2?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/super91_)
[![Support](https://img.shields.io/badge/Support-support%40super91.com-6366f1?style=for-the-badge&logo=gmail&logoColor=white)](mailto:support@super91.com)

<p align="center">
  Empowering businesses, print entrepreneurs, and enterprise franchises across India with on-demand custom printing, automated prepress engineering, and decentralized fulfillment networks.
</p>

---

</div>

## 📌 About Super91

**Super91** is revolutionizing the printing and merchandise industry through proprietary full-stack automation. We bridge the gap between high-volume commercial manufacturing and agile neighborhood print fulfillment.

From high-precision business stationery and promotional collateral to large-format signage and custom packaging, our platform connects direct-to-consumer digital storefronts with centralized production hubs (NPH/CPH) and local delivery franchises (DF).

---

## 🏗️ Core Platform Ecosystem

```
+--------------------------------------------------------+
|             Super91 Customer Storefront                |
|  Dynamic PDP · Multi-Attribute Pricing · Artwork Upload|
+--------------------------+-----------------------------+
                           |
                           v
+--------------------------------------------------------+
|              Central Prepress Engine (DCP)             |
|  FIFO Queue · Single-User Lock Guard · Preflight Rules |
+--------------------------+-----------------------------+
                           |
            +--------------+--------------+
            |                             |
            v                             v
+-----------------------+     +-----------------------+
|National Production Hub|     | Central Production Hub|
|         (NPH)         |     |         (CPH)         |
|Multi-Dept Print Line  |     |Fast-Turnaround Finishing|
+-----------+-----------+     +-----------+-----------+
            |                             |
            +--------------+--------------+
                           |
                           v
+--------------------------------------------------------+
|          Intelligent Logistics & Franchise Network     |
| Multi-Box Barcode Scanning · Rack Routing · Delivery OTP|
+--------------------------------------------------------+
```

### 1. 🛍️ Dynamic Storefront & Product Configurator
* **Real-Time Costing Engines:** Instant multi-attribute calculation based on sheet sizes, paper GSM, lamination types, quantity tiers, and square-footage dimensional formulas.
* **Smart Artwork Intake:** Vector PDF, high-res raster, and multi-file composite artwork validation backed by Google Cloud Storage (GCS).

### 2. 🎨 Central Prepress & DCP Operations
* **Unified FIFO Queue:** Shared cross-entity prepress check queue between Head Office operators and specialized franchise designers.
* **Atomic Single-User Locking:** Race-condition prevention ensuring only one designer claims and verifies an artwork at any given moment.
* **Fairness & Incentive Engine:** Sequence-break safeguards, out-of-turn warning alerts, and automated performance point allocation.

### 3. 🏭 Production Jobsheets & Hub Networks
* **Dual-Hub Architecture:** Orchestration between large-scale National Production Hubs (**NPH**) and localized Central Production Hubs (**CPH**).
* **Granular Stage Tracking:** Real-time visibility across Prepress ➔ Printing ➔ Post-Print / Lamination ➔ Ready for Handover / Packing ➔ Complete.

### 4. 📦 Intelligent Logistics, Scanning & Handover
* **Multi-Box Gated Scanning:** Continuous camera and hardware barcode scanning for multi-parcel shipments with automatic session resets on cancellation.
* **Rack & Zone Management:** Physical and virtual rack mapping for delivery sub-zones, partner DF holds, and self-pickup shelves.
* **End-to-End Custody:** Secure delivery handoffs backed by 4-digit customer OTPs and courier route manifests.

---

## 🛠️ Technology Stack

| Domain | Technologies |
|---|---|
| **Frontend Web** | React 18, TypeScript, Vite, Tailwind CSS, Lucide Icons, Axios |
| **Backend API** | Node.js (ESM), Express.js, Mongoose, REST & GraphQL APIs |
| **Database & Cache** | MongoDB Atlas, Redis Caching, In-Memory TTL stores |
| **Cloud & Media** | Google Cloud Storage (GCS), Cloudinary, Docker |
| **Tooling & CI/CD** | GitHub Actions, Git Workflows, Jest, ESLint, Prettier |

---

## 🌐 Hub & Logistics Operating Model

| Hub Type | Description | Primary Operational Focus |
|---|---|---|
| **NPH** (National Production Hub) | High-capacity industrial manufacturing facility | Large offset print runs, bulk catalogs, and multi-stage packaging |
| **CPH** (Central Production Hub) | Regional high-speed production center | Rapid digital printing, fast-turnaround jobs, and direct counter pickup |
| **DF** (Delivery Franchise) | Localized distribution franchise | Last-mile parcel reception, sorting, driver dispatch, and customer collection |

---

## 👨‍💻 Engineering Culture & Developer Workflows

We build with strict attention to performance, security, operational simplicity, and real-world floor usability.

### 🌿 Branching Strategy
* `main` / `production` — Production-ready, auto-deployed releases.
* `v1.1` / `staging` — Release staging and pre-production regression testing.
* `feat/<ticket>-<description>` — Feature branches.
* `fix/<ticket>-<description>` — Bug fixes and operational patches.

### 📝 Commit Message Conventions
We adhere to Conventional Commits:
* `feat(logistics): add in-modal continuous multi-box scan counter`
* `fix(prepress): prevent race conditions during DCP order claim`
* `refactor(franchise): optimize queue aggregate queries`

---

## 📬 Contact & Connect

* 🌐 **Website:** [super91.com](https://super91.com)
* 💼 **HQ & Operations:** Jaipur, Rajasthan, India
* 📧 **Developer & Platform Support:** [support@super91.com](mailto:support@super91.com)
* 🐦 **X / Twitter:** [@super91_](https://twitter.com/super91_)

<div align="center">
  <sub>© 2026 Super91. All rights reserved. Built with precision for India's print creators.</sub>
</div>
