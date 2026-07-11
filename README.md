# SendWaste AI

SendWaste AI is building a cloud-native operating layer for verified waste collection, settlement and recovery data in African cities.

The platform is designed to connect households, informal collectors, recycling partners, businesses and public agencies through one evidence trail. A collection request becomes a geo-tagged service record. AI assists with material recognition, fraud screening, route prioritisation and impact calculations. Operators retain decision authority and every material action is auditable.

## Why this matters

Waste collection across fast-growing cities remains fragmented. Residents struggle to access reliable pickup. Informal collectors complete valuable work without the records needed to prove income, performance or environmental impact. Recyclers lack predictable supply data. Governments and corporate sustainability teams cannot easily verify where material came from, who handled it or what was recovered.

SendWaste AI converts this missing evidence into operational infrastructure.

## Current stage

**Stage:** functional public prototype and cloud architecture prepared for pilot development.

The current repository contains:

- a responsive product and venture website;
- a working browser-based collection request demonstration;
- public architecture, data model, privacy and responsible AI documentation;
- deployment configurations for GitHub Pages, Cloudflare Pages and Vercel;
- mapped implementation paths for AWS, Microsoft Azure and Cloudflare;
- a 12-month engineering roadmap for a live Abuja pilot.

The prototype is separate from the earlier SendWaste Cardano experiment. It focuses on AI-assisted operations, cloud deployment and verifiable recovery records rather than blockchain infrastructure.

## Product workflow

1. **Request**: a resident or organisation submits material type, estimated quantity, location and preferred collection window.
2. **Triage**: the platform classifies the request, checks for duplicate or suspicious submissions and produces an operational priority score.
3. **Dispatch**: the system matches a suitable collector and proposes an efficient route.
4. **Verify**: collection evidence, weight and partner confirmation create an auditable recovery record.
5. **Settle**: participants receive a transparent breakdown of earnings, fees or rewards.
6. **Report**: dashboards aggregate service, material and environmental indicators for authorised users.

## Proposed cloud workload

The production system requires more than static hosting. The architecture includes:

- identity and role-based access;
- API services and background jobs;
- relational transaction data;
- object storage for collection evidence;
- geospatial search and route optimisation;
- AI inference endpoints;
- event queues and notification services;
- analytics, observability and model monitoring;
- encryption, secrets management, audit logs and edge protection.

See [`docs/CLOUD_ARCHITECTURE.md`](docs/CLOUD_ARCHITECTURE.md) and [`docs/CLOUD_CREDITS_READINESS.md`](docs/CLOUD_CREDITS_READINESS.md).

## Pilot objectives

The first production pilot is planned for Abuja and will test whether SendWaste AI can:

- reduce the time required to assign collection requests;
- improve the completeness of recovery evidence;
- reduce duplicate and invalid records;
- create reliable income and service histories for collectors;
- provide partners with exportable recovery and impact data.

Pilot targets will be finalised with implementation partners and reported separately from historical UpwardEco activity.

## Founding team

**Muhammed Sanusi, Co-founder and Chief Executive Officer**  
Strategy, operations, institutional partnerships and field implementation.

**Bethel Chinedu Clement, Co-founder and Chief Technology Officer**  
Product architecture, AI systems, data governance, research and technical delivery.

The founding team combines practical circular-economy operations with technology and environmental research experience in Nigeria.

## Run locally

No build step is required.

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080`.

## Repository map

```text
.
├── index.html
├── styles.css
├── app.js
├── assets/
├── docs/
├── .github/workflows/pages.yml
├── wrangler.toml
└── vercel.json
```

## Public contacts

Planned domain: `sendwaste.ai`

- General: `hello@sendwaste.ai`
- Pilot partnerships: `pilots@sendwaste.ai`
- Institutional partnerships: `partnerships@sendwaste.ai`
- Security: `security@sendwaste.ai`
- Privacy: `privacy@sendwaste.ai`

Until domain email is activated, contact: `clementsbethel@gmail.com`.

## Licence

MIT. See [`LICENSE`](LICENSE).
