# Karpathy Loop — Weighbridge Length & Site Sizing

**Method:** hypothesize → check against data → refine → re-check. Four rounds. All numbers cross-referenced to [05-research-log.md](05-research-log.md) tags (e.g. [B3]).

---

## Round 1 — Baseline Hypothesis

**Hypothesis:** "A 40-ft (12 m) weighbridge is enough for a highway site in Pondy; smaller platform = smaller land, smaller capex, faster payback."

### Check against data

- **Industry spec [B3]:** 12 m platform fits 2-axle rigid trucks and shorter rigids (up to 14-wheel). **Tractor-semitrailers (the 22-wheeler multi-axle class) need 18–24 m.**
- **Cuddalore corridor commodity mix [A6]:** granite, cement (India Cements is on this corridor), containers to Ennore/Chennai port, sugar, pharma. Granite and container trailers are **multi-axle / 22-wheelers by default.**
- **Cost delta [B4]:** 60-ton vs 100-ton is only ~₹3 L of hardware. Civil cost scales roughly with platform length (18 m pad vs 12 m pad → ~50% more concrete) but is small in absolute terms (~₹3–5 L extra).

### Refinement

A 40-ft platform **explicitly excludes** the highest-margin segment of the market (full-semitrailer loads, where the weighment fee is higher and the driver has no alternative within 8 km). Saving ₹5–8 L on capex costs you ~30–40% of addressable revenue permanently.

**Round 1 conclusion:** 40-ft is the wrong question. The question is 60-ft vs 70-ft (18 m vs 22 m).

---

## Round 2 — Truck Mix Reality Check

**Hypothesis:** "Truck mix on the Pondy corridor justifies 60-ft; 70-ft is over-engineered."

### Check against data

- **NH-32 AADT [A2, A5]:** ~17,800 PCUs/day Marakkanam–Puducherry stretch; commercial vehicle share ~15–25% → **~2,500–4,000 trucks/day both directions** (derived).
- **Commodity-driven axle mix [A6]:** granite from quarries + port-bound containers = high share of multi-axle 22-wheelers and semi-trailers. Cement bulk tankers = rigid 3/4-axle. Sugar/pharma from SIPCOT = container + rigid.
- **Expected axle distribution on this corridor (industry norm, verify):**
  - 2-axle rigid (6-wheel): ~25%
  - 3-axle rigid / tipper: ~30%
  - Multi-axle 4+ axle / semi-trailer: ~40%
  - Over-dimensional / trailer combos: ~5%
- **60-ft (18 m) covers the first three classes completely** — i.e., ~95% of addressable trucks. 70-ft (22 m) adds only the ODC corner, which is a trickle.

### Refinement

60-ft is the sweet spot. 70-ft is real-estate-hungry and serves <5% of the population.

**Round 2 conclusion:** 60-ft (18 m × 3.4 m), 80-ton capacity is the optimum. (Go to 100-ton capacity only if data from existing local weighbridges shows regular overloaded trucks — that is diligence Q2 in [01-panel.md](01-panel.md).)

---

## Round 3 — Queuing, Turnaround & Site Geometry

**Hypothesis:** "Weighbridge zone = platform + ramps + cabin ≈ 500 sqm. Rest is parking."

### Check against data

- **Platform:** 18 m × 3.4 m = **61 sqm**.
- **Approach + departure ramps:** 15 m each side of platform, 4 m wide = 120 sqm. Needed for truck to align squarely on the load cells; short ramps cause repeat weighments.
- **Total linear weighbridge axis:** 15 + 18 + 15 = **48 m long** × 4 m corridor = 192 sqm corridor.
- **Weigh cabin:** 3 × 4 = **12 sqm**, positioned at a 90° angle to platform for sightline.
- **Queuing lane** (peak-hour: 8 trucks/hr × 5 min dwell = ~1 truck in the platform + 1 waiting): need space for **2 trucks in queue** = 2 × 20 m = **40 m** of queuing lane at 4 m wide = **160 sqm**.
- **Turnaround / pull-out:** entering truck needs 15 m swept path; exiting truck needs room to merge back toward highway. Budget **300 sqm** for maneuvering.
- **Bypass lane** (so a truck that decides not to weigh doesn't block the queue): **80 sqm**.

### Refinement

Weighbridge zone realistic footprint:

| Zone | sqm |
|---|---|
| Platform + ramps + cabin | 265 |
| Queuing lane (2 trucks) | 160 |
| Turnaround / maneuvering | 300 |
| Bypass lane | 80 |
| **Subtotal** | **~805 sqm** |

That's **~8,660 sqft just for the weighbridge operation** — 3× larger than a naive "platform + ramps" estimate.

**Round 3 conclusion:** Weighbridge zone realistic footprint is ~800 sqm (0.20 acre) on its own, before adding coffee shop, EV, or shared parking.

---

## Round 4 — Panel Constraint: Physical Segregation

**Panel signal (from [01-panel.md](01-panel.md)):** The weighbridge forecourt must be physically segregated from the car/EV forecourt. Shared entry → brand repulsion (Godin, Doumont). Separation → dual-access plot.

### What this adds

- **Heavy-vehicle entry** from highway service road, directly into weighbridge zone, **separate from** passenger entrance.
- **Visual screening** (landscape berm or 2.5 m boundary wall with planting) between truck zone and hospitality zone = ~5 m buffer strip × the interface length.
- Implication: weighbridge must be at the **back** of the plot (furthest from coffee/EV) with its own service road off the highway. Plot must have sufficient highway frontage for two access points OR be at a T-junction / side-road corner (Porter's "scarce land" criterion).

### Minimum plot frontage implied

- Heavy-vehicle access width (ingress + egress): ~12 m
- 40 m separation on highway frontage (NHAI access-permission norm for two cuts)
- Light-vehicle access width: ~12 m
- **Implied highway frontage minimum: ~65 m** (ideally a corner plot so the two accesses sit on different roads).

---

## Convergent Recommendation

| Decision | Call |
|---|---|
| **Platform length** | **60 ft (18 m)** |
| **Platform width** | 3.4 m |
| **Capacity** | 80-ton (go to 100-ton only if local weighbridge data shows regular overloads) |
| **Construction** | Pitless (per [B5]) — faster install, no water-logging, easier maintenance |
| **Position on plot** | Back of plot, separate entry from hospitality forecourt |
| **Weighbridge-only zone** | ~800 sqm / 0.20 acre |
| **Turnkey capex (weighbridge only)** | ₹18–25 L ([B4]) + ~₹3 L segregation boundary/landscape |

### The one assumption most likely to break this model

**Local weighbridge market saturation.** If there are already 3–4 weighbridges within 8 km and each is running at 40% utilization, your capture rate collapses to 10–15 trucks/day and the zone is over-sized for the revenue. The Round 2 truck-mix math is necessary but not sufficient — you also need diligence Q2 (visit each competing weighbridge, time it, count trucks) to confirm demand isn't already satisfied.

If market is saturated: drop to **40-ft (12 m), 60-ton** as a small tenant-only weighbridge serving one or two logistics companies under contract, and reclaim ~400 sqm of the site for expanded EV / F&B. But then the weighbridge is a captive service, not a public utility, and the economics change.

---

## Output handed to [04-site-plan.md](04-site-plan.md)

- Weighbridge zone: **800 sqm** (expected case), segregated back-of-plot
- Minimum highway frontage: **~65 m** for dual-access
- Capex reserved: **₹22 L** (turnkey + segregation works)
