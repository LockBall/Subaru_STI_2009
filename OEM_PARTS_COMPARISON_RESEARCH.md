# Subaru OEM Parts Analysis and Alternative Comparison Research

Date: 2026-07-16
Scope: broadened research across core maintenance parts for 2009 STI (EJ257), using an evidence-first approach.

## Purpose

Build a reusable, source-ranked framework to compare OEM Subaru parts against alternatives without relying on weak claims.

## Evidence quality ladder

1. OEM/manufacturer technical documents (Subaru, NGK, Denso, WIX, etc.)
2. Standardized test reports or directly attributable lab data (ISO/SAE method shown)
3. Structured catalog specifications from established catalogs
4. Independent teardown or measured tests with transparent method
5. Community/forum reports and reseller/blog claims

Decision rule:
- Do not mark an aftermarket part as "better" unless categories 1-3 provide direct, comparable metrics.

## Parts to compare

- Oil filter (fully consolidated in `OIL_FILTER_RESEARCH.md`)
- Engine air filter (`16546AA12A` vs alternatives)
- Cabin air filter (`72880FG000` vs alternatives)
- Spark plugs (`22401AA670` / NGK SILFR6A vs equivalents)
- Oxygen sensors (`22641AA510`, `22690AA850` vs Denso/NTK alternatives)
- Drain plug washer (`11126AA000`, `037010000` vs generic washers)

## Preliminary broad-search findings

### Oil filter
- All oil-filter-specific findings, sources, conclusions, supersession chain, and watchlists are maintained in `OIL_FILTER_RESEARCH.md` to avoid duplication.

### Engine air and cabin filters
- Broad web results are dominated by generic blogs, retailer content, and forum opinions.
- There is limited Subaru-specific, controlled comparison data in top indexed results.
- Need to focus on fitment dimensions, media type, and pressure-drop/efficiency data from brand tech docs.

### Spark plugs
- OEM fitment linkage to NGK SILFR6A is clear in Subaru parts catalog references.
- Broad web results contain many low-authority comparison pages.
- Counterfeit risk signal is high; sourcing integrity matters as much as brand choice.

### Oxygen sensors
- Strong recurring theme: OEM-equivalent supplier selection (Denso/NTK/Bosch by application) matters more than generic aftermarket picks.
- Broad results are again opinion-heavy; must verify exact sensor type and connector/calibration by part number/VIN.

### Crush washers
- Broad results are mostly forum/mechanic anecdotes and generic copper-vs-aluminum writeups.
- Practical takeaway from broad signal: prioritize correct dimensions/material and one-time-use sealing behavior over brand marketing.

### Counterfeit risk
- Counterfeit spark plugs and filters are repeatedly discussed across communities.
- Practical sourcing control should be part of every comparison.

## High-confidence source targets by part type

### Oil filter
- See `OIL_FILTER_RESEARCH.md` (canonical oil filter source in this workspace).

### Engine air and cabin filters
- Subaru OEM part pages and dimensions
- Official manufacturer technical docs for alternatives
- Any standard-method filtration/pressure-drop data

### Spark plugs
- Subaru OEM part pages (exact part mapping)
- NGK official part/spec and anti-counterfeit guidance
- Denso/other equivalent manufacturer spec pages for exact alternative candidates

### Oxygen sensors
- Subaru OEM part pages by position (upstream/downstream)
- Denso/NTK official catalog cross-reference by exact OE number
- Avoid universal sensors unless engineering justification is explicit

### Crush washers
- OEM dimensions/material references from Subaru part pages and parts diagrams
- Reputable engineering references for washer material behavior

## Research backlog (next targeted passes)

1. Build part-by-part comparison tables with only category 1-3 sources.
2. Add "unknown" fields explicitly where Subaru or manufacturers do not publish values.
3. Add source confidence per row and exclude unverified claims from conclusions.
4. Add sourcing guidance section (authorized channels, counterfeit red flags).

## Current conclusion

A broadened search confirms that:
- useful signal exists, but much of the indexed web is low-authority opinion content,
- authoritative, directly comparable technical data is uneven across part categories,
- OEM remains the baseline when key performance metrics are not publicly published for fair comparison.
