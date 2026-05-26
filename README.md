# 19 Linden St, Brookline Village — Development Feasibility Study

Residential development research and investor materials for the property at **19 Linden Street, Brookline Village, MA**.

## Property Snapshot

| Detail | Value |
|---|---|
| Address | 19 Linden St, Brookline Village, MA |
| Lot Size | 17,698 sq ft (~0.41 acres) |
| Zoning | M-1.0 (Multi-family, FAR 1.0) |
| Max Units (density formula) | 15 |
| Current Structure | 1843 Greek Revival (National Register) |
| Asking Price | $5,950,000 |
| Target Acquisition | $5,500,000 |

## Development Scenarios Under Analysis

| | Scenario A: Density (14 units) | Scenario B: Luxury (5-6 units) |
|---|---|---|
| Revenue (IZ-adjusted) | ~$20.8M | ~$18-21M |
| Estimated Profit | ~$5.3M | ~$2.6-5.0M |
| Margin | 25.4% | 14-25% |
| Timeline | 4 years | ~3.5 years |

## Landing Page Structure (for Lovable)

The `data/` directory contains structured JSON files for four landing page sections:

### Section 1: Buyers Page (`buyers-page.json`)
Property presentation for potential end-buyers — aspirational, visual, focused on lifestyle and location. Includes two development vision scenarios and comparable sales.

### Section 2: Investors Page (`investors-page.json`)
Decision-support dashboard with two detailed financial scenarios (Amr's 14-unit density plan vs. Beatka's 5-6 unit luxury plan), by-law constraints analysis, sensitivity tables, risk matrix, and recommendations.

### Section 3: Research Takeaways (`research-takeaways.json`)
Distilled findings: 12 key takeaways with by-law deep dive, regulatory implications, and an updated decision framework matrix.

### Section 4: Next Steps (`next-steps-page.json`)
Action items organized by phase (immediate, short-term, pre-commitment), key contacts, open questions tracker, and project timeline.

## Repository Structure

```
data/
  property-overview.json       # Core property data
  buyers-page.json             # Section 1: Buyer-facing presentation
  investors-page.json          # Section 2: Investor decision support (v2)
  research-takeaways.json      # Section 3: Key findings & by-law analysis (v2)
  next-steps-page.json         # Section 4: Action items & timeline (NEW)
research/
  zoning-and-entitlements.md   # M-1.0 zoning deep dive
  historic-preservation.md     # National Register & local constraints
  neighborhood-context.md      # Brookline Village market context
  financial-analysis.md        # Original pro forma scenarios (v1)
  development-strategies.md    # Four development paths compared (v1)
  refined-analysis-v2.md       # Updated analysis with by-law findings (v2)
New info/
  19 Linden St Brookline Financials.pdf  # Amr's financial model
  Input from agent1.PNG                  # Beatka's development recommendations
  Input from agent2.PNG                  # Beatka's pricing estimates
  Amr input on by-laws and number of units.PNG  # Amr/Beatka by-law discussion
  Number of units_Amr's analysis.png     # Amr's unit mix spreadsheet
  Zoning by-law.PNG                      # Emily Noel's regulatory guidance
assets/
  IMG_8541.PNG                 # Original property communication
```

## Quick Start for Lovable

1. Import this repo into Lovable
2. The four JSON files in `data/` map directly to the four page sections
3. Each JSON has a `page` field identifying which section it powers
4. The `research/` markdown files contain supporting detail if you want deeper content pages

## Key By-Law Sections to Know

| Section | What It Does | Impact |
|---|---|---|
| **4.08** | Inclusionary zoning — 15% affordable units for 4+ unit projects | Reduces revenue by $500K-2.2M |
| **5.21** | Public benefit incentive — FAR/height exceptions for community benefits | Potential upside if preservation qualifies |
| **6.02** | Parking — Transit Overlay reduces to 1 space/unit | Saves $350-700K in garage costs |
| **Table 5.01** | Dimensional requirements — side setback = Length/10 + 10 ft | Constrains building envelope |
