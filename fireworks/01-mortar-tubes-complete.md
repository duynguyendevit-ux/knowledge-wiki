---
title: Fireworks Mortar Tubes - Complete Technical Reference
tags: [fireworks, engineering, physics, materials, tubes]
date: 2026-06-08
---

# Fireworks Mortar Tubes - Complete Technical Reference

Comprehensive guide to fireworks mortar tube engineering, physics, materials, and specifications.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Physics & Engineering](#physics-engineering)
3. [Material Science](#material-science)
4. [Tube Specifications by Caliber](#specifications)
5. [Ballistics & Trajectory](#ballistics)
6. [Regional Standards](#standards)
7. [Inspection & Maintenance](#maintenance)
8. [Game Development Guidelines](#game-dev)

---

## Introduction {#introduction}

A fireworks mortar tube is a launch cylinder designed to safely contain and direct the explosive thrust of a fireworks shell. The tube must withstand internal pressures from 100-200+ PSI while maintaining structural integrity through repeated firings.

**Key Principle:** Tube dimensions are determined by shell caliber and required pressure rating, not by rack configuration.

**Shell Size Classes:**
Standard sizes include: **1.75, 2, 2.5, 3, 4, 5, 6, 7, 8, 10, 12, 16 inches**

**NFPA baseline rule:** Shell size = inside diameter of the mortar

---

## Physics & Engineering {#physics-engineering}

### Pressure Dynamics

**Internal Pressure Generation:**
- Lift charge burns rapidly (black powder: ~400 m/s burn rate)
- Gas expansion creates 100-200 PSI depending on lift charge mass
- Peak pressure occurs in first 10-50ms
- Tube must contain pressure until shell clears muzzle

**Material Strength Requirements:**
```
Hoop Stress (σ) = (P × r) / t

Where:
P = internal pressure (PSI)
r = tube inner radius (inches)
t = wall thickness (inches)

Safety Factor = Material Yield Strength / Hoop Stress
Target Safety Factor: 3-5x for reusable tubes
```

**Engineering Trade-off:**
- Thicker walls (lower DR) = heavier, more expensive, higher pressure rating
- Thinner walls (higher DR) = lighter, cheaper, adequate for controlled lift charges

### Dimension Ratio (DR) System

**DR = Outside Diameter ÷ Wall Thickness**

Higher DR = thinner walls = lower pressure rating

**Common Ratings:**

#### DR11 - Consumer Grade
- **Pressure rating:** 200 PSI class
- **Example:** 2.4" OD ÷ 11 = 0.218" theoretical wall
- **Actual:** ~0.245" (manufacturing variance)
- **Use:** 1.75" consumer shells (60-100g lift powder)

#### DR17 - Light Professional
- **Pressure rating:** 125 PSI class
- **Example:** 3.5" OD ÷ 17 = 0.206" wall
- **Use:** 3" display shells (150-250g lift powder)

#### DR21 - Heavy Professional
- **Pressure rating:** 100 PSI class
- **Example:** 4.5" OD ÷ 21 = 0.214" wall
- **Use:** 4", 5", 6" display shells (250-900g lift powder)

---

## Material Science {#material-science}

### HDPE (High-Density Polyethylene)

**Properties:**
- **Density:** 0.93-0.97 g/cm³
- **Tensile strength:** 26-33 MPa
- **Melting point:** 120-180°C
- **Impact resistance:** Excellent (especially at low temperatures)
- **Chemical resistance:** Excellent (acids, bases, solvents)

**Advantages:**
- Reusable (100+ firings with proper care)
- Impact-resistant (survives drops, transport)
- Weather-resistant (UV-stabilized grades)
- Lightweight
- Cost-effective for mass production

**Color Coding:**
- **Black:** UV-stabilized, most common consumer
- **Orange:** High-visibility variant
- **Natural/white:** Professional display tubes

**Thermal Behavior:**
- Softens at ~80°C
- Melts at ~130°C
- Residual heat from repeated firings can degrade material
- **Recommended cool-down:** 2-5 minutes between shots

**Visual Characteristics for Games:**
- **Finish:** Matte, slightly rough texture
- **Reflectivity:** Low (10-20%)
- **Weathering:** Scuff marks, dirt accumulation
- **Does NOT rust** (common mistake in games)

### Fiberglass / FRE (Fire-Resistant Epoxy)

**Properties:**
- **Density:** 1.4-1.9 g/cm³
- **Tensile strength:** 70-200 MPa (depending on fiber weave)
- **Heat resistance:** 150-300°C
- **Stiffness:** Higher than HDPE
- **Impact resistance:** Moderate (can crack if dropped)

**Advantages:**
- Higher temperature tolerance
- Thinner walls possible (higher strength-to-weight)
- Professional-grade aesthetics
- Better dimensional stability under heat

**Construction:**
- Fiberglass cloth + epoxy resin
- Wrapped in layers (3-8 plies typical)
- Reinforced ends with extra plies
- May include aramid fiber (Kevlar) in high-stress areas

**Color Coding:**
- **Yellow:** Standard European professional
- **Natural/tan:** Bare resin finish
- **Black:** Rare, carbon fiber composite

**Visual Characteristics for Games:**
- **Finish:** Smooth, glossy (resin surface)
- **Reflectivity:** Medium (30-40%)
- **Weathering:** Edge chipping, resin cracks, delamination
- **Professional appearance**

### Cardboard

**Properties:**
- **Single-use only**
- **Wall thickness:** 2-5mm (multi-ply spiral wound)
- **Cheap, disposable**
- **Burns after firing** (intentional safety feature)

**Modern Use:**
- Reloadable consumer kits
- Low-cost festivals
- Single-event displays

**Visual:** Brown kraft paper, spiral winding visible, lightweight appearance

### Steel

**Properties:**
- Extremely durable
- High pressure rating
- Heavy (difficult to transport)
- Rust concerns
- Expensive

**Modern Use:**
- Rare in contemporary catalogs
- Legacy installations
- Fixed heavy-mortar positions

---

## Tube Specifications by Caliber {#specifications}

### Complete Specification Table

| Shell Size | Inner Diameter | Outer Diameter | Wall Thickness | Length | DR Rating | Material | Typical Lift Powder |
|------------|---------------|----------------|----------------|--------|-----------|----------|---------------------|
| **1.75"** (consumer) | 1.91" (4.85 cm) | 2.4" (6.1 cm) | ~0.245" (0.62 cm) | 12"-15" (30.5-38.1 cm) | DR11 | HDPE | 60-100g |
| **2"** (display) | 2.0" (5.1 cm) | 2.4" (6.1 cm) | ~0.2" (0.5 cm) | 12"-14" (30.5-35 cm) | DR11 | HDPE | 80-120g |
| **2.5"** (display) | 2.5" (6.4 cm) | 2.75" (6.9 cm) | ~0.13" (0.3 cm) | 16"-18" (42-45.7 cm) | Thin | HDPE | 120-180g |
| **3"** (display) | 3.0" (7.6 cm) | 3.5" (8.9 cm) | ~0.25" (0.64 cm) | 18"-20" (45.7-50.8 cm) | DR17 | HDPE | 150-250g |
| **4"** (display) | 4.0" (10.2 cm) | 4.5" (11.4 cm) | ~0.25" (0.64 cm) | 24" (61 cm) | DR21 | HDPE | 250-400g |
| **5"** (display) | 5.0" (12.7 cm) | 5.5" (14.0 cm) | ~0.26" (0.66 cm) | 28" (71.1 cm) | DR21 | HDPE | 400-650g |
| **6"** (display) | 6.0" (15.2 cm) | 6.5" (16.5 cm) | ~0.31" (0.79 cm) | 33" (83.8 cm) | DR21 | HDPE | 650-900g |
| **7"** (display) | 7.0" (17.8 cm) | 7.5" (19.0 cm) | ~0.25" (0.64 cm) | 39" (99 cm) | Medium | Fiberglass | 900-1200g |
| **8"** (display) | 8.0" (20.3 cm) | 8.75" (22.2 cm) | ~0.38" (0.97 cm) | 44" (112 cm) | Heavy | Fiberglass | 1-1.5kg |
| **10"** (display) | 10.0" (25.4 cm) | 10.75" (27.3 cm) | ~0.38" (0.97 cm) | 48" (122 cm) | Heavy | Fiberglass | 1.5-2.5kg |
| **12"** (display) | 12.0" (30.5 cm) | 13.0" (33.0 cm) | ~0.5" (1.27 cm) | 51" (130 cm) | Extra Heavy | Steel/FRE | 2.5-4kg |
| **16"** (display) | 16.0" (40.6 cm) | 17.0" (43.2 cm) | ~0.5" (1.27 cm) | 64" (162 cm) | Extra Heavy | Steel/FRE | 4-6kg |

### Length-to-Diameter Ratios

**Consumer shells (1.75"-2.5"):**
- 12" tube = **6.3:1** length:ID ratio
- 15" tube = **7.9:1** length:ID ratio
- Longer tubes provide more consistent aim but are harder to rack

**Professional shells (3"-6"):**
- Typical ratio: **6:1 to 5.5:1**

**Large shells (8"-10"):**
- Typical ratio: **5.5:1 to 4.8:1**

**Extra-large shells (12"+):**
- Typical ratio: **4.25:1**

**Why shorter ratios for larger shells:**
1. Weight constraints (longer tubes = much heavier)
2. Trajectory control (larger shells are more stable in flight)
3. Structural limits (excessive length causes tube flex)

### Weight Reference

**Consumer Equipment:**
- Empty 6-shot rack: ~4 lbs (1.8 kg)
- 6× DR11 12" tubes: ~12 lbs (5.4 kg)
- **Total 6-shot system:** ~16 lbs (7.3 kg)

**Display Equipment:**
- 3" HDPE tube (20"): ~2-3 lbs each
- 4" HDPE tube (24"): ~3-4 lbs each
- 5" HDPE tube (28"): ~4-5 lbs each
- 6" HDPE tube (33"): ~5-7 lbs each

---

## Ballistics & Trajectory {#ballistics}

### Launch Velocity

**Typical muzzle velocities:**
- Consumer 1.75": **30-40 m/s**
- 3" display: **40-50 m/s**
- 6" display: **50-65 m/s**
- 10" display: **60-80 m/s**

**Velocity Formula (simplified):**
```
v = √(2 × P × V / m)

Where:
P = average pressure during acceleration
V = tube volume
m = shell mass
```

Higher pressure or longer tube → higher velocity → higher apex

### Apex Height

**Theoretical apex (ignoring air resistance):**
```
h = v² / (2 × g)

Where:
v = muzzle velocity
g = 9.81 m/s² (gravity)
```

**Practical apex heights:**
- **1.75" consumer:** 30-60m
- **3" display:** 60-100m
- **6" display:** 100-150m
- **10" display:** 150-250m
- **12" display:** 200-300m

### Trajectory Angle

**Standard angles:**
- **90° (vertical):** Maximum height, centered break
- **75-80°:** Common for slight wind compensation
- **60-70°:** Fan effects, crossfire patterns
- **45° (theoretical maximum range):** Rarely used (safety concerns)

**Angle deviation tolerance:**
- **±5°:** Acceptable for consumer displays
- **±2°:** Professional standard
- **±1°:** Competition/synchronized shows

Tubes are typically embedded in sand, foam, or mechanical mounts to maintain angle.

---

## Regional Standards & Regulations {#standards}

### United States (NFPA 1123)

**Regulatory Bodies:**
- **NFPA 1123:** Display fireworks standard
- **DOT:** Transport classification
- **CPSC:** Consumer product safety
- **ATF:** Storage and licensing

**Key Requirements:**
- Minimum wall thickness based on shell size
- Pressure testing for reusable tubes
- Inspection after accidents
- Retirement criteria (cracks, deformation, burns)

### European Union (EN 15947-5)

**Standards:**
- **EN 15947-5:** Fireworks display equipment
- **CE marking:** Required for commercial tubes

**Differences from US:**
- More common use of fiberglass over HDPE
- Stricter reinforcement requirements for 7"+ shells
- Yellow color standard for professional visibility

### Asia - China (GB 10631)

**Standards:**
- **GB 10631:** Safety standards for fireworks
- Manufacturing focus on cardboard (disposable)
- Steel tubes for large shells (10"+)

---

## Inspection & Maintenance {#maintenance}

### Pre-Fire Inspection

**Visual checks:**
- Cracks in tube body
- Deformation (bulges, dents)
- Muzzle damage (chips, cracks)
- Bottom plug integrity
- Discoloration from heat damage

**Rejection criteria:**
- Any visible crack
- Bulge > 5% of nominal diameter
- Muzzle damage > 10mm
- Heat discoloration > 30% of surface

### Maintenance Procedures

**HDPE tubes:**
1. Clean with soap and water after use
2. Inspect for cracks while wet (easier to see)
3. Store indoors (avoid UV exposure)
4. Do not stack more than 5 high (prevent deformation)

**Fiberglass tubes:**
1. Inspect for delamination (layers separating)
2. Check reinforced ends for resin cracking
3. Avoid impacts when cold (more brittle)
4. Sand down rough edges (prevent shell hang-ups)

### Service Life & Retirement

**Typical service life:**
- **HDPE consumer:** 50-100 firings
- **HDPE professional:** 100-200 firings
- **Fiberglass:** 200-500 firings
- **Steel:** 1000+ firings (if maintained)

**Retirement triggers:**
- Visible damage
- Excessive heat exposure (melting, charring)
- Manufacturer recommendation
- Regulatory inspection failure

---

## Game Development Guidelines {#game-dev}

### Visual Scale Reference

**Tube height is the strongest visual anchor:**
- **1.75" consumer:** 30-40 cm tall (baseline scale)
- **3" display:** 45-50 cm tall
- **6" display:** 80-90 cm tall
- **10" display:** 120 cm tall

**Use tube height to establish scene scale** - it's the most recognizable visual element.

### Proportions for Modeling

**General rules:**
- OD ≈ ID + 0.5-1.0" (smaller shells)
- OD ≈ ID + 0.75-1.5" (larger shells)
- Length ≈ 6× ID (consumer)
- Length ≈ 5× ID (professional)

### Material Representation

**HDPE (consumer/common):**
- **Albedo:** Matte black (#1A1A1A) or safety orange (#FF6600)
- **Roughness:** 0.7-0.9 (rough surface)
- **Metallic:** 0.0 (non-metallic)
- **Specular:** Low (10-20%)
- **Weathering:** Scuff marks, dirt accumulation, scratches
- **Does NOT rust** (common error)

**Fiberglass (professional):**
- **Albedo:** Bright yellow (#FFD700) or natural tan (#D2B48C)
- **Roughness:** 0.3-0.5 (smooth resin surface)
- **Metallic:** 0.0
- **Specular:** Medium (30-40%)
- **Weathering:** Edge chipping, resin cracks, delamination at seams
- **Glossy appearance**

### Physical Detail Levels

**LOD0 (Hero/Close-up):**
- Model bottom plugs (HDPE: molded; fiberglass: separate cap)
- Include fuse holes near bottom
- Show wall thickness at muzzle
- Add mounting hardware (stakes, brackets)
- Include manufacturer markings/labels

**LOD1 (Medium Distance):**
- Simplified plugs
- Basic fuse holes
- Combined geometry
- Simplified hardware

**LOD2 (Far Distance):**
- Cylinder proxy
- Single material
- No detail features

### Collision Meshes

- **Consumer tube:** Cylinder 6cm diameter × 35cm height
- **3" display:** Cylinder 9cm diameter × 50cm height
- **6" display:** Cylinder 17cm diameter × 85cm height

### Texture Resolution

- **Consumer rack albedo:** 2K sufficient
- **Display rack albedo:** 2K-4K for hero shots
- **Normal maps:** Focus on tube openings, plug seams, and surface scratches
- **Roughness maps:** Weathering variation

### Common Mistakes to Avoid

❌ **Wrong:** Tubes too small (toy-like appearance)  
✅ **Right:** Use height reference (30-120cm based on caliber)

❌ **Wrong:** Shiny plastic material (looks wet)  
✅ **Right:** Matte HDPE or glossy fiberglass (match material family)

❌ **Wrong:** Rusty consumer tubes  
✅ **Right:** HDPE doesn't rust, only scuffs and dirt

❌ **Wrong:** Uniform pristine appearance  
✅ **Right:** Add weathering (consumer: dirt/scuffs; professional: chips/cracks)

---

## Quick Reference

### Tube Dimensions Summary

| Shell | Height | Diameter | Weight | Apex | Material |
|-------|--------|----------|--------|------|----------|
| 1.75" | 30-38cm | 6.1cm | Light | 30-60m | HDPE black |
| 3" | 45-51cm | 8.9cm | Medium | 60-100m | HDPE black |
| 6" | 84cm | 16.5cm | Heavy | 100-150m | HDPE/Fiberglass |
| 10" | 122cm | 27.3cm | Very Heavy | 150-250m | Fiberglass yellow |

### Material Quick Comparison

| Property | HDPE | Fiberglass |
|----------|------|------------|
| Color | Black/Orange | Yellow/Tan |
| Finish | Matte | Glossy |
| Weight | Light | Medium |
| Use | Consumer/Pro | Professional |
| Reusability | 100-200 | 200-500 |
| Cost | Low | Medium |

---

## Sources & References

**Technical Standards:**
- NFPA 1123: Code for Fireworks Display (2020 Edition)
- EN 15947-5: Pyrotechnic articles - Part 5: Display fireworks
- GB 10631: Safety standards for fireworks (China)

**Material Data:**
- HDPE: ASTM D4976 (polyethylene pressure pipe)
- Fiberglass: ASTM D3039 (tensile testing)

**Manufacturer Specifications:**
- American Wholesale Fireworks
- Pyro Supply, PyroDirect
- Great Lakes Mortar Racks
- Pro Pyro Racks, PyroBoom

**Field References:**
- Natural Resources Canada: Display Fireworks Manual
- California Fire Marshal: Fireworks Guidelines
- UK HSE: Storing and Using Fireworks

---

**Last Updated:** 2026-06-08  
**Related:** [[02-rack-systems-complete|Rack Systems]] | [[03-effects-types-complete|Effects Types]] | [[04-chemistry-colors-complete|Chemistry & Colors]]
