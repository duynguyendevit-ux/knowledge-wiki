---
title: Fireworks Chemistry & Colors
tags: [fireworks, chemistry, colors, vfx-reference]
date: 2026-06-07
---

# Fireworks Chemistry & Colors

Chemical compounds and color production in fireworks for accurate game rendering.

## Color Production Mechanism

**Basic principle:** Metal salts produce colors when heated
1. Heat excites electrons in metal atoms
2. Electrons jump to higher energy level
3. Electrons return to normal state
4. Energy released as light at specific wavelength
5. Each metal = distinct color wavelength

## Primary Color Compounds

### Red
**Primary compound:** Strontium salts
- Strontium carbonate (SrCO₃)
- Strontium nitrate (Sr(NO₃)₂)
- Strontium sulfate (SrSO₄)

**Alternative:** Lithium compounds
- Lithium carbonate (Li₂CO₃)
- Less common than strontium

**Wavelength:** ~650-700 nm
**Game color:** `#FF0000` to `#FF3333`

### Orange
**Primary compound:** Calcium salts
- Calcium chloride (CaCl₂)
- Calcium sulfate (CaSO₄)

**Wavelength:** ~585-620 nm
**Game color:** `#FF6600` to `#FF9933`

### Yellow / Gold
**Primary compound:** Sodium salts
- Sodium nitrate (NaNO₃)
- Sodium oxalate (Na₂C₂O₄)
- Cryolite (Na₃AlF₆)

**Wavelength:** ~585-595 nm
**Game color:** `#FFFF00` to `#FFD700`
**Note:** Very intense, bright yellow

### Green
**Primary compound:** Barium salts with chlorine
- Barium chlorate (Ba(ClO₃)₂)
- Barium nitrate (Ba(NO₃)₂)
- Barium chloride (BaCl₂)

**Wavelength:** ~500-560 nm
**Game color:** `#00FF00` to `#66FF33`
**Note:** Requires chlorine donor for best color

### Blue
**Primary compound:** Copper compounds
- Copper chloride (CuCl₂)
- Copper carbonate (CuCO₃)
- Copper oxide (CuO)

**Wavelength:** ~450-490 nm
**Game color:** `#0066FF` to `#3399FF`
**Note:** **Hardest color to produce** - requires precise temperature

### Purple / Violet
**Mixture:** Strontium (red) + Copper (blue)
- Mix of red and blue compounds
- Ratio determines shade

**Game color:** `#9933FF` to `#CC33FF`
**Note:** Not a pure spectral color

### White
**Primary compounds:** 
- Magnesium (Mg) - bright white
- Aluminum (Al) - silver-white
- Titanium (Ti) - brilliant white spark

**Wavelength:** Full spectrum
**Game color:** `#FFFFFF` with bloom
**Note:** Very bright, often used as core

### Silver / Gray
**Primary compound:** Aluminum powder
- Creates spark trails
- Common in brocade/willow effects

**Game color:** `#C0C0C0` to `#E8E8E8`

## Color Temperature Notes

### Hot Colors (Easy)
- **Red:** 800-1000°C
- **Orange:** 1000-1200°C
- **Yellow:** 1200-1600°C
- **White:** 1600°C+

### Cool Colors (Difficult)
- **Green:** 800-1000°C (requires chlorine)
- **Blue:** 800-900°C (very narrow range)

**Game implication:** Blue is rarest/most premium in realistic displays

## Metallic Effects

### Gold Sparkle
**Compounds:**
- Iron filings (Fe)
- Charcoal (C)
- Aluminum (Al)

**Visual:** Long-lasting gold sparks
**Common in:** Chrysanthemum, palm effects

### Silver Sparkle
**Compounds:**
- Aluminum powder
- Titanium powder

**Visual:** Bright white/silver sparks
**Common in:** Brocade, glitter effects

### Crackling (Dragon Eggs)
**Compounds:**
- Bismuth trioxide (Bi₂O₃)
- Lead tetroxide (Pb₃O₄)

**Effect:** Small micro-explosions
**Sound:** Rapid crackling

## Color Mixing

### Possible Combinations
- **Purple:** Red + Blue compounds
- **Pink:** Red + White (less strontium)
- **Teal:** Green + Blue compounds
- **Amber:** Yellow + Orange

### Impossible Mixes
- Can't mix yellow + blue for green (different chemistry)
- Each color needs specific metal compound

## Color Intensity Factors

### Brightness Scale
1. **White/Silver:** Brightest (full spectrum)
2. **Yellow:** Very bright (sodium intense)
3. **Green:** Bright
4. **Red:** Medium-bright
5. **Orange:** Medium
6. **Blue:** Dimmest (hardest to see from distance)

### Distance Visibility
- **Best at distance:** Yellow, white, green
- **Moderate:** Red, orange
- **Worst:** Blue, purple

**Game camera distance:** Scale blue brightness up for visibility

## Color Transition Effects

### Color-Changing Stars
**Mechanism:** Layered compounds burn in sequence
- **Outside layer:** One compound (e.g., green)
- **Core layer:** Different compound (e.g., red)
- **Effect:** Green → Red as it burns

**Common transitions:**
- Green → Red
- Blue → Silver
- Gold → Red

### Strobe Colors
**Common:** White strobe, green strobe
**Rare:** Colored strobes (more complex chemistry)

## Game Color Palette

### Realistic Display Palette
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

### HDR / Bloom Values
- **White/Yellow:** 200-300% overbright
- **Green/Red:** 150-200%
- **Blue/Purple:** 100-150%

## Safety & Realism Notes

### Toxic Compounds (Historical)
- **Barium:** Toxic but still used (green)
- **Copper:** Toxic residue
- **Lead:** Banned in many regions
- **Arsenic:** Historically used, now banned

### Modern Trends
- Moving toward less toxic alternatives
- Environmental regulations affect colors
- Blue remains difficult/expensive

### Budget Implications
- **Cheap shows:** More red, green, white
- **Premium shows:** More blue, complex effects
- **Color distribution:** Not random, cost-driven

## Technical Implementation

### Particle Emissive Colors
Use emissive materials with bloom:
- Red: `emission * 2.0`
- Yellow: `emission * 3.0`
- Blue: `emission * 1.5` (compensate for visibility)

### Color Temperature
- Hot colors: 3000-4000K
- Cool colors: 5000-7000K
- White: 6500K+

### Trail Colors
- Gold trails: Warmer than core burst
- Silver trails: Cooler than core
- Colored trails: Match star compound

---

**Related:** [[index|Fireworks Index]] | [[effects-types|Effects Types]] | [[mortar-tube-dimensions|Tube Dimensions]]
