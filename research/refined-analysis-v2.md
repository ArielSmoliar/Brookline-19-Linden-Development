# Refined Analysis: 19 Linden St — v2 (May 2026)

Updated model incorporating Amr's financial spreadsheet, Beatka Zakrzewski's agent input, Emily Noel's (Building Inspector) regulatory guidance, and by-law research.

---

## What Changed From the Original Model

| Factor | Original Model (v1) | Amr's Model | Delta |
|---|---|---|---|
| **Purchase price** | $5,950,000 ask / $4,500,000 target | $5,500,000 | Negotiated ~$450K off ask |
| **Unit count** | 14-16 generic | 14 (2 existing + 12 new 1,000 sqft) | Same count, different mix |
| **Unit mix** | Uniform ~1,100 sqft | 1x 3,000sf + 1x 1,200sf (existing) + 12x 1,000sf (new) | Small-unit strategy |
| **Sale price/sqft** | $1,100-$1,300 | $1,200 (existing) / $1,500 (new small units) | Higher $/sqft for smaller units |
| **Total revenue** | $16.5M-$19.2M | $23,040,000 | +$4-6.5M revenue |
| **Building cost** | $500/sqft | $498/sqft ($7,048K build + $1,200K finishes) | Comparable |
| **Other costs** | $1.95M soft costs | $644K other + $1,152K selling | Different breakdown |
| **Profit (project)** | -$960K to +$1.6M | $7,496,000 | Dramatically higher |
| **Project IRR** | Not calculated | 48.22% | — |
| **Investor returns** | Not calculated | $3,647,736 net cash / 23.61% annual over 4 yrs | — |
| **Inclusionary zoning** | Not modeled | Not modeled | **BOTH MISSED THIS** |
| **Parking** | "Confirm" placeholder | Not broken out | **Needs quantifying** |

### Why Amr's Revenue Is So Much Higher

The entire gap comes from the **small-unit premium strategy**: 12 units at 1,000 sqft priced at **$1,500/sqft** = $18M of the $23M total. Our original model priced everything at $1,100-1,300/sqft.

**Is $1,500/sqft realistic?** Comp support:
- 58 Kent St (2025): 1,217 sqft, 2BR/2BA → **$1,396/sqft** (sold)
- Solaire Fisher Hill: 3,000-4,000 sqft → $1,000-1,333/sqft
- Brookline Village median resale: $830/sqft (+29.3% YoY)

$1,500/sqft is at the top of market for new construction. Achievable but not conservative. See sensitivity analysis below.

### FAR Overage Flag

Amr's total is 17,860 sqft on a 17,698 sqft lot (FAR 1.0). That's **162 sqft over the FAR limit**. Needs to be trimmed — either reduce unit sizes slightly or reduce common space from 1,660 to ~1,500 sqft.

---

## By-Law Deep Dive

### Section 4.08 — Inclusionary / Affordable Housing (CRITICAL)

**Source:** Brookline Zoning By-Law § 4.08; Brookline Housing Division

**This was not in either model and materially changes the economics.**

| Rule | Detail |
|---|---|
| **Trigger** | 4+ residential units (new construction or conversion) |
| **Requirement** | 15% of units must be Affordable Units on-site |
| **Bedrooms** | 15% of total bedrooms must also be in affordable units |
| **Income target (for-sale)** | ≤ 80% Area Median Income (AMI) |
| **Income target (rental)** | ≤ 50% AMI |
| **Alternative** | Cash payment in-lieu to Brookline Housing Trust |

**Impact on a 14-unit for-sale project:**
- 15% × 14 = **2.1 units** → likely 2 affordable units (rounding rules need confirmation with Planning Dept.)
- Those 2 units sell at deed-restricted 80% AMI pricing, **not** market rate
- Estimated affordable sale price: ~$350-450K per unit (vs. $1,200-1,500K market) depending on bedroom count and current AMI limits
- **Revenue reduction**: ~$1.5-2.0M vs. Amr's all-market-rate model
- **Payment-in-lieu alternative** may be preferable — need to confirm the per-unit fee

