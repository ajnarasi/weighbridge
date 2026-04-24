# Research Log — Live Data Sources

Date compiled: 2026-04-23
Purpose: Ground the sizing loops and site plan in verifiable external data, not vibes.

Confidence legend: **[H]** high / **[M]** medium / **[L]** low / **[V]** assumption — verify on site / **[—]** no reliable source, requires local verification.

---

## A. Highway & Truck Volume Context

| # | Finding | Confidence | Source |
|---|---|---|---|
| A1 | NH-32 (formerly NH-45A) runs Marakkanam → Puducherry → Villupuram → Cuddalore → Chidambaram → Karaikal → Nagapattinam — the corridor you care about. | H | [IRB HAM project](https://www.irb.co.in/home/ham-projects/puducherry-poondiyankuppam-nh-45a-new-nh-32-project/), [MoRTH notice](https://morth.nic.in/nhai-piu-puducherry-four-laning-poondiyankuppam-km67000-sattanathapuram-km123800-section-nh-45a-0) |
| A2 | AADT estimated ~17,800 PCUs/day on Marakkanam–Puducherry corridor (FY25). | M | [NH-332A corridor brief](https://swarajyamag.com/news-brief/puducherry-to-get-rs-436-crore-elevated-corridor-to-ease-congestion-on-nh-32) |
| A3 | Villupuram–Puducherry 4-laning completed by Dilip Buildcon (Apr 2024). Marakkanam–Puducherry 4-lane HAM project (₹2,157 Cr) approved by Cabinet. | H | [DD News](https://ddnews.gov.in/en/cabinet-approves-%E2%82%B92157-crore-marakkanam-puducherry-four-lane-highway-project/), [Business Standard](https://www.business-standard.com/markets/capital-market-news/dilip-buildcon-completes-villupuram-puducherry-road-project-124042401083_1.html) |
| A4 | ₹436 Cr elevated corridor planned to relieve NH-32 congestion near Puducherry. | H | [Swarajya](https://swarajyamag.com/news-brief/puducherry-to-get-rs-436-crore-elevated-corridor-to-ease-congestion-on-nh-32) |
| A5 | Commercial vehicle share on Indian NH corridors typically 15–25% of AADT → **~2,500–4,000 trucks/day both directions** on Marakkanam–Puducherry stretch (derived). | V | Derived from A2 using MoRTH norms |
| A6 | Cuddalore = "Sugar bowl of TN" — sugar, cement (India Cements), chemicals (SIPCOT), granite, cotton, pharma flowing toward Chennai/Ennore port. | H | [Cuddalore District](https://cuddalore.nic.in/transport/) |
| A7 | Truck count at any specific plot is NOT the corridor average. You must count manually at the candidate plot for 4 weeks (weekday + weekend + Monday post-holiday). | — | Panel kill-criterion #1 |

## B. Weighbridge Tech & Regulatory

| # | Finding | Confidence | Source |
|---|---|---|---|
| B1 | Puducherry has a Dy Collector (Excise) / Dy Controller (Legal Metrology) — this is the licensing authority for commercial public weighbridges. | H | [Puducherry district](https://puducherry-dt.gov.in/dy-collector-excise-and-dy-controller-legal-metrology/) |
| B2 | Governing law: Legal Metrology Act 2009 + Legal Metrology (General) Rules 2011. Commercial weighbridges need W&M licence, periodic stamping, certified-weight calibration. | H | [Legal Metrology overview](https://genzcfo.com/growthx/weighbridge-calibration-and-legal-metrologycertification) |
| B3 | Platform-length → truck mapping: 12 m (~40 ft) = 2-axle rigid + many 14-wheelers; **18–24 m (60–80 ft) needed for tractor-semitrailers (multi-axle / 22-wheelers)**. Widths 3–3.4 m. | H | [Truck scale (Wikipedia)](https://en.wikipedia.org/wiki/Truck_scale), [Captels guide](https://pesage-captels.com/en/technic/weighbridge-and-axle-weighting-system-complete-guide-for-illuminated-selection-2/) |
| B4 | Equipment-only pricing (pitless, Indian OEMs): **60-ton ≈ ₹4 L**, 80-ton ≈ ₹4.5 L, 100-ton ≈ ₹7 L. Add civil + cabin + software + licence ≈ another ₹8–12 L. **Turnkey ₹18–25 L.** | H | [Essaar Weigh](https://www.essaarweigh.com/60-ton-weighbridge-price-in-india/), [IndiaMART 80T](https://www.indiamart.com/proddetail/80-ton-pitless-weighbridge-19889516188.html), [CUBLiFT 100T](https://www.cublift.com/100-ton-weighbridge/) |
| B5 | Pitless > pit-mounted for greenfield highway site: less civil work, no water-logging, easier maintenance. | H | [CUBLiFT](https://www.cublift.com/60-ton-weighbridge/) |
| B6 | 100-ton pitless platforms come in 3 m / 3.4 m widths and 16–24 m lengths — modular. | H | [CUBLiFT 100T](https://www.cublift.com/100-ton-weighbridge/) |
| B7 | Public-weighment fee per truck and daily throughput at operating weighbridges on TN/PY highways. | — | No open source — visit 3 existing weighbridges within 8 km, pay, time, and observe (panel diligence Q2) |

## C. Puducherry EV Charging Policy & Incentives

| # | Finding | Confidence | Source |
|---|---|---|---|
| C1 | PM E-DRIVE replaced FAME II in Oct 2024; runs through Mar 2026; ₹2,000 Cr earmarked for ~72,000 chargers nationally. | H | [PM E-DRIVE](https://pmedrive.heavyindustries.gov.in/), [ICCT](https://theicct.org/wp-content/uploads/2024/10/ID-239-%E2%80%93-E-DRIVE-charging_final.pdf) |
| C2 | DISCOMs mandated to supply up to 150 kW connections to public charging stations on expedited timelines. | H | [Exicom policy brief](https://www.exicom.com/insights/blogs/these-policies-scaled-ev-charging-in-india-2025) |
| C3 | BEE guideline: public EV charger every 25 km on national highways. | H | [BEE 2024 guidelines](https://beeindia.gov.in//guidelines-for-installation-and-operation-of-electric-vehicle-charging-infrastructure-2024) |
| C4 | **Puducherry has the lowest Level 2 charger density among Indian states/UTs.** Undersupply signal — but also means low benchmark-demand evidence. | M | [India EV landscape 2025](https://www.anariev.com/india-ev-charging-station-landscape/), [IndiaDataMap](https://indiadatamap.com/2025/11/13/ev-charging-stations-in-india/) |
| C5 | No Puducherry-UT-specific EV policy document surfaced via open search. | — | Requires direct query to Puducherry Transport / Electricity Dept. |
| C6 | Typical public station footprint: **~500 sqft for 3–4 car bays.** | H | [1charging guide](https://1charging.com/setup-ev-charging-station-cost-requirements-maintenance/) |
| C7 | 60 kW DC dual-gun is the workhorse for highway sites. 240 kW "megachargers" are appearing (Tata.ev). | H | [Statiq 60kW](https://www.statiq.in/60kw), [Tata Motors megacharger](https://www.tatamotors.com/press-releases/tata-ev-accelerates-indias-ev-journey-with-launch-of-10-tata-ev-megachargers/) |
| C8 | 55–75 kVA transformer suffices for a small fast-charger cluster (~₹1 L). Full public station (4–5 chargers, transformer, HT cables, safety, civil) **₹24–50 L** excl. land. | H | [1charging](https://1charging.com/setup-ev-charging-station-cost-requirements-maintenance/), [Lendingkart](https://www.lendingkart.com/blog/cost-estimates-o-ev-public-charging-station/) |
| C9 | National co-location pattern: Tata Power EZ Charge (5,500+ stations), Statiq, ChargeZone, Ather Grid all co-locate at highway dhabas — charging + restroom + café + store is the norm. | H | [Tata Power EZ Charge](https://www.tatapower.com/ezcharge), [Statiq at dhabas](https://www.statiq.in/) |

## D. Puducherry Land Rates & Zoning

| # | Finding | Confidence | Source |
|---|---|---|---|
| D1 | Bahour commercial plot (21,600 sqft) listed ₹4.32 Cr → **~₹2,000/sqft → ~₹87 L/acre** for listed commercial on outskirts. | M | [99acres commercial](https://www.99acres.com/commercial-property-in-pondicherry-ffid) |
| D2 | Bahour agricultural land listed at ~₹9/sqft (not usable without NA conversion). | M | [Waa2](https://property.waa2.in/for-sale/agriculture-land-in-pondicherry) |
| D3 | Ariyankuppam / Barathi Nagar has premium commercial-and-institutional plots with multiple access roads — likely 2×+ Bahour rates. | M | [99acres Ariyankuppam](https://www.99acres.com/residential-land-in-ariyankuppam-pondicherry-ffid) |
| D4 | Kamaraj Nagar (Pondy city) ≈ ₹10,000/sqft — NOT your target. Mentioned for benchmark only. | H | [99acres](https://www.99acres.com/commercial-property-in-pondicherry-ffid) |
| D5 | ECR near Pondy = beachside premium (Auroville, malls). Expensive per sqft; wrong customer mix for trucker weighbridge. | M | [99acres ECR plots](https://www.99acres.com/residential-land-in-ecr-pondicherry-ffid) |
| D6 | NA (non-agricultural) conversion required before any commercial build. Process runs through Puducherry Revenue Dept. | V | Standard UT/TN process — confirm with local advocate |

## E. NHAI Setback / Right-of-Way

| # | Finding | Confidence | Source |
|---|---|---|---|
| E1 | No construction within 40 m of NH centreline (≈ to NH boundary) — anything built inside can be demolished without compensation. | H | [Moneylife](https://www.moneylife.in/article/new-guidelines-on-anvil-for-building-construction-near-highways/54129.html), [NH Rules 1957](https://wbpwd.gov.in/files/contents/acts_rules/nh_rules_1957.pdf) |
| E2 | NHAI raised minimum wayside construction setback to **7.5 m from boundary stones**; construction in 5–7 m only with demolition-affidavit. | H | [Construction World](https://www.constructionworld.in/transport-infrastructure/highways-and-roads-infrastructure/nhai-to-raise-minimum-distance-of-wayside-construction-to-7.5-m/29030) |
| E3 | NHAI No-Objection-Certificate is **mandatory** for highway-frontage commercial access — access permissions are NHAI-gated. | H | [MoRTH guidelines PDF](http://morth.gov.in/sites/default/files/circulars_document/Revised%20guidelines%20%20Norms%20for%20access%20permission%20(3)_compressed_compressed%20(1)_reduce.pdf) |
| E4 | Commercial-establishment minimum distance from NH: historically 6 m (pre-revision). | M | [NoBroker forum](https://www.nobroker.in/forum/how-close-can-you-build-to-a-highway/) |

## F. Coffee / F&B at Highway Locations

| # | Finding | Confidence | Source |
|---|---|---|---|
| F1 | CCD Xpress kiosks are **~60 sqft** — too small for a highway format, useful only as a drive-thru counter. | H | [CCD outlet range](https://www.cafecoffeeday.com/about-us/range-of-outlets) |
| F2 | Chaayos full café = **~700 sqft** (malls / high-street); franchise units 200–400 sqft. | H | [Chaayos locator](https://chaayos.com/pages/cafe-locator), [Kouzina franchise](https://www.kouzinafoodtech.com/blog/chaayos-franchise) |
| F3 | Highway café anatomy: small built-up kitchen + large open seating + outdoor/semi-covered area. Restrooms are often the real draw, especially for truckers and families. | M | [Vibes of India](https://www.vibesofindia.com/those-friendly-cafes-on-sg-highway/) |
| F4 | Typical dhaba + charger co-location in India is the dominant pattern for highway stops today (Punjab NH-1, Haryana NH-7, Rajasthan NH-8 case studies). | H | [Statiq at dhabas](https://www.statiq.in/Statiq-Virsa-Dhaba-Station-ev-charging-station-id-8149) |

---

## Gaps explicitly flagged as "requires local verification"

- Puducherry EV policy document (UT-level) — direct query to Transport / Electricity Dept required.
- Per-truck weighment fee and daily throughput on NH-32 / ECR — field visit to 3 nearby weighbridges.
- Specific-plot truck count at the candidate location — 4-week manual count (weekday + Saturday + Monday post-holiday).
- Circle rate / guideline value for the exact revenue-village of the candidate plot — from Puducherry Registration Dept.
- Whether any named CPO (Tata Power / Statiq / ChargeZone / Ather) will sign a site LOI before land purchase.
- NHAI 2030 master plan alignment check for the Pondy corridor — any proposed bypass will kill the plot's value.

These gaps are the *most important* data points; the open-web has none of them. Your field diligence, not further desk research, is the blocker from here.
