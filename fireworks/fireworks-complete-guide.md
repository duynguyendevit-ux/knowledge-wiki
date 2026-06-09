---
title: Fireworks Complete Technical Guide
tags: [fireworks, game-design, 3d-modeling, technical-reference, complete-guide]
date: 2026-06-08
---

# Fireworks Complete Technical Guide

Comprehensive technical documentation for fireworks modeling in games and 3D applications. Combines physics, engineering, chemistry, and visual effects reference.

---

## Table of Contents

1. [Mortar Tubes - Physics & Engineering](#mortar-tubes)
2. [Rack Systems - Configuration & Safety](#rack-systems)
3. [Effects Types - Visual Reference](#effects-types)
4. [Chemistry & Colors](#chemistry-colors)
5. [Game Development Guidelines](#game-development)
6. [Quick Reference Tables](#quick-reference)

---

## Mortar Tubes - Physics & Engineering {#mortar-tubes}

### Introduction

A fireworks mortar tube is a launch cylinder designed to safely contain and direct the explosive thrust of a fireworks shell. The tube must withstand internal pressures from 100-200+ PSI while maintaining structural integrity through repeated firings.

**Key Principle:** Tube dimensions are determined by shell caliber and required pressure rating, not by rack configuration.

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

### Dimension Ratio (DR) System

**DR = Outside Diameter ÷ Wall Thickness**

Higher DR = thinner walls = lower pressure rating

**Common Ratings:**
- **DR11:** 200 PSI class (consumer grade)
  - Example: 2.4" OD ÷ 11 = 0.218" theoretical wall
  - Actual: ~0.245" (manufacturing variance)
  
- **DR17:** 125 PSI class (light professional)
  - Example: 3.5" OD ÷ 17 = 0.206" wall
  - Used for: 3" display shells
  
- **DR21:** 100 PSI class (heavy professional)
  - Example: 4.5" OD ÷ 21 = 0.214" wall
  - Used for: 4", 5", 6" display shells

### Material Science

#### HDPE (High-Density Polyethylene)

**Properties:**
- Density: 0.93-0.97 g/cm³
- Tensile strength: 26-33 MPa
- Melting point: 120-180°C
- Impact resistance: Excellent
- Chemical resistance: Excellent

**Advantages:**
- Reusable (100+ firings)
- Impact-resistant
- Weather-resistant
- Lightweight
- Cost-effective

**Color Coding:**
- Black: UV-stabilized, most common
- Orange: High-visibility variant
- Natural/white: Professional display

#### Fiberglass / FRE

**Properties:**
- Density: 1.4-1.9 g/cm³
- Tensile strength: 70-200 MPa
- Heat resistance: 150-300°C
- Higher stiffness than HDPE

**Advantages:**
- Higher temperature tolerance
- Thinner walls possible
- Professional-grade aesthetics
- Better dimensional stability

**Construction:**
- Fiberglass cloth + epoxy resin
- 3-8 plies typical
- Reinforced ends
- May include Kevlar in high-stress areas

**Color:**
- Yellow: Standard European professional
- Natural/tan: Bare resin finish
- Black: Carbon fiber composite (rare)

### Tube Specifications by Caliber

| Shell Size | Inner Diameter | Outer Diameter | Wall Thickness | Length | DR Rating | Material | Lift Powder |
|---|---|---|---|---|---|---|---|
| **1.75"** | 1.91" (4.9cm) | 2.4" (6.1cm) | ~0.245" (0.6cm) | 12"-15" (30-38cm) | DR11 | HDPE | 60-100g |
| **3"** | 3.0" (7.6cm) | 3.5" (8.9cm) | ~0.25" (0.6cm) | 18"-20" (45-51cm) | DR17 | HDPE | 150-250g |
| **4"** | 4.0" (10.2cm) | 4.5" (11.4cm) | ~0.25" (0.6cm) | 24" (61cm) | DR21 | HDPE | 250-400g |
| **5"** | 5.0" (12.7cm) | 5.5" (14.0cm) | ~0.26" (0.7cm) | 28" (71cm) | DR21 | HDPE | 400-650g |
| **6"** | 6.0" (15.2cm) | 6.5" (16.5cm) | ~0.31" (0.8cm) | 33" (84cm) | DR21 | HDPE | 650-900g |
| **8"** | 8.0" (20.3cm) | 8.75" (22.2cm) | ~0.38" (1.0cm) | 44" (112cm) | Heavy | Fiberglass | 1-1.5kg |
| **10"** | 10.0" (25.4cm) | 10.75" (27.3cm) | ~0.38" (1.0cm) | 48" (122cm) | Heavy | Fiberglass | 1.5-2.5kg |
| **12"** | 12.0" (30.5cm) | 13.0" (33.0cm) | ~0.5" (1.3cm) | 51" (130cm) | Extra Heavy | Steel/FRE | 2.5-4kg |

### Ballistics & Trajectory

**Typical muzzle velocities:**
- Consumer 1.75": 30-40 m/s
- 3" display: 40-50 m/s
- 6" display: 50-65 m/s
- 10" display: 60-80 m/s

**Practical apex heights:**
- 1.75" consumer: 30-60m
- 3" display: 60-100m
- 6" display: 100-150m
- 10" display: 150-250m
- 12" display: 200-300m

**Standard angles:**
- 90° (vertical): Maximum height, centered break
- 75-80°: Common for wind compensation
- 60-70°: Fan effects, crossfire patterns

---

## Rack Systems - Configuration & Safety {#rack-systems}

### Introduction

A fireworks rack is a structural assembly that holds multiple mortar tubes in a fixed geometric configuration. Racks serve three primary functions:

1. **Safety:** Maintain correct tube angles and spacing
2. **Efficiency:** Enable rapid sequential or simultaneous firing
3. **Choreography:** Create geometric break patterns

### Rack Classification

#### By Tube Count
- **Small:** 1-6 tubes (testing, accents)
- **Medium:** 8-24 tubes (standard consumer/pro)
- **Large:** 25-50 tubes (finale racks)
- **Array:** 50+ tubes (synchronized displays)

#### By Pattern Type
- **Straight/Linear:** Single row, uniform spacing
- **V-Fan:** Two angled rows diverging from center
- **W-Fan:** Three rows (center straight, sides angled)
- **Circular:** Tubes arranged in ring pattern
- **Custom:** Irregular patterns for specific effects

#### By Construction
- **Consumer Modular:** Plastic injection-molded (HDPE)
- **Professional Bar:** Steel/aluminum rail systems
- **Wood Crate:** Plywood box frames
- **Ground-Set:** Individual buried tubes
- **Elevated:** Mounted on towers/platforms

### Engineering Principles

#### Spacing Requirements

**NFPA 1123 Minimum Tube Separation:**
- **2" shells:** No minimum specified (practical: 2-3")
- **3" shells:** 2" clear space between tubes
- **4" shells:** 2" clear space
- **5-6" shells:** 3" clear space
- **8" shells:** 4" clear space

**Practical Spacing (Consumer Racks):**
- Tube OD: 2.4" (6.1cm)
- Clear space: 0.5-1.0" (1.3-2.5cm)
- Center-to-center pitch: 3.0-3.5" (7.6-8.9cm)

#### Fan Angle Calculations

**V-Fan Configuration:**
- Standard divergence: **15° per side** from center axis
- Total spread angle: 30°

**W-Fan Configuration:**
- Center row: 0° (vertical)
- Outer rows: 15° divergence
- Creates three distinct break zones

### Standard Rack Configurations

#### Consumer Straight Racks

**6-Shot Straight:**
- Dimensions: 18" L × 13" W × 5" H (46 × 33 × 13 cm)
- Tube size: 1.91" ID × 12" length
- Tube spacing: 3" (7.6cm) center-to-center
- Weight (loaded): 5.5-6.5kg
- Pattern: Single horizontal line

**12-Shot Straight:**
- Dimensions: 36" L × 13" W × 5" H (91 × 33 × 13 cm)
- Tube size: 1.91" ID × 12" or 15" length
- Weight (loaded): 9-11kg
- Pattern: Single horizontal line

#### Consumer V-Fan Racks

**24-Shot V-Fan:**
- Dimensions: 36" L × 26" W × 5" H (91 × 66 × 13 cm)
- Layout: 2 rows × 12 tubes
- Angle: 15° divergence from center axis
- Weight (loaded): 18-22kg
- Spread at 50m apex: ~26m wide

#### Consumer W-Fan Racks

**24-Shot W-Fan:**
- Dimensions: 36" L × 36" W × 5" H (91 × 91 × 13 cm)
- Layout: 3 rows × 8 tubes
- Center row: 0° (vertical)
- Outer rows: 15° divergence
- Weight (loaded): 18-22kg

**36-Shot W-Fan:**
- Dimensions: 36" L × 45" W × 5" H (91 × 114 × 13 cm)
- Layout: 3 rows × 12 tubes
- Weight (loaded): 26-30kg

#### Professional Bar Racks

**3" Display Bar (8-tube):**
- Dimensions: 30" L × 6" W × 48" H (76 × 15 × 122 cm)
- Frame: 1.5" steel square tube
- Tube spacing: 3.5" (8.9cm) center-to-center
- Weight (loaded): 30-40kg

**4" Display Bar (6-tube):**
- Dimensions: 24" L × 8" W × 60" H (61 × 20 × 152 cm)
- Frame: 2" steel square tube
- Weight (loaded): 45-60kg

**5" Display Bar (4-tube):**
- Dimensions: 20" L × 10" W × 72" H (51 × 25 × 183 cm)
- Weight (loaded): 60-80kg

### Safety Standards

#### NFPA 1123 Requirements

**Chain-Fused Rack Limits:**
- **≤3" shells:** Max 15 tubes per chain
- **4" shells:** Max 12 tubes per chain
- **5-6" shells:** Max 10 tubes per chain
- **>6" shells:** No chain-fusing allowed

#### Spectator Safety Distances

| Shell Size | Minimum Distance | Fallout Radius |
|------------|------------------|----------------|
| **1.75"** | 35m | ±10m |
| **2"** | 43m | ±15m |
| **3"** | 64m | ±20m |
| **4"** | 85m | ±25m |
| **5"** | 107m | ±30m |
| **6"** | 128m | ±35m |
| **8"** | 171m | ±50m |
| **10"** | 213m | ±60m |
| **12"** | 256m | ±75m |

**Distance Calculation:**
```
Minimum Distance = Shell Diameter (inches) × 70 feet
                 = Shell Diameter (inches) × 21.3 meters
```

---

## Effects Types - Visual Reference {#effects-types}

### Spherical Break Effects

#### Peony
- **Description:** Spherical break of colored stars without trails
- **Visual:** Clean burst, stars fade quickly
- **Common in:** Consumer fireworks, basic displays
- **Game use:** Simple burst particle effect

#### Chrysanthemum
- **Description:** Spherical break with visible spark trails
- **Visual:** Like peony but stars leave glittering tails
- **Common in:** Professional displays, premium consumer
- **Game use:** Particle trails, more complex than peony

#### Dahlia
- **Description:** Fewer, larger stars that travel longer distance
- **Visual:** Bigger, bolder than peony, fewer points
- **Shell shape:** Often cylindrical for larger stars
- **Game use:** Hero shots, featured explosions

### Falling Effects

#### Willow
- **Description:** Long-burning stars that fall slowly
- **Visual:** Drooping branches like a willow tree
- **Common in:** Gold/silver effects
- **Game use:** Cascading particle systems

#### Palm
- **Description:** Thick rising stem followed by drooping effect
- **Visual:** Gold/silver stem + palm fronds
- **Common in:** Gold palm trees
- **Game use:** Two-stage effect (rise + fall)

#### Horsetail
- **Description:** Compact burst falling straight down
- **Visual:** Tight vertical fall like horse tail
- **Game use:** Vertical particle cascade

#### Waterfall
- **Description:** Heavy long-burning stars, short travel, free-fall
- **Visual:** Named for waterfall shape
- **Game use:** Heavy gravity particle effect

### Specialty Effects

#### Brocade
- **Description:** Silver tail effect, glitter-based
- **Visual:** Umbrella pattern of spark trails
- **Brightness:** Brighter than willow
- **Game use:** Glitter particle trails

#### Kamuro (Crown)
- **Description:** Dense spherical burst of thousands of gold sparks
- **Visual:** Thick golden sphere, very bright
- **Japanese name:** "Crown"
- **Game use:** High particle count effect (500-2000 particles)

#### Spider
- **Description:** Fast burn, hard burst, flat shooting
- **Visual:** Straight radial lines like spider legs
- **Game use:** Sharp linear particle rays

#### Crossette
- **Description:** Large stars break into smaller stars mid-flight
- **Visual:** Grid pattern with crackling sound
- **Sound:** Loud crackling
- **Game use:** Multi-stage particle split

### Visual Modifiers

#### Pistil
- **Description:** Center cluster of different color/effect
- **Visual:** Core + outer shell (different colors)
- **Game use:** Nested particle systems

#### Strobe
- **Description:** Stars flash on/off rapidly
- **Visual:** Shimmering/pulsing light
- **Game use:** Flashing particle alpha animation

#### Glitter
- **Description:** Slow-burning metallic sparkle
- **Visual:** Long-lasting shimmer
- **Game use:** Persistent sparkle particles

#### Crackle (Dragon Eggs)
- **Description:** Small explosions with crackling sound
- **Visual:** Popping bursts
- **Sound:** Rapid crackling
- **Game use:** Audio-visual particle pops

---

## Chemistry & Colors {#chemistry-colors}

### Color Production Mechanism

**Basic principle:** Metal salts produce colors when heated
1. Heat excites electrons in metal atoms
2. Electrons jump to higher energy level
3. Electrons return to normal state
4. Energy released as light at specific wavelength
5. Each metal = distinct color wavelength

### Primary Color Compounds

#### Red
- **Primary compound:** Strontium salts (SrCO₃, Sr(NO₃)₂)
- **Alternative:** Lithium compounds
- **Wavelength:** ~650-700 nm
- **Game color:** `#FF0000` to `#FF3333`

#### Orange
- **Primary compound:** Calcium salts (CaCl₂, CaSO₄)
- **Wavelength:** ~585-620 nm
- **Game color:** `#FF6600` to `#FF9933`

#### Yellow / Gold
- **Primary compound:** Sodium salts (NaNO₃)
- **Wavelength:** ~585-595 nm
- **Game color:** `#FFFF00` to `#FFD700`
- **Note:** Very intense, bright yellow

#### Green
- **Primary compound:** Barium salts with chlorine (Ba(ClO₃)₂, BaCl₂)
- **Wavelength:** ~500-560 nm
- **Game color:** `#00FF00` to `#66FF33`
- **Note:** Requires chlorine donor for best color

#### Blue
- **Primary compound:** Copper compounds (CuCl₂, CuCO₃)
- **Wavelength:** ~450-490 nm
- **Game color:** `#0066FF` to `#3399FF`
- **Note:** **Hardest color to produce** - requires precise temperature

#### Purple / Violet
- **Mixture:** Strontium (red) + Copper (blue)
- **Game color:** `#9933FF` to `#CC33FF`
- **Note:** Not a pure spectral color

#### White
- **Primary compounds:** Magnesium (Mg), Aluminum (Al), Titanium (Ti)
- **Wavelength:** Full spectrum
- **Game color:** `#FFFFFF` with bloom
- **Note:** Very bright, often used as core

#### Silver / Gray
- **Primary compound:** Aluminum powder
- **Game color:** `#C0C0C0` to `#E8E8E8`
- **Use:** Spark trails, brocade/willow effects

### Color Temperature Notes

**Hot Colors (Easy):**
- Red: 800-1000°C
- Orange: 1000-1200°C
- Yellow: 1200-1600°C
- White: 1600°C+

**Cool Colors (Difficult):**
- Green: 800-1000°C (requires chlorine)
- Blue: 800-900°C (very narrow range)

**Game implication:** Blue is rarest/most premium in realistic displays

### Brightness & Visibility

**Brightness Scale:**
1. White/Silver: Brightest (full spectrum)
2. Yellow: Very bright (sodium intense)
3. Green: Bright
4. Red: Medium-bright
5. Orange: Medium
6. Blue: Dimmest (hardest to see from distance)

**Distance Visibility:**
- **Best at distance:** Yellow, white, green
- **Moderate:** Red, orange
- **Worst:** Blue, purple

### Game Color Palette

**Realistic Display Palette:**
```
Red:     #FF2244  (strontium red)
Orange:  #FF7733  (calcium orange)
Yellow:  #FFD700  (sodium gold)
Green:   #44FF44  (barium green)
Blue:    #3388FF  (copper blue)
Purple:  #AA44FF  (mixed)
White:   #FFFFFF  (magnesium)
Silver:  #D0D0D0  (aluminum)
Gold:    #FFB347  (iron sparkle)
```

**HDR / Bloom Values:**
- White/Yellow: 200-300% overbright
- Green/Red: 150-200%
- Blue/Purple: 100-150%

---

## Game Development Guidelines {#game-development}

### Visual Scale Reference

**Tube height is the strongest visual anchor:**
- 1.75" consumer: **30-40 cm tall** (baseline scale)
- 3" display: **45-50 cm tall**
- 6" display: **80-90 cm tall**
- 10" display: **120 cm tall**

### Material Representation

**HDPE (consumer/common):**
- Color: Matte black or safety orange
- Finish: Slightly rough texture
- Weathering: Scuff marks, dirt accumulation
- Reflectivity: Low (10-20%)

**Fiberglass (professional):**
- Color: Bright yellow or natural tan
- Finish: Smooth, glossy (resin surface)
- Weathering: Edge chipping, resin cracks
- Reflectivity: Medium (30-40%)

### Physical Accuracy

**For realistic scenes:**
- Show bottom plugs (HDPE: molded; fiberglass: separate cap)
- Include fuse holes near bottom
- Add mounting hardware (stakes, brackets, sand bags)
- Show slight angle variations (±2-5°)
- Include safety equipment (buckets, extinguishers, sand)

**For stylized/game scenes:**
- May simplify bottom plugs
- Can use uniform angles
- May omit safety equipment
- Acceptable to use single material family

### Behavioral Animation

**Setup Sequence:**
1. Place rack (ground contact, slight settle)
2. Adjust angle (small rotations)
3. Load shells (insert from top, slight bounce)
4. Connect fuses (character interaction)
5. Step back (safety clearance)

**Firing Sequence:**
1. Ignition flash (bright, momentary)
2. Fuse burn (sparks along fuse line)
3. Launch flash (muzzle bloom)
4. Tube recoil (slight backward jerk)
5. Smoke emission (gray-white plume)
6. Repeat for each tube

### Audio Design

**Rack Handling:**
- Placement: Thud, slight rattle (HDPE), creak (wood)
- Shell loading: Slide, seating thunk
- Fuse handling: Rustling, tape tearing

**Firing Audio:**
- Ignition: Sharp crack (cap ignition)
- Fuse burn: Sizzle, hiss
- Launch: Deep thump, pressure wave
- Tube recoil: Metal clang (bar racks), wood creak (crates)

### Performance Tiers

**Low:**
- Peony, simple single-color bursts
- 50-200 particles per burst

**Medium:**
- Chrysanthemum with trails, palms
- 100-300 particles with trails

**High:**
- Kamuro (high particle count), multi-break
- 500-2000 particles

**Ultra:**
- Strobe effects, complex multi-stage
- 2000+ particles, multiple effects combined

### Common Mistakes to Avoid

**Incorrect Scale:**
- Racks too small (tubes look like toys)
- Racks too large (tubes become structural elements)
- **Fix:** Use tube height as anchor (30-40cm consumer, 120cm professional)

**Unrealistic Patterns:**
- Random tube angles (racks are designed for consistency)
- Excessive tube density (ignores safety spacing)
- **Fix:** Use standard patterns (straight, V, W)

**Material Errors:**
- Shiny plastic (HDPE is matte)
- Rusty consumer racks (HDPE doesn't rust)
- Pristine professional crates (wood gets weathered)
- **Fix:** Match material to rack type

**Animation Errors:**
- Instantaneous setup (racks need physical handling time)
- No recoil on launch (pressure causes movement)
- Tubes fire without ignition (need fuse burn or electric signal)
- **Fix:** Add setup and ignition sequences

---

## Quick Reference Tables {#quick-reference}

### Tube Dimensions Quick Reference

| Shell | ID | OD | Length | Weight | Apex Height |
|-------|----|----|--------|--------|-------------|
| 1.75" | 4.9cm | 6.1cm | 30-38cm | Light | 30-60m |
| 3" | 7.6cm | 8.9cm | 45-51cm | Medium | 60-100m |
| 6" | 15.2cm | 16.5cm | 84cm | Heavy | 100-150m |
| 10" | 25.4cm | 27.3cm | 122cm | Very Heavy | 150-250m |

### Rack Dimensions Quick Reference

| Rack Type | Shot Count | Size (L×W×H cm) | Weight (kg) |
|-----------|-----------|-----------------|-------------|
| Small consumer | 6 | 46 × 33 × 13 | 7.3 |
| Standard consumer | 12 | 91 × 33 × 13 | 14.5 |
| Fan consumer | 24-V | 91 × 66 × 13 | 29 |
| Wide fan consumer | 24-W | 91 × 91 × 13 | 29 |
| Finale consumer | 36-W | 91 × 114 × 13 | 43 |
| Pro 3" bar | 8 | 112 × 20 × 60 | 30-35 |
| Pro 4" bar | 6 | 99 × 25 × 70 | 35-40 |

### Effects Particle Count Reference

| Effect | Particle Count | Lifetime | Complexity |
|--------|---------------|----------|------------|
| Peony | 50-200 | 1-2s | Low |
| Chrysanthemum | 100-300 | 2-3s | Medium |
| Willow | 100-300 | 2-4s | Medium |
| Kamuro | 500-2000 | 1-2s | High |
| Crossette | 200-500 | 2-3s | High |

### Color Chemistry Quick Reference

| Color | Metal | Temperature | Difficulty | Visibility |
|-------|-------|-------------|------------|------------|
| Red | Strontium | 800-1000°C | Easy | Medium |
| Yellow | Sodium | 1200-1600°C | Easy | Excellent |
| Green | Barium | 800-1000°C | Medium | Good |
| Blue | Copper | 800-900°C | Hard | Poor |
| White | Magnesium | 1600°C+ | Easy | Excellent |

### Safety Distance Quick Reference

| Shell Size | Min Distance | Use Case |
|------------|--------------|----------|
| 1.75" | 35m | Backyard consumer |
| 3" | 64m | Small professional |
| 6" | 128m | Large professional |
| 10" | 213m | Major displays |

---

## Sources & Standards

**Technical Standards:**
- NFPA 1123: Code for Fireworks Display (2020)
- EN 15947-5: Pyrotechnic articles - Display fireworks
- GB 10631: Safety standards for fireworks (China)

**Material Data:**
- ASTM D4976 (polyethylene pressure pipe)
- ASTM D3039 (tensile testing)

**Manufacturer Specifications:**
- American Wholesale Fireworks
- Pyro Supply, PyroDirect
- Great Lakes Mortar Racks
- Pro Pyro Racks, PyroBoom

**Field References:**
- Natural Resources Canada: Display Fireworks Manual
- California Fire Marshal: Fireworks Guidelines
- UK HSE: Storing and Using Fireworks
- Pyrotechnics Guild International (PGI)

---

**Last Updated:** 2026-06-08  
**Version:** 1.0 Complete

**Related Files:**
- [[mortar-tubes|Mortar Tubes Reference]]
- [[racks|Rack Systems Reference]]
- [[effects-types|Effects Types Reference]]
- [[chemistry-colors|Chemistry & Colors Reference]]
- [[index|Fireworks Index]]
