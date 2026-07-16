# Oil Filter Research for 2009 STI (EJ257)

Date: 2026-07-16

Canonical file note:
- This is the single consolidated file for all oil filter research and references in this workspace.

## Research question
Can we identify an oil filter that is objectively better than OEM Subaru 15208AA100 for this engine?

## Method
Compared filters on:
- bypass valve setting
- filtration efficiency claim
- media type
- anti-drainback valve
- fit specs (thread and gasket)

Prioritized manufacturer/catalog spec pages over forum claims.

## Oil filter bypass pressure (core concept)

Oil filter bypass pressure is the pressure difference across the filter media at which the filter bypass valve opens.

It is not the same as engine oil pressure. It is differential pressure between filter inlet and outlet.

Why this matters for the 2009 STI EJ257:
- Cold starts increase oil viscosity, which raises restriction through the filter media. A correctly calibrated bypass helps maintain rapid oil flow to bearings and turbo while oil is thick.
- Turbocharged, high-load operation increases oil flow demand. Filter behavior under high demand affects how often oil is filtered versus bypassed.
- If bypass pressure is too low, the valve can open too easily and allow more unfiltered oil circulation.
- If bypass pressure is too high, restriction can remain elevated too long during cold or high-demand conditions before bypass opens.

Practical takeaway:
- Use OEM or a proven equivalent that explicitly matches OEM bypass behavior for EJ257 application.
- Do not rely on thread/gasket fit alone when selecting an aftermarket filter.

## OEM bypass pressure evidence (deep sweep)

Goal: identify a numeric bypass relief valve setting for Subaru OEM filter family `15208AA100` / `SOA6351520812` / `15208AA12A`.

### Evidence table

| Source type | Source | What it provides | Numeric bypass value present? | Confidence |
|---|---|---|---|---|
| Official Subaru parts listing | https://parts.subaru.com/p/Subaru__/OIL-FILTER-COMPLETE/120988245/SOA6351520812.html | Confirms supersession (`15208AA100`, `15208AA12A`), generic feature text: spring-loaded relief valve | No | High for part identity; High confidence that no numeric value is published there |
| Official Subaru dealer network pages (same SimplePart content family) | Example: https://parts.subaru.com/p/Subaru_2009_STI/Oil-Filter-Complete/49227636/15208AA100.html | Fitment, supersession, marketing description | No | High for fitment; low for numeric spec because absent |
| Subaru/NHTSA bulletin mirrors for `15208AA12A` | https://oemdtc.com/tsb/10067860/ and https://oemdtc.com/tsb/10232860/ | Bulletin metadata and downloadable PDF links; no extracted numeric bypass spec from accessible HTML content | No confirmed numeric value in accessible extracted text | Medium (metadata reliable; numeric spec not confirmed) |
| OEM product photos (can + box labels) | Multi-source images (SubaruPartsDeal/STM/Flatirons product photos) | Confirms printed part number, maker markings, warnings/instructions | No visible PSI/bar bypass value printed on can/box in retrieved images | Medium-High |
| Structured aftermarket catalog cross-reference | WIX 57055: https://www.rockauto.com/en/moreinfo.php?pk=4768758 and https://www.wixfilters.com/en-nz/catalog/results/product.html/57055_wix.html | Explicit bypass values for WIX equivalent (27 psi, 1.9 bar) | Yes (aftermarket only) | Medium-High |
| Community/forum measured claims | Example search hits (BITOG/NASIOC/SubaruOutback threads) | User-measured or discussed OEM bypass values (often around low-20s to high-20s psi) | Yes, but not OEM published documentation | Low |

### Hard conclusion from this deeper pass

- No official Subaru source retrieved in this pass publishes a numeric bypass relief valve pressure for `15208AA100` / `SOA6351520812` / `15208AA12A`.
- Best-supported statement is therefore: the OEM bypass setting is not publicly published in the accessible official parts documentation we could retrieve.
- A commonly discussed third-party range appears to be roughly low-20s to high-20s psi, but this remains low-confidence unless tied to a primary Subaru/Tokyo Roki technical document or a repeatable independent lab test report.

