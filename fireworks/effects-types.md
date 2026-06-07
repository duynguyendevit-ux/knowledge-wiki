---
title: Fireworks Effects Types Reference
tags: [fireworks, vfx, game-design, visual-reference]
date: 2026-06-07
---

# Fireworks Effects Types Reference

Visual guide to common firework shell effects for game VFX and animation.

## Spherical Break Effects

### Peony
**Description:** Spherical break of colored stars without trails
**Visual:** Clean burst, stars fade quickly
**Common in:** Consumer fireworks, basic displays
**Game use:** Simple burst particle effect

### Chrysanthemum
**Description:** Spherical break with visible spark trails
**Visual:** Like peony but stars leave glittering tails
**Common in:** Professional displays, premium consumer
**Game use:** Particle trails, more complex than peony

### Dahlia
**Description:** Fewer, larger stars that travel longer distance
**Visual:** Bigger, bolder than peony, fewer points
**Shell shape:** Often cylindrical for larger stars
**Game use:** Hero shots, featured explosions

## Falling Effects

### Willow
**Description:** Long-burning stars that fall slowly
**Visual:** Drooping branches like a willow tree
**Common in:** Gold/silver effects
**Game use:** Cascading particle systems

### Palm
**Description:** Thick rising stem followed by drooping effect
**Visual:** Gold/silver stem + palm fronds
**Common in:** Gold palm trees
**Game use:** Two-stage effect (rise + fall)

### Horsetail
**Description:** Compact burst falling straight down
**Visual:** Tight vertical fall like horse tail
**Game use:** Vertical particle cascade

### Waterfall
**Description:** Heavy long-burning stars, short travel, free-fall
**Visual:** Named for waterfall shape
**Game use:** Heavy gravity particle effect

## Specialty Effects

### Brocade
**Description:** Silver tail effect, glitter-based
**Visual:** Umbrella pattern of spark trails
**Brightness:** Brighter than willow
**Game use:** Glitter particle trails

### Kamuro (Crown)
**Description:** Dense spherical burst of thousands of gold sparks
**Visual:** Thick golden sphere, very bright
**Japanese name:** "Crown"
**Game use:** High particle count effect

### Spider
**Description:** Fast burn, hard burst, flat shooting
**Visual:** Straight radial lines like spider legs
**Game use:** Sharp linear particle rays

### Crossette
**Description:** Large stars break into smaller stars mid-flight
**Visual:** Grid pattern with crackling sound
**Sound:** Loud crackling
**Game use:** Multi-stage particle split

## Visual Modifiers

### Pistil
**Description:** Center cluster of different color/effect
**Visual:** Core + outer shell (different colors)
**Game use:** Nested particle systems

### Strobe
**Description:** Stars flash on/off rapidly
**Visual:** Shimmering/pulsing light
**With hundreds:** Looks like water shimmer
**Game use:** Flashing particle alpha animation

### Glitter
**Description:** Slow-burning metallic sparkle
**Visual:** Long-lasting shimmer
**Common in:** Brocade tails
**Game use:** Persistent sparkle particles

### Crackle (Dragon Eggs)
**Description:** Small explosions with crackling sound
**Visual:** Popping bursts
**Sound:** Rapid crackling
**Game use:** Audio-visual particle pops

### Fish
**Description:** Small swimming/darting effects
**Visual:** Erratic movement like fish
**Game use:** Random motion particle behavior

## Color Categories

### Single Color
- Red (strontium)
- Green (barium)
- Blue (copper)
- Yellow/Gold (sodium)
- White (magnesium/aluminum)
- Orange (calcium)

### Multi-Color
- **Bi-color:** Two distinct colors in same shell
- **Rainbow:** Multiple colors in sequence
- **Color-changing:** Stars shift color as they burn

## Break Patterns

### Ring Shell
**Visual:** Circular ring of stars
**Construction:** Stars arranged in ring pattern
**Game use:** Circular particle spawn pattern

### Saturn Shell
**Visual:** Ring with center burst
**Game use:** Nested ring + sphere particles

### Multi-Break
**Description:** Multiple breaks from one shell
**Types:** Double-break, triple-break
**Game use:** Delayed sequential bursts

## Timing & Sequencing

### Rising Tail
**Description:** Colored trail as shell rises
**Visual:** Stem effect before burst
**Game use:** Launch trail particles

### Delayed Break
**Description:** Shell rises higher before bursting
**Visual:** Long pause after launch
**Game use:** Longer particle lifetime before burst

### Salute
**Description:** Flash powder explosion, minimal color
**Visual:** Bright white flash
**Sound:** VERY loud boom
**Game use:** Flash effect + screen shake

## Game Implementation Notes

**Performance tiers:**
- **Low:** Peony, simple single-color bursts
- **Medium:** Chrysanthemum with trails, palms
- **High:** Kamuro (high particle count), multi-break
- **Ultra:** Strobe effects, complex multi-stage

**Common patterns:**
- Peony: 50-200 particles
- Chrysanthemum: 100-300 particles with trails
- Kamuro: 500-2000 particles
- Willow: Long lifetime (2-4s)
- Spider: Fast velocity, short lifetime

**Audio cues:**
- Chrysanthemum: Crackling sound
- Crossette: Sharp crack
- Salute: Deep boom
- Crackle: Rapid popping

## Visual Reference Priority

For realistic game visuals, focus on:
1. **Peony** (most common baseline)
2. **Chrysanthemum** (adds detail)
3. **Willow/Palm** (falling effects)
4. **Brocade** (glitter trails)
5. **Kamuro** (hero moments)

---

**Related:** [[index|Fireworks Index]] | [[mortar-tube-dimensions|Tube Dimensions]] | [[fireworks-chemistry|Chemistry & Colors]]
