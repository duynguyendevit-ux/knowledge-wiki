---
title: Fireworks Chemistry & Colors - Complete Technical Reference
tags: [fireworks, chemistry, colors, vfx-reference, game-design]
date: 2026-06-08
---

# Fireworks Chemistry & Colors - Complete Technical Reference

Comprehensive guide to fireworks color production, chemical compounds, and game rendering implementation.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Color Production Mechanism](#color-mechanism)
3. [Primary Color Compounds](#primary-colors)
4. [Metallic Effects](#metallic-effects)
5. [Color Mixing & Transitions](#color-mixing)
6. [Brightness & Visibility](#brightness)
7. [Game Implementation](#game-implementation)
8. [Technical Specifications](#technical-specs)

---

## Introduction {#introduction}

Firework colors are produced by heating metal salts to specific temperatures. Each metal produces a characteristic wavelength of light, creating distinct colors visible from long distances.

**Key Principle:** Color is determined by metal chemistry, not dyes or pigments. Temperature control is critical for color purity.

---

## Color Production Mechanism {#color-mechanism}

### Basic Physics

**How fireworks produce color:**

1. **Heat:** Burning lift charge heats metal salts
2. **Excitation:** Electrons jump to higher energy level
3. **Return:** Electrons fall back to ground state
4. **Emission:** Energy released as light (specific wavelength)
5. **Color:** Wavelength determines color we see

**Chemical Formula:**
```
Metal Salt + Heat → Excited Atoms → Light Emission

Example (Strontium - Red):
Sr + Heat (800-1000°C) → Sr* (excited) → Red light (650-700nm) + Sr
```

### Temperature Dependence

**Critical factor:** Each metal has an optimal temperature range

- **Too cold:** Insufficient excitation, dim or no color
- **Optimal:** Bright, pure color
- **Too hot:** Different emission lines, color impurity

**Temperature ranges:**
- **Red (Strontium):** 800-1000°C
- **Orange (Calcium):** 1000-1200°C
- **Yellow (Sodium):** 1200-1600°C
- **Green (Barium):** 800-1000°C (requires chlorine)
- **Blue (Copper):** 800-900°C (narrow range - hardest to produce)
- **White (Magnesium):** 1600°C+

---

## Primary Color Compounds {#primary-colors}

### Red

**Primary Metal:** Strontium (Sr)

**Common Compounds:**
- **Strontium carbonate (SrCO₃):** Most common, stable
- **Strontium nitrate (Sr(NO₃)₂):** Oxidizer, bright red
- **Strontium sulfate (SrSO₄):** Less common
- **Strontium oxalate (SrC₂O₄):** High-purity applications

**Alternative Metal:** Lithium (Li)
- **Lithium carbonate (Li₂CO₃):** Deeper red, less common
- **Lithium chloride (LiCl):** Very intense, rarely used

**Properties:**
- **Wavelength:** 650-700 nm
- **Temperature:** 800-1000°C
- **Difficulty:** Easy to produce
- **Brightness:** Medium-high
- **Visibility:** Good at distance

**Game Color Values:**
- **Base:** `#FF0000`
- **Realistic:** `#FF2244` (strontium red)
- **Deep:** `#CC0022` (lithium red)
- **Bright:** `#FF3333` (high-intensity)

**HDR/Bloom:** 150-200% overbright

---

### Orange

**Primary Metal:** Calcium (Ca)

**Common Compounds:**
- **Calcium chloride (CaCl₂):** Most common
- **Calcium sulfate (CaSO₄):** Alternative
- **Calcium carbonate (CaCO₃):** Less effective

**Properties:**
- **Wavelength:** 585-620 nm
- **Temperature:** 1000-1200°C
- **Difficulty:** Easy
- **Brightness:** Medium
- **Visibility:** Good

**Game Color Values:**
- **Base:** `#FF6600`
- **Realistic:** `#FF7733` (calcium orange)
- **Bright:** `#FF8844`

**HDR/Bloom:** 150-180%

**Notes:**
- Often mixed with red/yellow to adjust shade
- Less common than red or yellow as primary color

---

### Yellow / Gold

**Primary Metal:** Sodium (Na)

**Common Compounds:**
- **Sodium nitrate (NaNO₃):** Most common, bright yellow
- **Sodium oxalate (Na₂C₂O₄):** High purity
- **Cryolite (Na₃AlF₆):** Industrial grade

**Properties:**
- **Wavelength:** 585-595 nm (very narrow, pure yellow)
- **Temperature:** 1200-1600°C
- **Difficulty:** Easy to produce
- **Brightness:** VERY HIGH (brightest visible color)
- **Visibility:** Excellent (best at distance)

**Game Color Values:**
- **Base:** `#FFFF00` (pure yellow)
- **Realistic:** `#FFD700` (gold)
- **Sodium:** `#FFDD00` (sodium yellow)
- **Warm gold:** `#FFB347`

**HDR/Bloom:** 200-300% overbright (brightest effect)

**Notes:**
- Sodium is extremely intense
- Can overpower other colors if mixed
- Most visible color at long distances
- "Gold" effects typically use iron/aluminum, not sodium

---

### Green

**Primary Metal:** Barium (Ba)

**Common Compounds:**
- **Barium chlorate (Ba(ClO₃)₂):** Best green, requires chlorine
- **Barium nitrate (Ba(NO₃)₂):** Good green
- **Barium chloride (BaCl₂):** With chlorine donor

**Critical Requirement:**
- **Needs chlorine donor** for best color
- Without chlorine: Weak, yellowish-green
- With chlorine: Bright, pure green

**Chlorine Donors:**
- PVC (polyvinyl chloride)
- Chlorinated rubber
- Perchlorates

**Properties:**
- **Wavelength:** 500-560 nm
- **Temperature:** 800-1000°C
- **Difficulty:** Medium (requires chlorine chemistry)
- **Brightness:** High
- **Visibility:** Good

**Game Color Values:**
- **Base:** `#00FF00`
- **Realistic:** `#44FF44` (barium green)
- **Bright:** `#66FF33`
- **Emerald:** `#00CC66`

**HDR/Bloom:** 150-200%

**Safety Note:**
- Barium compounds are toxic
- Environmental concerns in some regions

---

### Blue

**Primary Metal:** Copper (Cu)

**Common Compounds:**
- **Copper chloride (CuCl₂):** Most common
- **Copper carbonate (CuCO₃):** Basic blue copper carbonate
- **Copper oxide (CuO):** Black copper oxide
- **Copper sulfate (CuSO₄):** Less effective

**Critical Requirements:**
- **Very narrow temperature range:** 800-900°C
- **Requires chlorine donor** (like green)
- **Temperature control critical**

**Properties:**
- **Wavelength:** 450-490 nm
- **Temperature:** 800-900°C (narrow!)
- **Difficulty:** HARD (hardest color to produce)
- **Brightness:** Low-medium (dimmest)
- **Visibility:** Poor at distance

**Why Blue is Hard:**
1. Narrow temperature range (±50°C tolerance)
2. Too hot → green tint
3. Too cold → dim or no color
4. Requires precise fuel mixture
5. Affected by combustion products

**Game Color Values:**
- **Base:** `#0066FF`
- **Realistic:** `#3388FF` (copper blue)
- **Bright:** `#4499FF`
- **Deep:** `#0055CC`

**HDR/Bloom:** 100-150% (compensate for visibility)

**Game Consideration:**
- Blue is rarest/most expensive in realistic shows
- May need brightness boost for visibility
- Premium/high-budget displays use more blue

---

### Purple / Violet

**Method:** Mixture of red and blue compounds

**Composition:**
- **Red:** Strontium compounds
- **Blue:** Copper compounds
- **Ratio:** Varies to adjust shade

**Properties:**
- **Wavelength:** Mixed (not pure spectral color)
- **Temperature:** Must balance red and blue requirements
- **Difficulty:** Hard (blue chemistry + mixing)
- **Brightness:** Medium

**Game Color Values:**
- **Base:** `#9933FF`
- **Realistic:** `#AA44FF` (red-violet)
- **Deep:** `#6622CC`
- **Bright:** `#CC33FF`

**HDR/Bloom:** 120-180%

**Notes:**
- Not a pure spectral color (combination)
- Challenging to produce (blue difficulty)
- Less common than primary colors

---

### White

**Primary Metals:**
- **Magnesium (Mg):** Bright white, most common
- **Aluminum (Al):** Silver-white, sparkly
- **Titanium (Ti):** Brilliant white spark

**Mechanism:**
- Burns at very high temperature (1600°C+)
- Emits full spectrum (all wavelengths)
- Appears as bright white

**Properties:**
- **Wavelength:** Full spectrum (380-750 nm)
- **Temperature:** 1600°C+
- **Difficulty:** Easy
- **Brightness:** EXTREME (brightest effect)
- **Visibility:** Excellent

**Game Color Values:**
- **Pure white:** `#FFFFFF`
- **Magnesium:** `#FFFFEE` (slight warm)
- **Titanium:** `#FFFFFF` (pure)
- **Aluminum:** `#F0F0F0` (silver-white)

**HDR/Bloom:** 200-300% overbright (very bright)

**Common Uses:**
- Core/pistil effects
- Strobe effects
- Salutes (flash powder)
- Accent stars

---

### Silver / Gray

**Primary Metal:** Aluminum (Al) powder

**Mechanism:**
- Creates spark trails
- Reflects light (metallic)
- Burns with silver color

**Properties:**
- **Appearance:** Silver-gray sparks
- **Use:** Trails, brocade, willow effects
- **Brightness:** High

**Game Color Values:**
- **Silver:** `#C0C0C0`
- **Bright silver:** `#E8E8E8`
- **Dark silver:** `#A0A0A0`

**HDR/Bloom:** 150-200%

---

## Metallic Effects {#metallic-effects}

### Gold Sparkle

**Compounds:**
- **Iron filings (Fe):** Primary gold color
- **Charcoal (C):** Fuel and color
- **Aluminum (Al):** Brightness

**Mechanism:**
- Burning iron creates gold sparks
- Not pure spectral color
- Creates trailing sparks

**Visual Characteristics:**
- **Color:** Warm gold (#FFB347)
- **Trail:** Long-lasting sparks
- **Brightness:** High
- **Duration:** 2-4 seconds

**Common Effects:**
- Chrysanthemum tails
- Palm effects
- Willow effects
- Brocade patterns

**Game Implementation:**
- **Main particle:** Warm gold
- **Trail particles:** Smaller gold sparks
- **Lifetime:** Long (2-4s per spark)
- **Brightness:** High with bloom

---

### Silver Sparkle

**Compounds:**
- **Aluminum powder:** Primary sparkle
- **Titanium powder:** Extra brightness

**Visual Characteristics:**
- **Color:** Bright white/silver
- **Trail:** Bright spark trails
- **Brightness:** Very high
- **Duration:** 1-3 seconds

**Common Effects:**
- Brocade effects
- Glitter tails
- Strobe stars
- Flash effects

**Game Implementation:**
- **Color:** Bright white/silver (#E8E8E8)
- **Bloom:** Very high (200-300%)
- **Sparkle:** Rapid alpha flicker

---

### Crackling (Dragon Eggs)

**Compounds:**
- **Bismuth trioxide (Bi₂O₃):** Primary
- **Lead tetroxide (Pb₃O₄):** Alternative (banned in many places)

**Mechanism:**
- Small micro-explosions
- Creates crackling sound
- Brief bright flashes

**Visual Characteristics:**
- **Color:** White flash
- **Duration:** 0.05-0.1s per pop
- **Frequency:** 5-20 pops/second
- **Brightness:** Very high (brief flash)

**Game Implementation:**
- **Flash event:** Brief white particle
- **Duration:** 0.05-0.1s
- **Audio:** Sync crackling sound
- **Timing:** Random intervals

---

## Color Mixing & Transitions {#color-mixing}

### Possible Combinations

**Successful Mixes:**
- **Purple:** Red (strontium) + Blue (copper)
- **Pink:** Red (strontium) + White (magnesium)
- **Teal:** Green (barium) + Blue (copper)
- **Amber:** Yellow (sodium) + Orange (calcium)

**Methodology:**
- Mix metal compounds in same star
- Both metals emit simultaneously
- Colors blend visually

### Impossible Mixes

**Cannot Create:**
- **Green from Yellow + Blue:** Different chemistry, not additive mixing
- Pure spectral colors can only come from specific metals

**Why:**
- Firework colors are emission spectra, not pigments
- Each metal emits specific wavelengths
- Cannot "mix" wavelengths chemically

### Color-Changing Stars

**Mechanism:** Layered compounds burn in sequence

**Construction:**
- **Layer 1 (outside):** First color compound
- **Layer 2 (middle):** Transition layer
- **Layer 3 (core):** Second color compound

**Burn Sequence:**
1. Outside layer burns first → Color 1
2. Middle layer burns → Transition
3. Core burns → Color 2

**Common Transitions:**
- **Green → Red:** Barium exterior, strontium core
- **Blue → Silver:** Copper exterior, aluminum core
- **Gold → Red:** Iron exterior, strontium core

**Timing:**
- Transition time: 0.5-2 seconds
- Depends on layer thickness

**Game Implementation:**
- **Color interpolation:** Lerp between colors over time
- **Timing:** Match transition duration
- **Particle system:** Gradually change emissive color

---

## Brightness & Visibility {#brightness}

### Brightness Scale

**Relative brightness (from brightest to dimmest):**

1. **White/Silver** (Mg/Al) - 100% reference
2. **Yellow** (Na) - 90% (extreme intensity)
3. **Green** (Ba) - 70%
4. **Red** (Sr) - 60%
5. **Orange** (Ca) - 50%
6. **Blue** (Cu) - 30% (dimmest)
7. **Purple** (Sr+Cu) - 40%

### Distance Visibility

**Best at distance:**
- **Yellow:** Excellent (brightest, pure wavelength)
- **White:** Excellent (full spectrum)
- **Green:** Good (bright, mid-spectrum)

**Moderate at distance:**
- **Red:** Medium (dimmer than yellow/green)
- **Orange:** Medium

**Worst at distance:**
- **Blue:** Poor (dimmest, easily lost)
- **Purple:** Poor (contains blue)

**Game Consideration:**
- **Camera distance:** Scale blue brightness up for visibility
- **Realistic shows:** Fewer blue shells (expensive, dim)
- **Game shows:** Can boost blue for player experience

### Color Temperature

**Concept:** Color temperature affects visual perception

**Hot Colors (appear brighter):**
- White: 6500K+ (daylight)
- Yellow: 3000-4000K (warm)
- Orange: 2500-3000K

**Cool Colors (appear dimmer):**
- Green: 5000-7000K
- Blue: 7000-9000K (cool)

**Game Implementation:**
- **Emissive temperature:** Match to color
- **Bloom amount:** Higher for hot colors
- **HDR values:** Scale with brightness

---

## Game Implementation {#game-implementation}

### Realistic Display Color Palette

**Primary Colors:**
```
Red:     #FF2244  (strontium red)
Orange:  #FF7733  (calcium orange)
Yellow:  #FFD700  (sodium gold)
Green:   #44FF44  (barium green)
Blue:    #3388FF  (copper blue)
Purple:  #AA44FF  (strontium + copper)
White:   #FFFFFF  (magnesium)
```

**Metallic Effects:**
```
Gold:    #FFB347  (iron sparkle)
Silver:  #D0D0D0  (aluminum)
```

### HDR / Bloom Values

**Recommended overbright multipliers:**

| Color | HDR Multiplier | Bloom Strength |
|-------|----------------|----------------|
| **White** | 200-300% | Very High |
| **Yellow** | 200-300% | Very High |
| **Green** | 150-200% | High |
| **Red** | 150-200% | Medium-High |
| **Orange** | 150-180% | Medium |
| **Blue** | 100-150% | Medium (boost for visibility) |
| **Purple** | 120-180% | Medium |
| **Gold** | 180-250% | High |
| **Silver** | 200-300% | Very High |

### Material Setup (PBR)

**Emissive Material:**
```
Base Color: Color from palette
Emissive: Same color × HDR multiplier
Metallic: 0.0 (non-metallic)
Roughness: 1.0 (fully rough)
Alpha: Animated (fade over lifetime)
```

**Trail Particles:**
```
Base Color: Slightly desaturated
Emissive: Lower than main particle (50-80%)
Size: Smaller (20-50% of main)
Lifetime: Shorter
```

### Color Composition Guidelines

**Budget-Friendly Shows (realistic):**
- **Heavy use:** Red, green, white (cheap compounds)
- **Moderate use:** Yellow, orange
- **Light use:** Blue, purple (expensive, difficult)

**Premium Shows:**
- **More blue:** Indicates high budget
- **Color transitions:** Expensive, impressive
- **Complex pistil combinations**

**Game Freedom:**
- Can use any color distribution
- Boost blue brightness for player experience
- Not bound by cost/difficulty constraints

### Particle Emissive Setup

**Shader Properties:**
```glsl
// Base emissive color
vec3 emissiveColor = baseColor;

// HDR multiplier (based on color)
float hdrMultiplier = 2.0; // 200% for most colors

// Bloom contribution
vec3 emission = emissiveColor * hdrMultiplier;

// Time-based fade
float alpha = 1.0 - (lifetime / maxLifetime);
emission *= alpha;

// Final output
fragColor = vec4(emission, alpha);
```

### Color Distance Falloff

**Simulate atmospheric perspective:**

```
// Reduce saturation with distance
float distanceFactor = saturate(distance / maxDistance);
vec3 desaturated = mix(color, vec3(luminance), distanceFactor * 0.3);

// Reduce brightness with distance
float brightnessFalloff = 1.0 / (1.0 + distance * 0.01);
vec3 final = desaturated * brightnessFalloff;
```

---

## Technical Specifications {#technical-specs}

### Color Wavelengths

| Color | Wavelength (nm) | Frequency (THz) |
|-------|-----------------|-----------------|
| **Red** | 650-700 | 430-460 |
| **Orange** | 585-620 | 484-512 |
| **Yellow** | 585-595 | 504-512 |
| **Green** | 500-560 | 536-600 |
| **Blue** | 450-490 | 612-667 |
| **Violet** | 400-450 | 667-750 |
| **White** | 380-750 | Full spectrum |

### Temperature Ranges

| Color | Optimal Temp (°C) | Tolerance | Difficulty |
|-------|-------------------|-----------|------------|
| **Red** | 800-1000 | ±100°C | Easy |
| **Orange** | 1000-1200 | ±100°C | Easy |
| **Yellow** | 1200-1600 | ±200°C | Easy |
| **Green** | 800-1000 | ±100°C | Medium |
| **Blue** | 800-900 | ±50°C | Hard |
| **White** | 1600+ | ±200°C | Easy |

### Cost & Availability (Realistic)

| Color | Relative Cost | Availability | Common Use |
|-------|---------------|--------------|------------|
| **Red** | Low | Excellent | Very Common |
| **Green** | Low | Excellent | Very Common |
| **White** | Low | Excellent | Very Common |
| **Yellow** | Low-Medium | Excellent | Common |
| **Orange** | Medium | Good | Moderate |
| **Blue** | High | Good | Rare |
| **Purple** | High | Good | Rare |

---

## Quick Reference

### Color-Metal Chart

| Color | Metal | Formula Example | Difficulty | Brightness |
|-------|-------|-----------------|------------|------------|
| Red | Strontium | SrCO₃ | Easy | Medium |
| Orange | Calcium | CaCl₂ | Easy | Medium |
| Yellow | Sodium | NaNO₃ | Easy | Very High |
| Green | Barium | Ba(ClO₃)₂ | Medium | High |
| Blue | Copper | CuCl₂ | Hard | Low |
| Purple | Sr + Cu | Mixed | Hard | Medium |
| White | Magnesium | Mg | Easy | Extreme |
| Gold | Iron | Fe | Easy | High |
| Silver | Aluminum | Al | Easy | Very High |

### Game Color Palette

```
#FF2244  Red (strontium)
#FF7733  Orange (calcium)
#FFD700  Yellow (sodium)
#44FF44  Green (barium)
#3388FF  Blue (copper)
#AA44FF  Purple (mixed)
#FFFFFF  White (magnesium)
#FFB347  Gold (iron)
#D0D0D0  Silver (aluminum)
```

---

## Sources & References

**Chemistry Documentation:**
- Pyrotechnic Chemistry: Principles and Applications
- Journal of Pyrotechnics: Color production studies
- American Chemical Society: Fireworks chemistry

**Field Standards:**
- NFPA 1123: Color specifications
- Natural Resources Canada: Chemical compound references
- Pyrotechnics Guild International: Best practices

**Safety Documentation:**
- OSHA: Chemical safety for pyrotechnics
- EPA: Environmental impact studies
- International Fireworks Regulations

---

**Last Updated:** 2026-06-08  
**Related:** [[01-mortar-tubes-complete|Mortar Tubes]] | [[02-rack-systems-complete|Rack Systems]] | [[03-effects-types-complete|Effects Types]]
