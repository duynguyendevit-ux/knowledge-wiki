---
title: Firework Mortar Tube Dimensions Reference
tags: [fireworks, game-design, 3d-modeling, technical-reference]
date: 2026-06-07
---

# Firework Mortar Tube Dimensions Reference

## Executive Summary

**Key principle:** Individual tube dimensions are driven by **shell caliber**, not by rack shot count. A 5-shot, 10-shot, or 50-shot rack can all use the same 12-inch DR11 tube; what changes is the number of tubes and layout (straight, V-fan, or W-fan).

For game scale, the strongest visual anchors are the **tube heights**:
- Consumer 1.75" shells: **30.5-38.1 cm** tall
- Professional display tubes scale up fast
- Dense racks look realistic up to ~6 inches
- 8"+ shells are better as single tubes or sparse groups

## Shell Size Classes

Standard sizes include: **1.75, 2, 2.5, 3, 4, 5, 6, 7, 8, 10, 12, 16 inches**

NFPA baseline rule: **shell size = inside diameter of the mortar**

## Material Families

### HDPE (High-Density Polyethylene)
- Dominates U.S. reusable consumer and display tubes
- Visual: Black or orange, thicker walls
- Common in 12"/15" consumer formats

### Fiberglass / FRE (Fire-Resistant Epoxy)
- Dominates European professional tubes
- Visual: Yellow or natural color, slimmer small-caliber tubes
- Reinforced ends on 7-10" professional mortars

### Cardboard
- Still appears in reloadable consumer kits
- Single-use, disposable

### Steel
- Present in professional contexts
- Less common in current catalogs vs HDPE/fiberglass

## Tube Dimension Reference Table

| Shell Class | Tube ID | Tube OD | Tube Length | Wall | Typical Usage |
|-------------|---------|---------|-------------|------|---------------|
| **1.75" consumer** (DR11) | ~4.9 cm | ~5.8-6.1 cm | **30.5-38.1 cm** | thin-medium | Dense consumer straight/fan racks |
| **2" display** | ~5.1 cm | ~5.5-6.1 cm | **30.5-35 cm** | thin-medium | Single tube, compact display rack |
| **2.5" display** | ~6.4 cm | ~6.9 cm | **42-45.7 cm** | thin | Small pro rack, short bar rack |
| **3" display** | ~7.6 cm | ~8.2-8.9 cm | **45-50.8 cm** | thin-medium | 6-8 tube bars, wood crates |
| **4" display** | ~10.1-10.2 cm | ~10.7-11.4 cm | **55-65 cm** | medium | 6-tube bar racks, medium crates |
| **5" display** | ~12.7 cm | ~13.2-14.0 cm | **71-80 cm** | medium | 5-10 tube wood racks |
| **6" display** | ~15.1-15.4 cm | ~15.8-16.5 cm | **84-90 cm** | medium-heavy | Steel bars, heavy wood crates |
| **7" display** | ~17.7-17.8 cm | ~18.1-18.7 cm | **~100 cm** | medium | Sparse groups, large singles |
| **8" display** | ~20.3-20.8 cm | ~21.3-22.4 cm | **110-122 cm** | heavy | Single tubes, very sparse groups |
| **10" display** | ~25.4-25.6 cm | ~26.0-27.6 cm | **120-121.3 cm** | heavy | Isolated heavy singles |
| **12" display** | ~30.6 cm | ~33.0 cm | **~130 cm** | very heavy | Single heavy tube only |
| **16" display** | - | - | **~161.9 cm** | very heavy | Specialist show scale only |

## Rack Archetypes

### Consumer Straight Rack
- **6-shot:** ~45-50 L × 10-15 W × 35-40 H cm
- **12-shot:** ~90 L × 10-15 W × 35-40 H cm
- Visual: Dense, one-row, black/orange HDPE

### Consumer V-Fan Rack
- **24-shot V:** ~90 L × 25-35 W × 35-40 H cm
- Two rows of 12 tubes
- Outer rows angled **15° off center** (real product spec)

### Consumer W-Fan Rack
- **24-shot W:** ~90 L × 35-45 W × 35-40 H cm
- **36-shot W:** ~90 L × 45-55 W × 35-40 H cm
- Three rows: center straight, outer rows angled

### Metal Display Bar Rack
- 3" for 8 tubes; 4" for 6; 6" for 4
- Bar length: ~74-76 cm before side legs
- Visual: Industrial, heavier than wood consumer racks

### Wood/Plywood Crate Rack
- Common pro-display look (3"-6")
- Boxed sides, braces, diagonal bracing
- Visual: "Crate" silhouette with mass

### Modular Sleeve Rack
- 6-shot ARC component: **44.5 cm long × ~7.6 cm wide**
- Tube pitch: ~7.4 cm per tube lane
- Good for kit-bash systems

## NFPA Rack Safety Rules

- **≤6" shells:** May be rack-fired
- **7-8" shells:** Require extra restrictions in racks
- **>8" shells:** Move away from dense rack use
- **Chain-fused racks capped at:**
  - 15 tubes for 3" and under
  - 12 tubes for 4"
  - 10 tubes for 5-6"
  - No racks above 6" in that category

**Game implication:** Dense racks look realistic up to ~6". Use singles/sparse groups for 8"+.

## Spectator Safety Distances (NFPA)

| Shell Size | Minimum Distance |
|------------|------------------|
| 2" | ~43 m |
| 3" | ~64 m |
| 4" | ~85 m |
| 5" | ~107 m |
| 6" | ~128 m |
| 8" | ~171 m |
| 10" | ~213 m |

**Game scale tip:** If spectators are only a few meters from mortars, it reads as stylized, not realistic.

## Regional Style Split

### U.S.-Leaning Scenes
- Black or orange HDPE
- Thicker walls
- 12"/15" consumer formats common

### EU-Leaning Scenes
- Yellow or natural fiberglass/FRE
- Slimmer small-caliber tubes
- Reinforced 7-10" professional mortars

## Game Art Workflow

```
1. Choose show style (consumer DR11 or professional display)
2. Choose caliber ladder (1.75", 3-6", 7-10"+)
3. Set tube height and OD from reference table
4. Choose rack family (single, straight, fan, bar, crate)
5. Block out environment scale
6. Place shells, fuses, wires, braces, drums/legs
7. Texture by material family
8. Finalize gameplay collision and staging
```

## Recommended Game Mix

For neutral, contemporary baseline that reads correctly:

- **Small setups:** 1.75" consumer shells in 1.91" HDPE fan racks
- **Pro-middle scale:** 3-6" black HDPE or fiberglass tubes in wood/metal racks
- **Large-show moments:** 7-10" yellow fiberglass/FRE singles or sparse heavy groups

## Technical Notes

- **Consumer 6-shot ARC sleeve:** 17.5" (44.5 cm) long holding 6 tubes = ~7.4 cm pitch per tube
- **V-fan angle:** 15° off center (PyroBoom product spec)
- **Tube spacing:** Minimal clearance between shell OD and mortar ID (NFPA guidance)
- **Large-caliber staging:** Use buried tubes in sand or sand-filled drums (NRCan method)

## Sources

Primary sources include:
- NFPA 1123 (Display Fireworks standards)
- Natural Resources Canada Display Fireworks Manual
- NICO Europe, Pyroservice UG, Pyro Direct, American Wholesale Fireworks catalogs
- Fire-code and inspection documents

---

**Related:** [[index|Fireworks Index]] | [[mortar-tube-dimensions-vi|Bản tiếng Việt]]
