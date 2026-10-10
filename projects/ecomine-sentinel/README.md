# EcoMine Sentinel - Forum MVP

**Team 91 · Track 4: Climate, Ecological and Biodiversity Engineering**  
Russian-African Forum-Contest of Young Scientists under the auspices of UNESCO, 2026.

EcoMine Sentinel is a proposed **low-cost ecological digital twin** for mine-water, biodiversity and restoration monitoring. This repository contains a presentation-ready, offline-first MVP that demonstrates the accepted project workflow.

> **Scientific integrity:** all dashboard readings, alerts and performance values in the MVP are **simulated demo data**. They demonstrate the proposed workflow and pre-specified proof-of-concept targets; they are not claimed field results.

## Accepted core design

The accepted concept proposes a 12-month Nigerian pilot with six modular stations:

- 2 impact-zone nodes
- 2 buffer-zone nodes
- 2 reference-zone nodes
- 15-minute pH, conductivity, turbidity, temperature, humidity, particulate and noise readings
- Sentinel-2 NDVI / NDWI / bare-soil change metrics
- bird acoustic monitoring, pollinator transects and vegetation plots
- verified community observations
- monthly field/laboratory validation and quarterly metal analyses

Starting explainable risk weights:

- Mine-water condition: **40%**
- Habitat stress: **20%**
- Biodiversity response: **20%**
- Satellite change: **10%**
- Verified community observations: **10%**

These weights are starting values to be recalibrated against expert classifications.

## Proof-of-concept targets

- ≥85% data uptime
- ≥80% agreement with expert classifications
- ≥15% improvement over the strongest single-source method
- ≥20% lower monitoring cost per cycle than consultant-only inspection
- alerts within 24 hours
- accepted proof-of-concept budget: **US$18,000**

## Why the MVP is aligned to Track 4

The official Track 4 focus is engineering methods for ecosystem conservation and climate adaptation, including mining-water management, ecosystem conservation around new mining areas, and reducing environmental footprint. EcoMine Sentinel makes **mine-water warning the first decision layer**, then tests whether habitat and biodiversity indicators show ecological recovery.

It also demonstrates useful digital-twin and IoT ideas without changing the project's primary Track 4 environmental purpose.

## Kuje / FCT expansion - proposed Phase 2

The accepted first pilot remains in **Plateau State**. The MVP presents Kuje/FCT only as a future scale-out after proof-of-concept validation.

Evidence supporting a Kuje/FCT scoping phase:

- The Nigerian Geological Survey Agency's 2022 FCT mineral-resources map lists commodities across the FCT including gold, granite, feldspar, kaolin, lead-zinc, cassiterite, tantalite, tin and sand.
- A 2023 study in Chibiri, Kuje reported environmental impacts associated with sand mining, including land alteration, ecosystem disturbance, soil erosion and vegetation loss.

Any Kuje deployment should begin with site/cadastre confirmation, permissions and baseline sampling; no current deployment is claimed.

## Run locally

No framework or build step is required.

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080`.

Useful reproducible demo states:

- `?view=overview&scenario=water`
- `?view=evidence&scenario=water`
- `?view=validation&scenario=water`
- `?view=scale&scenario=water`

## 3-minute panel flow

1. **Overview:** trigger **Mine-water event**.
2. **Explain:** show why the score changed and which evidence supports it.
3. **Evidence Fusion:** demonstrate that every signal stays visible and auditable.
4. **Validation:** show the testable POC targets and US$18k budget.
5. **Scale & Partnership:** keep Plateau as Phase 1; explain Kuje/FCT as Phase 2 and Russia as cold-climate co-validation.
6. **Ask:** funded POC + mine/lab host + co-validation partner.

## Team

- **Bethel Chinedu Clement** - Project Lead; ecology, biodiversity monitoring, pollinators, birds, vegetation, environmental data integration
- **Kitgak Simon** - Systems Engineering Lead; sensors, solar power, communications, local nodes and field reliability
- **Chinazaekpere Emmanuel Ofodile** - Climate Analytics and Implementation Lead; climate analytics, community implementation and climate-risk interpretation

## References used for the scale narrative

- Russian-African Forum-Contest official Track 4 description: https://youthafrica.spmi.ru/en/participants
- Nigerian Geological Survey Agency (2022), Geological and Mineral Resources Map of FCT Abuja
- Oluyori & Umeh (2023), Environmental Impact of Sand Mining and its Attendant Soil Loss in Chibiri, Kuje Area Council, FCT Abuja
