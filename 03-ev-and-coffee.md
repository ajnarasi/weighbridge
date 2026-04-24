# Karpathy Loop — EV Charging & Coffee Shop Sizing

Same hypothesis → check → refine discipline as [02-sizing-loop.md](02-sizing-loop.md). Data tags reference [05-research-log.md](05-research-log.md).

---

## Part A — EV Charging Station

### Round 1 — Baseline hypothesis

"Install 2 DC fast chargers (60 kW dual-gun), done. ~200 sqft per bay × 4 guns = 800 sqft total."

### Check

- **BEE mandate [C3]:** one public charger every 25 km on NH. Corridor is currently under-served — Puducherry has the **lowest Level 2 density** nationally [C4].
- **Typical station footprint [C6]:** ~500 sqft for 3–4 car bays.
- **National co-location pattern [C9]:** Tata Power / Statiq / ChargeZone / Ather all co-locate at dhabas — the playbook is proven.
- **Cost envelope [C8]:** ₹24–50 L for a 4–5 charger public station (excl. land).

### Refinement — what's missing from the baseline

1. **Two chargers is under-scale.** A 60 kW dual-gun unit charges one car in ~45 min. At highway peak (12–3 pm, Fri–Sun), demand outstrips supply almost immediately. The next-available-charger check in apps like Tata Power and Statiq drives drivers *past* undersized stations.
2. **AC-only mix is wrong.** Highway = dwell-time constrained, EV driver wants DC.
3. **No transformer pad.** A 55–75 kVA transformer [C8] + LT/HT panel needs ~20 sqm of dedicated secure space.
4. **No queuing / waiting area.** EV drivers wait 30–45 min; they walk to the coffee shop. Flow must support this without blocking bays.

### Round 2 — Right-sized hypothesis

"4 DC fast-charge guns (2 dual-gun 60 kW units) + 2 AC slow chargers (7–22 kW) for longer dwell / overnight. Partner with one named CPO for revenue-share."

### Check against data