### Local visual references saved in project

- `references/oil_filter_images/oem_filter_with_box_front.jpg`
- `references/oil_filter_images/oem_filter_with_box_alt.jpg`
- `references/oil_filter_images/oem_filter_angle_front.jpg`
- `references/oil_filter_images/oem_filter_rear_label.jpg`
- `references/oil_filter_images/oem_filter_cutaway_internal_media.jpg`

Image provenance and purpose:
- `oem_filter_with_box_front.jpg`
  - Purpose: confirms box label and can label together.
  - Source: https://www.flatironstuning.com/media/catalog/product/2/0/20230830_102300.jpg
- `oem_filter_with_box_alt.jpg`
  - Purpose: alternate high-resolution box + filter shot.
  - Source: https://www.flatironstuning.com/media/catalog/product/t/o/tokyo_roki.jpg
- `oem_filter_angle_front.jpg`
  - Purpose: angled view of can and base plate/thread form.
  - Source: https://stmtuned.com/cdn/shop/files/15208AA100-subaru-black-roki-engine-oil-filter-1_1024x1024.jpg?v=1738864979
- `oem_filter_rear_label.jpg`
  - Purpose: rear text/instructions side of can.
  - Source: https://stmtuned.com/cdn/shop/files/15208AA100-subaru-black-roki-engine-oil-filter-2_1024x1024.jpg?v=1738864979
- `oem_filter_cutaway_internal_media.jpg`
  - Purpose: internal media/cutaway reference for construction comparison.
  - Source: https://www.flatironstuning.com/media/catalog/product/2/0/20230830_102627.jpg

Note:
- No saved image in this set shows an explicit printed bypass pressure value (psi/bar) on the can or box.

## Independent tests and YouTube watchlist (bypass pressure)

The sources below are saved as a working list of independent testing/analysis leads focused on bypass pressure behavior.

| Source | Link | What it appears to contain | Confidence | Verification status |
|---|---|---|---|---|
| BITOG forum thread | https://bobistheoilguy.com/forums/threads/subaru-oem-filters-c-p-bypass-relief-pressure-measured.383381/ | Subaru OEM filter cut-open discussion with user-reported bypass opening measurement method and results | Medium | Partial: indexed snippets only in this workspace (direct fetch blocked/403) |
| YouTube (FlatironsTuning) | https://www.youtube.com/watch?v=MPfqucFejVw | Subaru oil filter relief valve spring comparison (Subaru-specific topic) | Medium | Metadata confirmed; full transcript/details not directly retrievable here |
| YouTube (The Motor Oil Geek) | https://www.youtube.com/watch?v=gSFNpW6kmxc | Cold-start bypass behavior test/analysis | Medium | Metadata confirmed; full transcript/details not directly retrievable here |
| YouTube (frozen filter test) | https://www.youtube.com/watch?v=inUzyT7a_Iw | Demonstration of bypass behavior under cold/high-viscosity conditions | Medium-Low for Subaru-specific relevance | Title/snippet confirmed; full details not directly retrievable here |
| YouTube (bigger filter testing claim) | https://www.youtube.com/watch?v=bff6rCVt7uo | Search snippet indicates Subaru-style filter about 23 psi vs Honda-style about 12 psi | Low-Medium until manually verified in-video | Snippet-level claim captured; requires manual confirmation in the video |

Notes:
- These are independent enthusiast sources, not official Subaru engineering publications.
- For decision-grade use, manually confirm each video's stated test method, exact pressure values, and whether values are measured or quoted from other sources.

## Reputable forum and video sources (OEM oil filter focus)

This is a tighter list of higher-signal community/video references specifically for Subaru OEM oil filter bypass behavior.