**Impact on a 5-unit project (Beatka's plan):**
- 15% × 5 = **0.75 units** → likely 1 affordable unit (or payment-in-lieu)
- Smaller hit but still a factor

**Action item:** Confirm with Planning Dept: (1) exact rounding rules, (2) current payment-in-lieu amount, (3) whether the $25,000 "rebate for A9" noted in Amr's spreadsheet relates to this.

---

### Side Setback — "Length / 10 + 10" Formula

**Source:** Emily Noel, Building Inspector; Brookline Zoning By-Law Table 5.01

The building inspector stated the side setback formula for M districts is:

> **Side setback = (Building length ÷ 10) + 10 feet**

This is more restrictive than we assumed (7.5-10 ft in the original model). It's a **sliding scale** — longer buildings require wider side yards.

| Building length | Required side setback | Both sides combined |
|---|---|---|
| 60 ft | 16 ft | 32 ft |
| 80 ft | 18 ft | 36 ft |
| 100 ft | 20 ft | 40 ft |
| 120 ft | 22 ft | 44 ft |

**What this means:** We need the **lot width** (not just lot area) to determine the maximum building width. If the lot is, say, 90 ft wide:
- 80 ft building → 36 ft in setbacks → 54 ft remaining → building can be 54 ft wide
- 100 ft building → 40 ft in setbacks → 50 ft remaining → building can be 50 ft wide

This constrains the **footprint** of the new construction. An architect needs to test whether 14 units + underground garage + the existing house all fit within this envelope.

**Action item:** Get a lot survey to confirm width/depth dimensions, then model buildable envelope.

---

### Maximum Height — 40 ft (Confirmed)

M-1.0 district max height: **40 feet** = 4 stories feasible.

At 4 stories with the FAR cap:
- 17,698 sqft GFA ÷ 4 floors = ~4,425 sqft per floor footprint needed

At 3 stories:
- 17,698 ÷ 3 = ~5,900 sqft per floor footprint — may be tight given setback constraints

**4 stories is the right design target** to keep the footprint manageable.

---

### Rear Setback — 30 ft (Confirmed)

Minimum rear yard: **30 feet** for M-1.0 multifamily districts.

This eats into the buildable depth. Combined with front setback (10-20 ft) and rear (30 ft), you lose 40-50 ft of lot depth before you start building.

---

### Section 5.21 — Public Benefit Incentive (Potential Upside)

Section 5.21 allows **exceptions to FAR and height** in exchange for public benefits. This could be relevant if:
- The project preserves the historic house (public benefit = preservation)
- The project includes affordable units beyond the 15% minimum
- The project provides community amenities

**This needs architect/attorney review.** If activated, could allow FAR > 1.0 or height > 40 ft, unlocking more sellable sqft.

**Action item:** Discuss with Ted Murray (Building Inspector, emurray@brooklinema.gov) whether Section 5.21 could apply to this project.

---

### Section 6 — Parking Requirements

**Source:** Brookline Zoning By-Law § 6.02; 2021 Transit Overlay amendment

| Unit type | Standard requirement | Transit Overlay (within 0.5mi of Green Line) |
|---|---|---|
| Studio | 1.0 space | 0.5 spaces |
| 1 BR | 1.4 spaces | 1.0 space |
| 2 BR | 2.0 spaces | 1.0 space |
| 3+ BR | 2.0 spaces | 1.0 space |

**19 Linden St is ~5 min walk from Brookline Village Green Line D station — almost certainly qualifies for the Transit Overlay District.**

| Scenario | Standard parking | Transit Overlay parking |
|---|---|---|
| Amr's 14 units (assume mix of 1-2BR) | ~21-28 spaces | ~14 spaces |
| Beatka's 5 units (assume 3BR+) | ~10 spaces | ~5 spaces |

**Underground garage cost estimate:**
- 14 spaces × $75-100K/space = **$1.05-1.4M**
- 5 spaces × $75-100K/space = **$375-500K**

**Is this in Amr's budget?** His building cost is $7,048,000. At $498/sqft for 17,860 sqft, the parking garage could be embedded in the building cost — but it's not broken out. Both Amr and Beatka assume underground parking with elevator access. This needs explicit confirmation.

**Action item:** Confirm Transit Overlay District boundary includes this parcel. Break out parking cost in the pro forma.

---

### 18-Month Demolition Delay

Emily Noel confirmed the **18-month demo delay may apply** — "reach out to the preservation department."

This is consistent with our original analysis. Key nuance from the building inspector: the preservation department can help navigate the timeline.

**For adaptive reuse (keeping the existing house):** The delay may be **avoided entirely** — no demolition = no delay. This is the single biggest schedule advantage of the adaptive reuse approach.

**For full demolition:** 18 months of carry cost at $5.5M acquisition = ~$660K (at 8% interest).

---

## Two Refined Scenarios

Both scenarios incorporate the by-law findings above. Both agree on: **keep the existing house, underground garage, avoid 40B.**

### Scenario A: Amr's Plan — Maximize Density (14 Units)

| Component | Detail |
|---|---|
| **Concept** | Keep existing house as 2 units (3,000 + 1,200 sqft). Build 12 new ~1,000 sqft units behind/adjacent. Underground garage. |
| **Units** | 14 total (2 existing + 12 new) |
| **Total GFA** | ~17,700 sqft (must stay ≤ 17,698 for FAR 1.0) |
| **Purchase** | $5,500,000 |
| **Building** | $7,048,000 |
| **Unit finishes** | $1,200,000 |
| **Other costs** | $644,000 |
| **Selling** | $1,152,000 |

**Open question on the "Existing 1,200 sqft unit":** Amr's model shows two existing units (3,000 + 1,200 sqft) carved from what's described everywhere as a single Greek Revival house. Is Amr assuming the house gets subdivided (e.g., basement apartment, carriage house, or attic unit)? This needs confirmation because: (a) it's $1.44M of revenue that depends on feasibility of the split, and (b) splitting a National Register building may trigger the demolition delay if interior work requires significant exterior changes (the "systematic removal of character-defining elements" clause). **Clarify with Amr and the preservation department.**

**Revenue — Amr's Base Case (all market rate):**

| Unit type | Sqft | $/sqft | Revenue |
|---|---|---|---|
| Existing 3,000 sqft | 3,000 | $1,200 | $3,600,000 |
| Existing 1,200 sqft | 1,200 | $1,200 | $1,440,000 |
| 12 × 1,000 sqft new | 12,000 | $1,500 | $18,000,000 |
| **Total** | **16,200** | | **$23,040,000** |

**Revenue — Adjusted for Section 4.08 (2 affordable units):**

Assuming 2 of the 12 new units are deed-restricted at ~$400K each instead of $1,500K:

| Unit type | Sqft | $/sqft | Revenue |
|---|---|---|---|
| Existing 3,000 sqft | 3,000 | $1,200 | $3,600,000 |
| Existing 1,200 sqft | 1,200 | $1,200 | $1,440,000 |
| 10 × 1,000 sqft (market) | 10,000 | $1,500 | $15,000,000 |
| 2 × 1,000 sqft (affordable) | 2,000 | ~$400 | $800,000 |
| **Total** | **16,200** | | **$20,840,000** |

**Revenue reduction from IZ: ~$2.2M**

| Metric | Amr's Base | With IZ Adjustment |
|---|---|---|
| Revenue | $23,040,000 | $20,840,000 |
| Total costs | $15,544,000 | $15,544,000 |
| Profit | $7,496,000 | $5,296,000 |
| Margin | 32.5% | 25.4% |

Still a strong deal — but $2.2M less than Amr's model shows. And this assumes $1,500/sqft holds.

**Sensitivity on $/sqft for the 10 market-rate new units (with IZ adjustment):**

| New unit $/sqft | New unit revenue | Total revenue | Profit | Margin |
|---|---|---|---|---|
| $1,200 | $12,000,000 | $17,840,000 | $2,296,000 | 12.9% |
| $1,350 | $13,500,000 | $19,340,000 | $3,796,000 | 19.6% |
| $1,500 | $15,000,000 | $20,840,000 | $5,296,000 | 25.4% |
| $1,650 | $16,500,000 | $22,340,000 | $6,796,000 | 30.4% |

**The deal works at $1,200/sqft or higher, even with inclusionary zoning.**

---

### Scenario B: Beatka's Plan — Luxury Large Units (5-6 Units)

| Component | Detail |
|---|---|
| **Concept** | Existing house as 1 single-family attached home. Add a townhouse + 3-4 attached flats. Underground garage with elevator. |
| **Units** | 5-6 total |
| **Unit size** | ~3,500 sqft each (if 5 units) |
| **Total GFA** | ~17,500 sqft |
| **Target sell-out** | ~$20M (Beatka's estimate) |

**Revenue model (5 units at ~3,500 sqft):**

| Unit type | Sqft | $/sqft | Revenue |
|---|---|---|---|
| Existing house (flagship) | 3,500 | $1,300 | $4,550,000 |
| 4 × new luxury units | 14,000 | $1,200 | $16,800,000 |
| **Total** | **17,500** | | **$21,350,000** |

Note: Beatka estimated ~$20M. At $1,200/sqft blended this comes in at ~$21M. Smaller units would command higher $/sqft but Beatka's strategy is fewer, larger luxury units.

**Section 4.08 impact:** 15% × 5 = 0.75 → likely 1 affordable unit, or payment-in-lieu. Revenue impact: ~$500K-800K reduction, or a cash fee. Much smaller hit than Scenario A.

**Pros vs. Scenario A:**
- Simpler construction, fewer units to sell
- Lower parking count (5 vs 14 spaces)
- Less community opposition ("small responsible development")
- Less IZ impact (1 unit vs 2)
- Beatka's comp knowledge: sold 40 Kent + 40 Webster Place (1 block away), both NR-listed

**Cons vs. Scenario A:**
- ~$2-3M less total revenue
- Only maximizes value if $1,200+/sqft holds for 3,500 sqft units (larger units historically sell at lower $/sqft)
- Fewer units = less diversification of buyer risk
- Does not maximize density allowance (5 vs 15 possible units)

---

## Amr's Investor Cash Flow Model (From Spreadsheet)

| Line item | Amount |
|---|---|
| Sale + rent income | $23,065,000 |
| Return construction loan | -$14,392,000 |
| Selling/broker fees | -$1,162,000 |
| Investment Cash - Acquisition | ~$1,100,000 |
| Investment Cash - Construction Interest | ~$2,763,000 |
| Return investor cash | ~-$3,863,000 |
| **Net Free Cash Inflow** | **$3,647,736** |
| **Net Cash to Investors** | **$3,647,736** |
| **Target Return** | **94.42%** |
| **Years** | **4** |
| **Annual Return** | **23.61%** |

**Important notes:**
- This model does NOT account for Section 4.08 inclusionary zoning. Adjusted investor returns would be ~$1.5-2M lower. Still strong but needs updating.
- The **23.61% annual return is a leveraged return** to equity investors. Amr's model assumes a ~$14.4M construction loan with ~$3.9M of investor equity. The unlevered project return is 12.06% annual (48.22% over 4 years). The leverage amplifies returns to investors but also amplifies risk — if revenue falls, equity takes the first loss.

---

## Open Questions That Block Finalizing Numbers

### Must-Confirm (Before Closing)

1. **Section 4.08 rounding rules** — Is 2.1 units rounded to 2 or 3? What's the current payment-in-lieu amount? Contact Planning Dept.
2. **Transit Overlay District boundary** — Confirm 19 Linden is within 0.5 miles of Brookline Village station (almost certainly yes, but verify the official map)
3. **Lot dimensions (width × depth)** — Need survey to model buildable envelope with side setback formula. The 17,698 sqft lot area alone isn't enough.
4. **Side setback: confirm formula** — "Length / 10 + 10" per Emily Noel. Verify in Table 5.01 and confirm it applies to M-1.0.
5. **Parking cost breakout** — Is underground garage costed within Amr's $7M building number? If not, add $1-1.4M.
6. **Section 5.21 applicability** — Can preservation of the Greek Revival house qualify as a "public benefit" for FAR/height bonus?
7. **80% AMI sale price** — What does a 1,000 sqft deed-restricted unit at 80% AMI actually sell for in Brookline's current AMI tables?

### Should-Confirm (Before Design)

8. **Front setback** — Confirm exact depth from Table 5.01 (estimated 10-20 ft)
9. **Usable open space per unit** — Confirm from Table 5.01
10. **Demo delay for partial renovation** — If keeping the house but substantially renovating, does the "25% of exterior" trigger apply? Consult preservation dept.
11. **Section 6 bicycle parking** — New requirements may apply
12. **Affordable housing plan form** — Must be submitted; Brookline has specific guidelines (updated Sept 2024)

### Meeting Recommendations (from Emily Noel)

- **Ted Murray** (Building Inspector): emurray@brooklinema.gov — set up meeting to walk through Sections 4.08, 5.21, 6, and Table 5.01
- **Preservation Department**: discuss demo delay applicability for adaptive reuse approach
- Review these by-law sections before the meeting: 4.08, 5.21, 6

---

## Updated Recommendation

**Both scenarios work** — Amr's density play and Beatka's luxury play are both viable, and both are stronger than the original v1 model because they anchor on **keeping the existing house** (avoiding the 18-month demo delay and reducing community opposition).

**The inclusionary zoning requirement (Section 4.08) is the single biggest factor neither model originally accounted for.** It reduces Amr's revenue by ~$2.2M and Beatka's by ~$500-800K. The deal still works in both cases, but the pro forma must be updated.

**Near-term priorities:**
1. Meet with Ted Murray to confirm by-law specifics (setbacks, IZ rounding, Section 5.21)
2. Get a lot survey (width/depth) to model the buildable envelope
3. Update Amr's spreadsheet with IZ adjustment and parking cost breakout
4. Decide between Scenario A (14 units, higher revenue, more complexity) vs Scenario B (5-6 units, simpler, lower risk, lower return)

---

*Sources: Brookline Zoning By-Law §§ 4.08, 5.21, 6.02; Emily Noel (Building Inspector); Amr's financial model; Beatka Zakrzewski (agent); Brookline Housing Division inclusionary zoning guidelines*