- **4 DC guns × 1 car each = 4 simultaneous cars charging.** At 45-min session × 10 hrs useful daylight = ~50 sessions/day theoretical max. Realistic 50% utilization year-3 → **~25 sessions/day** — matches emerging industry benchmarks for Tier-2 highway sites.
- **2 AC slow chargers** serve (a) cars that arrive at low battery and want a cheaper top-up, (b) overnight truck EVs (3-wheelers, light commercial EVs) as the segment grows, (c) a visible low-cost tier that pulls drivers in.
- **Named-CPO LOI [Panel kill-criterion #4]:** the EV thesis does not survive without a CPO revenue-share. Your role is landlord; CPO owns app, pricing, customer. Model 15–25% revenue-share to the landlord is the typical range (field-verify).
- **Ather Grid / Jio-bp / Zeon** are also worth approaching in parallel to Tata Power and Statiq.

### Round 3 — Spatial layout

| Element | Count | Unit footprint | Subtotal |
|---|---|---|---|
| DC fast-charge bay (car + charger pad + clearance) | 4 | 25 sqm | 100 sqm |
| AC slow-charge bay | 2 | 18 sqm | 36 sqm |
| Transformer / HT-LT panel pad (fenced, secure) | 1 | 25 sqm | 25 sqm |
| Approach + short queue lane | — | — | 40 sqm |
| Signage + CPO-branded pylon base | 1 | 6 sqm | 6 sqm |
| **Subtotal EV zone** | | | **~207 sqm** |

Plus **future-proof growth pad** for 2 extra DC bays (you will under-estimate 2030 demand): reserve **50 sqm**.

### Recommendation — EV zone

- **6 bays total (4 DC + 2 AC) at go-live.** Pad prepped for 8 bays.
- **Footprint: ~260 sqm (~2,800 sqft)** including growth pad.
- **Landlord capex ~₹10–15 L** (civil, pad, HT line extension, cable trench, transformer pad, fencing). CPO funds the chargers themselves under revenue-share.
- **Critical dependency:** one named CPO LOI before land purchase.

### The one assumption most likely to break this

**EV adoption rate on the Chennai–Pondy–Cuddalore corridor vs. your 5-year break-even.** If sessions/day stays at 8–10 instead of climbing to 25+, revenue covers electricity but not the landlord capex. Mitigant: CPO revenue-share shifts asset risk to the CPO; landlord only loses the 260 sqm of ground rent during under-utilization.

---

## Part B — Coffee Shop

### Round 1 — Baseline hypothesis

"A 700 sqft Chaayos-style café covers it."

### Check

- **Chaayos full format [F2]:** 700 sqft, mall / high-street. **Chaayos outlets don't generally offer drive-through** and are not designed for highway flow.
- **CCD Xpress [F1]:** 60 sqft kiosks — way too small to be a destination stop, useful only as drive-thru supplement.
- **Highway-café anatomy [F3]:** small built-up kitchen + large seating + restrooms are the real draw. You need more than a café; you need a **highway rest stop** with F&B as one element.

### Round 2 — Segment reality

Three customer types have three different needs. The panel's Drucker lens demands you pick a **primary** customer. The coffee shop must serve the primary with excellence and the others as spillover.

| Customer | Dwell | Ticket | Primary need |
|---|---|---|---|
| EV driver (charging for 45 min) | 40 min | ₹150–400 | Wi-Fi, clean restroom, decent coffee, seating |
| Weekend Chennai–Pondy car driver | 15–25 min | ₹200–500 | Family-friendly, clean restroom, quick food |
| Trucker | 10–15 min | ₹40–100 | Cheap chai/meal, clean restroom, clean water |
| Local (from nearby village) | variable | ₹50–150 | Affordable, somewhere to go |

The recommended primary (per Panel synthesis): **EV driver + weekend car driver** — the highest-margin dwell segment. Trucker is served via a **separate lower-cost counter and separate toilets** consistent with the Godin/Doumont segregation argument in [01-panel.md](01-panel.md).

### Round 3 — Zone breakdown

| Zone | sqft | Notes |
|---|---|---|
| Kitchen (prep + grill + storage + cold) | 300 | Supports chai, coffee, sandwiches, simple Indian meals |
| Counter / ordering / POS | 150 | Dual counter: hospitality side + trucker side |
| Indoor seating (AC) | 400 | 16 covers at ~25 sqft/cover |
| Outdoor covered seating | 400 | 16 covers, shaded for truckers + families during day |
| Premium restrooms (passenger) | 180 | Separate M / F / accessible, **this is the differentiator** |
| Trucker restrooms (volume) | 120 | Separate block near truck forecourt |
| Back-of-house storage / staff | 100 | |
| Utility (water, DG, cylinders) | 100 | Fenced rear |
| **Subtotal building footprint** | **~1,750 sqft (~163 sqm)** | |
| Forecourt parking — cars/EVs (8–10 slots @ 150 sqft) | 1,200–1,500 | Shared with EV zone |
| Pedestrian pathways + landscape | 400 | |

### Recommendation — Coffee zone

- **Building footprint: ~1,750 sqft (~165 sqm).**
- **Plus shared parking ~1,400 sqft (~130 sqm)** — combined with EV zone for efficiency.
- **Build capex (mid-quality finish): ₹15–25 L** excluding kitchen equipment (add ₹6–10 L).
- **Dual-entry design:** premium door for car/EV customers, trucker counter from the side/rear with separate toilets.

### The one assumption most likely to break this

**Daily passenger footfall.** The coffee shop economics need ~80–120 tickets/day at ₹200 average to be healthy. That requires 1,500+ light vehicles passing AND a ~5–8% stop rate AND 60%+ of stoppers buying. If light-vehicle flow is below 800/day or the stretch is a through-route with no natural stopping reason (no scenery, no town), F&B struggles regardless of quality.

Mitigant: integrate F&B as the EV dwell amenity — captive audience during charging. This shifts the F&B break-even model from "convert passers-by" to "monetise dwell time."

---

## Combined EV + Coffee Summary

| Zone | Expected footprint |
|---|---|
| EV charging | 260 sqm (2,800 sqft) |
| Coffee shop building | 165 sqm (1,750 sqft) |
| Shared car/EV parking | 130 sqm (1,400 sqft) |
| Landscape + pathways | 40 sqm (430 sqft) |
| **Subtotal hospitality zone** | **~595 sqm (~6,400 sqft)** |

Handed to [04-site-plan.md](04-site-plan.md) for consolidation with the weighbridge zone from [02-sizing-loop.md](02-sizing-loop.md).