| Source type | Source | Why it is worth tracking | Reliability tier | Current verification status |
|---|---|---|---|---|
| Forum (technical, high signal) | https://bobistheoilguy.com/forums/threads/subaru-oem-filters-c-p-bypass-relief-pressure-measured.383381/ | Directly centered on measured bypass opening pressure for Subaru OEM filters; thread title and snippets indicate method/results discussion | Medium-High (community measured data, not OEM publication) | Snippet-level confirmation only (direct page fetch blocked in this workspace) |
| Forum (technical, historical context) | https://bobistheoilguy.com/forums/threads/subaru-and-27psi-bypass-filter-selection.323616/ | Long-running discussion of Subaru high-bypass filter assumptions and equivalent selection logic | Medium | Snippet-level confirmation only |
| Forum (vehicle-community OEM part context) | https://forums.nasioc.com/forums/showthread.php?t=1623020 | NASIOC thread about Subaru oil filter change announcement period; useful for timeline and part-transition context | Medium | Search-index title confirmed; direct thread fetch blocked |
| Forum (vehicle-community part lineage) | https://forums.nasioc.com/forums/showthread.php?t=1769829 | NASIOC thread focused on Tokyo Roki 15208AA100 part discussion | Medium | Search-index title confirmed; direct thread fetch blocked |
| Forum (owner community context) | https://www.subaruoutback.org/threads/made-in-japan-black-oil-filter.546895/ | Owner discussion on black Tokyo Roki filters and "correct bypass" claims; useful as secondary context only | Low-Medium | Snippet-level confirmation; content extraction unreliable |
| Video (Subaru-specific) | https://www.youtube.com/watch?v=MPfqucFejVw | Subaru-specific relief valve spring comparison topic; relevant to bypass behavior reasoning | Medium | Title/snippet confirmed through search index; direct YouTube fetch redirected to sign-in |
| Video (bypass behavior methodology) | https://www.youtube.com/watch?v=gSFNpW6kmxc | Focused on cold-start bypass activation claims and test logic, useful for method critique | Medium | Title/snippet confirmed through search index; direct YouTube fetch redirected to sign-in |
| Video (numeric claim to verify) | https://www.youtube.com/watch?v=bff6rCVt7uo | Search snippets mention Subaru-type filter around 23 psi vs Honda-type around 12 psi; candidate numeric claim source | Low-Medium until manually checked in-video | Snippet-level claim only |

### How to use these sources

- Treat all forum/video values as provisional unless method and instrumentation are visible and repeatable.
- Prefer posts/videos that show test rig details (pressure source, gauge calibration, fluid temperature, filter condition).
- Do not elevate any single forum or video claim above official Subaru/Tokyo Roki documentation.

## Collected data (with source quality)

### OEM Subaru 15208AA100
- Official Subaru page confirms part fitment/supersession and spring-loaded relief valve existence, but does not publish a numeric bypass setting or efficiency rating.
- Source: https://parts.subaru.com/p/Subaru_2009_STI/Oil-Filter-Complete/49227636/15208AA100.html
- Confidence: High for fitment; Low for numeric performance specs (not published there).

OEM supersession chain observed in Subaru ecosystem:
- 15208AA020
- 15208AA021
- 15208AA022
- 15208AA023
- 15208AA024
- 15208AA060
- 15208AA080
- 15208AA09A
- 15208AA12A
- SOA6351520812
- Current: 15208AA100

### WIX 57055
- Bypass Relief Valve Setting: 27 psi (RockAuto listing)
- Anti-Drain Back Valve: Yes
- Micron: 15 micron (nominal)
- Media: Enhanced cellulose
- Thread: M20x1.5
- Source 1: https://www.rockauto.com/en/moreinfo.php?pk=4768758
- Source 2: https://www.wixfilters.com/en-nz/catalog/results/product.html/57055_wix.html
  - WIX NZ page also lists bypass opening pressure = 1.9 bar (about 27.6 psi), matching RockAuto closely.
- Confidence: Medium-High (cross-confirmed across two catalog sources).

