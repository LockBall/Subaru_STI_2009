# Oil Filter — 2009 WRX STI (EJ257)

Last reviewed: 2026-07-16. This is the canonical oil-filter document.

## Recommendation

Use **Subaru `15208AA100`** when the goal is the lowest-risk choice. Subaru confirms fitment and the supersession chain, but does not publish its bypass-valve setting or filtration efficiency.

**WIX `57055`** is the best-documented non-OEM candidate in the current research. Its published 27 psi / 1.9 bar bypass setting is useful information, but it cannot be proven to match Subaru because Subaru does not publish the OEM value.

Do not select an oil filter by thread and gasket size alone. Bypass-valve behavior matters on a turbocharged engine, particularly with cold oil.

## OE part and supersession

| Part | Status | Source |
|---|---|---|
| Subaru `15208AA100` | Current OE reference in this tracker | [2009 STI Subaru catalog](https://parts.subaru.com/p/Subaru_2009_STI/Oil-Filter-Complete/49227636/15208AA100.html) |
| `15208AA020`, `021`, `022`, `023`, `024`, `060`, `080`, `09A`, `12A`, `SOA6351520812` | Prior / alternate numbers recorded in Subaru sources | Subaru catalog family |

## What is known

| Filter | Bypass setting | Other published data | Evidence limit |
|---|---:|---|---|
| Subaru `15208AA100` | Not published | Subaru describes a spring-loaded relief valve | No public numeric bypass or efficiency specification found |
| WIX `57055` | 27 psi; WIX also lists 1.9 bar | Anti-drainback valve; M20 × 1.5 thread; enhanced-cellulose media | Aftermarket specification, not proof of an OEM match |
| FRAM XG7317 | 9–15 psi | Synthetic-media and 99%+ filtration claims | Single structured catalog source in this research; lower bypass than WIX |

Sources: [WIX 57055](https://www.wixfilters.com/en-nz/catalog/results/product.html/57055_wix.html), [RockAuto WIX listing](https://www.rockauto.com/en/moreinfo.php?pk=4768758), [RockAuto FRAM listing](https://www.rockauto.com/en/moreinfo.php?pk=261240).

## Decision rule

- Choose **Subaru** for known OE fit and calibration intent.
- Choose **WIX 57055** only if you accept that its documented bypass setting is an informed proxy, not a verified OEM match.
- Do not choose **FRAM XG7317** solely for its filtration claim when bypass behavior is the priority.

## Community and video evidence

Forums and videos can add useful evidence if the exact filter, test setup, temperature, gauge, and measured opening point are shown. Current leads include [BITOG’s measured-bypass discussion](https://bobistheoilguy.com/forums/threads/subaru-oem-filters-c-p-bypass-relief-pressure-measured.383381/) and [Flatirons Tuning’s Subaru filter video](https://www.youtube.com/watch?v=MPfqucFejVw). Treat their numbers as provisional until the full method is checked; they do not override Subaru’s fitment information.

## Local image references

Photos and provenance are in [references/oil_filter_images](references/oil_filter_images/README.md). They confirm labels and construction details, not a bypass-pressure value.
