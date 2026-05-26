# Lovable Update Prompt — Paste This Into Lovable

Pull the latest from the GitHub repo and update the site with these changes:

## IMPORTANT: Tab Structure

The site must have **4 separate tabs** in the navigation:
1. **Buyers** — powered by `data/buyers-page.json`
2. **Investors** — powered by `data/investors-page.json`
3. **Research** — powered by `data/research-takeaways.json`
4. **Next Steps** — powered by `data/next-steps-page.json` (NEW — this is its own dedicated tab, NOT a section within Research)

**Do NOT nest the Next Steps content under the Research tab.** It must be a completely separate, standalone page accessible from the top-level navigation.

---

## 1. New Tab: "Next Steps" (4th tab — separate from Research)

Create a new top-level navigation tab called **"Next Steps"** using data from `data/next-steps-page.json`. This is a standalone page — do NOT put it inside the Research tab.

Display the following sections:

- **Phase Overview**: A horizontal timeline or stepper showing 4 project phases (Regulatory Confirmation → Design & Feasibility → Financial Commitment → Acquisition & Entitlement). Highlight "Phase 1: Regulatory Confirmation" as the current phase.
- **Immediate Actions**: Render the `immediateActions.items` array as a prioritized checklist/card layout. Each item has an `id`, `action`, `purpose`, `owner`, `priority` (CRITICAL/HIGH/MEDIUM), and `status`. Show priority with color coding (red = CRITICAL, orange = HIGH, yellow = MEDIUM). Show which items block other items using `blocksItems`.
- **Short-Term Actions**: Same card layout for `shortTermActions.items`. Show `blockedBy` dependencies as a note on each card.
- **Pre-Commitment Actions**: Same layout for `preCommitmentActions.items`.
- **Key Contacts**: Render `keyContacts.contacts` as a clean contact card grid with name, role, email (clickable mailto link where available), context, and who referred them.
- **Open Questions**: Render `openQuestions.questions` as a numbered list or table with columns: Question, Impact, Resolve With, Status. Use a badge/tag for status (open/resolved).

---

## 2. Major Update to Investors Tab

The `data/investors-page.json` has been significantly restructured (v2.0). Update the Investors tab:

- **Overall Recommendation**: Show the updated recommendation ("PROCEED WITH DILIGENCE") with the ratings array as a scorecard — each row shows category, rating badge (BUY/CONSIDER/PASS), score out of 10, and note.
- **Zoning & By-Laws Section** (NEW): Add a section before the financial scenarios titled "Zoning & By-Law Constraints". Render `zoningAndByLaws.criticalSections` as expandable cards or an accordion. Each card shows the section name, severity badge (HIGH/MEDIUM/LOW/UPSIDE with color coding), summary, and open questions. For the side setback formula, show the examples table.
- **Two Development Scenarios**: Replace the old 5-scenario layout with 2 detailed scenario cards side by side:
  - **Scenario A: Maximize Density (14 Units)** — Show unit mix table, expenses breakdown, revenue (both "Amr's Base Case" and "With Inclusionary Zoning" side by side), returns summary, and pros/cons lists.
  - **Scenario B: Luxury Large Units (5-6 Units)** — Same structure. Include Beatka's comp evidence section.
- **Head-to-Head Comparison**: Render `scenarioComparison.table` as a comparison table between the two scenarios.
- **Sensitivity Analysis** (NEW — Important): Create a dedicated section with these sensitivity tables:
  1. Scenario A: New unit $/sqft vs. profit (from `developmentScenarios[0].sensitivityAnalysis.table`)
  2. Scenario A: Purchase price vs. profit (from `developmentScenarios[0].acquisitionSensitivity.table`)
  3. Scenario B: Blended $/sqft vs. profit (from `developmentScenarios[1].sensitivityAnalysis.table`)
  4. Combined "What Breaks the Deal" matrix (from `combinedSensitivityMatrix`) showing break-even and target margin $/sqft at different purchase prices for both scenarios.
  
  Style the sensitivity tables with color gradients — green for high-margin cells, yellow for moderate, red for break-even or negative.
- **Risk Matrix**: Render `riskMatrix` as a table or card grid with probability/impact badges and mitigation text.
- **Opportunities**: Render `opportunities` as cards with probability and impact tags.
- **Comparable Sales**: Update the comps table to include the new `relevance` field as a subtitle under each address.

---

## 3. Update Research Takeaways Tab

The `data/research-takeaways.json` now has 12 findings (up from 10) with a `category` field that uses: `critical`, `positive`, `negative`, `neutral`, `opportunity`.

- Color-code findings by category: red for critical, green for positive, orange for negative, gray for neutral, blue for opportunity.
- The first two findings (Section 4.08 and Side Setback) are tagged `critical` — display them prominently at the top, perhaps with an alert/warning style.
- Update the decision framework to show the 6 new scenarios in the matrix.
- **Do NOT include Next Steps content here.** Next Steps is its own separate tab.

---

## 4. Update Buyers Tab

The `data/buyers-page.json` development vision now has two named scenarios:
- "The Heritage Collection (14 Residences)" — with `highlights` array
- "The Linden Estate (5-6 Grand Residences)" — with `highlights` array

Render the highlights as bullet points under each scenario card. The comps table now includes a `note` field for some entries — show it as a subtitle.

---

## 5. Update Property Overview

`data/property-overview.json` now includes `targetAcquisitionPrice`, `maxUnits`, `keyByLawSections`, and `transitOverlayParkingDistrict`. If any of these fields are displayed on the site, update them.

---

## Design Notes

- Keep the existing visual style and color scheme
- **4 tabs in navigation: Buyers, Investors, Research, Next Steps** — each is its own page
- Sensitivity analysis tables should be the most visually prominent new element on the Investors page — investors will focus on these
- Use the `lastUpdated` field from each JSON to show "Last updated: May 26, 2026" on each page
- The `version` field (2.0) can be shown in a footer or page header