### FRAM XG7317 (Ultra Synthetic)
- Bypass Relief Valve Setting: 9-15 psi
- Anti-Drain Back Valve: Yes
- Media: Synthetic, dual-layer marketing claim
- Filtration claim: 99%+ filtration efficiency (RockAuto text)
- Thread: M20x1.5
- Source: https://www.rockauto.com/en/moreinfo.php?pk=261240
- Confidence: Medium (single structured source, but detailed).

## What this means for EJ257
For this turbo engine, bypass behavior matters because cold oil and high demand can increase pressure drop across the filter.

Key tradeoff from available data:
- FRAM XG7317 appears stronger on advertised filtration efficiency/media.
- WIX 57055 appears much closer to the high bypass-setting style commonly associated with Subaru applications.

Because Subaru does not publish a numeric bypass spec on the official `15208AA100` / `SOA6351520812` pages we could access, we cannot prove a precise OEM numeric target from official documentation alone in this research pass.

## Factor-by-factor check: WIX 57055 vs OEM 15208AA100

Assumption for this section: WIX bypass setting is sufficiently close to OEM behavior for practical comparison.

| Factor | WIX 57055 evidence | OEM 15208AA100 evidence | Relative result | Confidence |
|---|---|---|---|---|
| Bypass setting | 27 psi (RockAuto), 1.9 bar (WIX NZ) | No numeric value publicly listed on official Subaru pages | WIX has stronger published numeric transparency, but OEM target still unknown | Medium-High |
| Filtration efficiency | RockAuto/WIX marketing-level ISO statement for WIX line (commonly cited around 99% at 23 microns) | No OEM ISO efficiency curve published in accessible official sources | Cannot prove WIX better than OEM | Medium for WIX claim, Low for OEM comparison |
| Dirt-holding capacity | RockAuto lists 18 g (ISO statement in listing text) | No official OEM capacity number found | Cannot prove WIX better than OEM | Medium for WIX claim, Low for OEM comparison |
| Flow restriction vs flow rate | WIX listings provide general flow-related figures | No OEM pressure-drop or pressure-vs-flow curve found | No apples-to-apples comparison possible | Low-Medium |
| Burst/collapse strength | No strong primary manufacturer value located in this pass for 57055 | No official OEM burst/collapse value found | Not comparable with current evidence | Low |
| Construction quality (media/endcaps/louvers/valve consistency) | Mixed user cut-open commentary exists; not controlled test data | Mixed user cut-open commentary exists; not controlled test data | No objective winner from controlled data | Low |

### Practical conclusion from this factor check

- Even if bypass is close, current evidence still does not prove WIX 57055 is overall better than OEM 15208AA100.
- Best defensible position: WIX is a plausible alternative with better published aftermarket spec detail, while OEM remains the lower-risk baseline for exact Subaru calibration intent.
- To prove WIX is better, we still need side-by-side third-party lab data for both part numbers on efficiency curves, capacity, pressure-drop vs flow, and burst/collapse.

## Determination: Is there a clearly better filter than OEM?
No clear universal winner from objective public data collected here.

- If your top priority is filtration efficiency marketing claim, FRAM XG7317 looks stronger.
- If your top priority is high bypass-setting behavior that is likely closer to Subaru-style calibration, WIX 57055 looks closer.
- If your top priority is lowest risk for OEM calibration and warranty-fit behavior, OEM 15208AA100 remains the safest default.

## Practical recommendation
For a 2009 STI used hard or in cold starts:
- Keep OEM 15208AA100 as default.
- Consider WIX 57055 as the closest documented high-bypass alternative from this dataset.
- Use FRAM XG7317 only if you intentionally prioritize its filtration claim and accept its lower listed bypass range.

## Remaining data gap
Still needed to make a stronger call:
- official numeric bypass setting and ISO efficiency data for OEM `15208AA100` from Subaru/Tokyo Roki technical documentation (or a clearly attributable engineering datasheet).
