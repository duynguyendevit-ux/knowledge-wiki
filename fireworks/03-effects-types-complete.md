---
title: Fireworks Effects Types - Complete Visual Reference
tags: [fireworks, vfx, effects, visual-reference, game-design]
date: 2026-06-08
---

# Fireworks Effects Types - Complete Visual Reference

Comprehensive visual guide to firework shell effects for game VFX, animation, and technical implementation.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Spherical Break Effects](#spherical-breaks)
3. [Falling Effects](#falling-effects)
4. [Specialty Effects](#specialty-effects)
5. [Visual Modifiers](#visual-modifiers)
6. [Break Patterns](#break-patterns)
7. [Timing & Sequencing](#timing)
8. [Game Implementation](#game-implementation)

---

## Introduction {#introduction}

Firework effects are created by the arrangement, composition, and timing of pyrotechnic stars within shells. Each effect type has distinct visual characteristics, particle behavior, and audio signatures.

**Classification System:**
- **Break type:** How the shell bursts (spherical, directional, multi-stage)
- **Star behavior:** How particles move and burn (falling, rising, splitting)
- **Visual modifiers:** Additional effects (glitter, strobe, crackle)

---

## Spherical Break Effects {#spherical-breaks}

### Peony

**Description:**
- Spherical break of colored stars without trails
- Stars radiate outward from center point
- Clean, simple burst pattern
- Stars fade quickly (1-2 seconds)

**Visual Characteristics:**
- **Shape:** Perfect sphere
- **Star count:** 50-200 stars
- **Trail:** None (stars burn without tail)
- **Color:** Solid single or multi-color
- **Brightness:** Medium

**Common Uses:**
- Consumer fireworks (most common type)
- Basic professional displays
- Budget-friendly shows
- Quick accent shots

**Game Implementation:**
- **Particle count:** 50-200
- **Velocity:** Uniform radial (spherical distribution)
- **Lifetime:** 1-2 seconds
- **Trail:** None
- **Fade:** Linear alpha decay

**Audio:**
- Launch: Deep thump
- Break: Sharp pop
- Burn: Quiet hiss

---

### Chrysanthemum

**Description:**
- Spherical break with visible spark trails
- Like peony but stars leave glittering tails
- More complex and visually rich
- Premium consumer and professional standard

**Visual Characteristics:**
- **Shape:** Sphere with trailing lines
- **Star count:** 100-300 stars
- **Trail:** Long golden/silver sparks
- **Trail length:** 2-5 meters
- **Brightness:** High (glitter sparkle)

**Common Uses:**
- Professional displays
- Premium consumer products
- High-visibility shows
- Signature effects

**Game Implementation:**
- **Particle count:** 100-300 main stars + trail particles
- **Main star velocity:** Radial uniform
- **Trail:** Spawn sub-particles along path (5-10 per star)
- **Trail lifetime:** 0.5-1 second per spark
- **Color:** Gold/silver trails, colored core

**Audio:**
- Launch: Deep thump
- Break: Sharp crack
- Burn: Loud crackling (from sparks)

**Variants:**
- **Golden chrysanthemum:** Gold star trails
- **Silver chrysanthemum:** Silver/white trails
- **Color chrysanthemum:** Colored stars with contrasting trails

---

### Dahlia

**Description:**
- Fewer, larger stars that travel longer distance
- Bold, dramatic appearance
- Bigger stars = bigger visual impact
- Often used in cylindrical shells

**Visual Characteristics:**
- **Shape:** Sparse sphere
- **Star count:** 20-80 stars (fewer than peony)
- **Star size:** Large (visually 2-3× peony stars)
- **Travel distance:** Long (slower burn = longer flight)
- **Brightness:** Very high

**Common Uses:**
- Professional displays
- Hero shots (featured effects)
- Large-caliber shells (6"+)
- Dramatic moments

**Game Implementation:**
- **Particle count:** 20-80
- **Particle size:** Large (2-3× peony)
- **Velocity:** Moderate (less than peony)
- **Lifetime:** 2-4 seconds (longer than peony)
- **Spacing:** Visible gaps between stars

**Audio:**
- Launch: Deep boom (large shell)
- Break: Heavy thud
- Burn: Loud hiss (large stars)

---

## Falling Effects {#falling-effects}

### Willow

**Description:**
- Long-burning stars that fall slowly
- Drooping branches like a willow tree
- Classic gold/silver effect
- Graceful, elegant appearance

**Visual Characteristics:**
- **Initial shape:** Sphere or rising stem
- **Falling pattern:** Arcs downward (parabolic)
- **Trail:** Long streaming sparks
- **Duration:** 2-4 seconds
- **Color:** Typically gold or silver

**Physics:**
- Stars burn slowly (long lifetime)
- Gravity pulls stars downward
- Creates characteristic drooping pattern
- Wind affects trajectory visibly

**Common Uses:**
- Classic professional effects
- Gold/silver specialty shows
- Traditional displays
- Elegant moments

**Game Implementation:**
- **Particle count:** 100-300
- **Initial velocity:** Radial burst
- **Gravity:** Strong (particles fall noticeably)
- **Trail:** Long spark trails (5-10 sub-particles per star)
- **Lifetime:** 2-4 seconds
- **Wind influence:** Optional (particles drift)

**Audio:**
- Launch: Moderate thump
- Break: Soft pop
- Burn: Sustained crackling

**Variants:**
- **Golden willow:** Gold stars and trails
- **Silver willow:** Silver/white trails
- **Weeping willow:** Longer, more drooping

---

### Palm

**Description:**
- Thick rising stem followed by drooping effect
- Two-stage visual: rise + fall
- Classic gold effect
- Named for palm tree appearance

**Visual Characteristics:**
- **Stage 1:** Rising gold stem (2-3 seconds)
- **Stage 2:** Burst into drooping trails
- **Color:** Typically gold (silver variants exist)
- **Height:** Rises higher than break point
- **Duration:** 3-5 seconds total

**Physics:**
- Initial thrust creates rising stars
- Stars burn and slow down
- Gravity takes over → falling pattern
- Combined effect looks like palm tree

**Common Uses:**
- Professional displays
- Gold specialty shows
- Signature palm tree effects
- Traditional celebrations

**Game Implementation:**
- **Stage 1 (rise):** Vertical particles, upward velocity
- **Stage 2 (burst):** Spawn new particles at apex
- **Fall pattern:** Parabolic with trails
- **Particle count:** 50-150 (stage 1) + 200-500 (stage 2)
- **Timing:** 2s rise + 3s fall

**Audio:**
- Launch: Deep thump
- Rising: Sustained hiss
- Break: Moderate pop
- Falling: Crackling cascade

---

### Horsetail

**Description:**
- Compact burst falling straight down
- Tight vertical fall pattern
- Named for horse tail appearance
- Less spread than willow

**Visual Characteristics:**
- **Shape:** Vertical column
- **Width:** Narrow (10-20° spread)
- **Fall pattern:** Nearly vertical
- **Trail:** Medium length sparks
- **Duration:** 2-3 seconds

**Game Implementation:**
- **Particle count:** 100-200
- **Initial velocity:** Low radial spread
- **Gravity:** Very strong (fast fall)
- **Spread angle:** 10-20° from vertical
- **Trail:** Moderate spark trails

---

### Waterfall

**Description:**
- Heavy long-burning stars
- Short initial travel, then free-fall
- Very dramatic falling effect
- Named for waterfall appearance

**Visual Characteristics:**
- **Initial burst:** Minimal spread
- **Fall pattern:** Straight down
- **Visual weight:** Heavy, thick streams
- **Duration:** 3-5 seconds
- **Brightness:** Very high

**Game Implementation:**
- **Particle count:** 200-500
- **Particle size:** Large
- **Initial velocity:** Very low
- **Gravity:** Strong (heavy particles)
- **Trail:** Thick, continuous streams

---

## Specialty Effects {#specialty-effects}

### Brocade

**Description:**
- Silver tail effect, glitter-based
- Umbrella pattern of spark trails
- Brighter than willow
- Premium visual effect

**Visual Characteristics:**
- **Color:** Silver/white dominant
- **Pattern:** Umbrella or inverted cone
- **Brightness:** Very high (glitter sparkle)
- **Trail density:** Very dense
- **Duration:** 2-3 seconds

**Game Implementation:**
- **Particle count:** 300-800 (high density)
- **Trail type:** Glitter sub-particles
- **Color:** Silver (#D0D0D0) with bright highlights
- **Bloom:** High (200-300% overbright)
- **Sparkle:** Random alpha flicker

**Audio:**
- Sharp, bright crackling (like glass breaking)

---

### Kamuro (Crown)

**Description:**
- Dense spherical burst of thousands of gold sparks
- Japanese specialty effect
- Extremely bright and dense
- "Crown" appearance

**Visual Characteristics:**
- **Shape:** Perfect dense sphere
- **Particle count:** 500-2000+ sparks
- **Color:** Pure gold
- **Duration:** 1-2 seconds
- **Brightness:** Extreme (brightest effect)

**Common Uses:**
- Professional Japanese-style displays
- Premium shows
- Hero moments
- Competition displays

**Game Implementation:**
- **Particle count:** 500-2000 (performance intensive)
- **Particle size:** Small (individual sparks)
- **Distribution:** Extremely uniform sphere
- **Color:** Gold (#FFB347)
- **Bloom:** Extreme (300%+ overbright)
- **Optimization:** Use GPU instancing

**Audio:**
- Loud, dense crackling roar

---

### Spider

**Description:**
- Fast burn, hard burst
- Flat, fast-moving stars
- Straight radial lines like spider legs
- Sharp, geometric appearance

**Visual Characteristics:**
- **Shape:** Flat radial pattern
- **Speed:** Very fast star velocity
- **Burn:** Short, intense
- **Pattern:** Geometric, straight lines
- **Duration:** 0.5-1.5 seconds

**Game Implementation:**
- **Particle count:** 50-150
- **Velocity:** High (2-3× normal)
- **Pattern:** Planar (horizontal disk)
- **Lifetime:** Short (0.5-1.5s)
- **Trail:** Minimal or none

**Audio:**
- Sharp, fast crackling

---

### Crossette

**Description:**
- Large stars break into smaller stars mid-flight
- Grid pattern effect
- Loud crackling sound
- Multi-stage visual

**Visual Characteristics:**
- **Stage 1:** Large stars (20-40 count)
- **Stage 2:** Each star splits into 3-5 smaller stars
- **Pattern:** Grid or lattice appearance
- **Sound:** Very loud crackling
- **Duration:** 2-3 seconds total

**Physics:**
- Initial stars contain small charge
- Mid-flight explosion splits star
- Creates branching pattern

**Game Implementation:**
- **Stage 1:** 20-40 large particles
- **Split timing:** 0.5-1s after launch
- **Split count:** 3-5 particles per star
- **Total particles:** 60-200 after split
- **Audio:** Sync crackling to split events

**Audio:**
- Initial: Moderate burst
- Split: Loud sequential cracking (grid pattern)

---

## Visual Modifiers {#visual-modifiers}

### Pistil

**Description:**
- Center cluster of different color/effect
- Core + outer shell design
- Two distinct visual zones
- Adds depth and complexity

**Visual Characteristics:**
- **Core:** Different color than outer
- **Core size:** 20-40% of total diameter
- **Common combinations:**
  - Red pistil + blue outer
  - White pistil + red outer
  - Gold pistil + green outer

**Game Implementation:**
- **Nested particle systems:**
  - Inner system: Core color/effect
  - Outer system: Shell color/effect
- **Spawn timing:** Simultaneous or slight delay
- **Velocity:** Core slightly slower (stays centered)

---

### Strobe

**Description:**
- Stars flash on/off rapidly
- Shimmering, pulsing effect
- With many stars, looks like water shimmer
- Distinctive visual signature

**Visual Characteristics:**
- **Flash rate:** 5-15 Hz (flashes per second)
- **Duty cycle:** 50% (on/off equal time)
- **Effect:** Shimmering, pulsing appearance
- **Colors:** White most common, green variants

**Game Implementation:**
- **Alpha animation:** Square wave (instant on/off)
- **Flash rate:** 8-12 Hz
- **Phase offset:** Randomize per particle (avoid sync)
- **Bloom:** High during "on" phase
- **Performance:** Can use shader for efficiency

**Audio:**
- Rapid popping (matches flash rate)

---

### Glitter

**Description:**
- Slow-burning metallic sparkle
- Long-lasting shimmer
- Common in brocade tails
- Adds visual richness

**Visual Characteristics:**
- **Appearance:** Small, bright sparkles
- **Duration:** Long (2-4 seconds)
- **Color:** Silver, gold, colored variants
- **Pattern:** Scattered throughout main effect

**Game Implementation:**
- **Sub-particles:** Spawn from main particles
- **Size:** Small (0.2-0.5× main particle)
- **Lifetime:** Long (2-4s)
- **Alpha:** Flicker/pulse animation
- **Color:** Bright highlights

---

### Crackle (Dragon Eggs)

**Description:**
- Small explosions with crackling sound
- Popping, snapping effect
- Audio-visual combination
- Adds excitement

**Visual Characteristics:**
- **Appearance:** Small white flashes
- **Sound:** Rapid crackling/popping
- **Timing:** Random throughout effect
- **Brightness:** High (brief flashes)

**Game Implementation:**
- **Pop events:** Random timing per particle
- **Flash:** Brief bright flash (0.1s)
- **Audio:** Sync sound to visual flash
- **Frequency:** 5-20 pops per second
- **Screen shake:** Subtle (optional)

---

### Fish

**Description:**
- Small swimming/darting effects
- Erratic, unpredictable movement
- Named for fish-like motion
- Adds playfulness

**Visual Characteristics:**
- **Movement:** Rapid direction changes
- **Trail:** Short spark trail
- **Pattern:** Chaotic, unpredictable
- **Duration:** 1-2 seconds

**Game Implementation:**
- **Movement:** Perlin noise + random impulses
- **Speed:** Variable (bursts of speed)
- **Direction:** Frequent random changes
- **Trail:** Short particle trail

---

## Break Patterns {#break-patterns}

### Ring Shell

**Description:**
- Circular ring of stars
- Hollow center
- Stars arranged in perfect circle
- Distinctive geometric pattern

**Construction:**
- Stars arranged in ring inside shell
- Break charge in center

**Game Implementation:**
- **Spawn pattern:** Circular ring (torus distribution)
- **Particle count:** 50-200
- **Ring radius:** Variable
- **Thickness:** Thin (single ring)

---

### Saturn Shell

**Description:**
- Ring with center burst
- Two distinct zones: ring + sphere
- Complex, layered effect

**Game Implementation:**
- **Two systems:**
  - Ring particles (outer)
  - Spherical burst (center)
- **Timing:** Simultaneous
- **Colors:** Often contrasting

---

### Multi-Break

**Description:**
- Multiple breaks from single shell
- Sequential or simultaneous bursts
- Creates layered effect

**Types:**
- **Double-break:** Two sequential bursts
- **Triple-break:** Three sequential bursts
- **Split:** Simultaneous multiple bursts

**Game Implementation:**
- **Timing:** Delayed particle system spawns
- **Positions:** Offset burst centers
- **Delay:** 0.5-1.5s between breaks

---

## Timing & Sequencing {#timing}

### Rising Tail

**Description:**
- Colored trail as shell rises
- Visible before main break
- Adds anticipation
- Common in professional displays

**Game Implementation:**
- **Launch phase:** Vertical particle trail
- **Duration:** 2-4 seconds (rise time)
- **Color:** Often gold, can be colored
- **Transition:** Smoothly lead to main break

---

### Delayed Break

**Description:**
- Shell rises higher before bursting
- Long pause after launch
- Creates suspense
- Higher break altitude

**Game Implementation:**
- **Rise time:** Extended (3-6 seconds)
- **Break timing:** Delay particle burst
- **Height:** Calculate accurate apex
- **Player expectation:** Build anticipation

---

### Salute

**Description:**
- Flash powder explosion
- Minimal color, maximum sound
- Very bright white flash
- Extremely loud boom

**Visual Characteristics:**
- **Color:** Bright white
- **Duration:** Brief (0.1-0.3s)
- **Brightness:** Extreme
- **Pattern:** Expanding sphere of light

**Game Implementation:**
- **Flash:** Bright white sphere
- **Duration:** 0.1-0.3 seconds
- **Bloom:** Extreme (500%+ overbright)
- **Screen shake:** Strong
- **Audio:** Very loud boom (bass heavy)

**Common Uses:**
- Finale punctuation
- Dramatic emphasis
- Competition displays
- Audio signature

---

## Game Implementation {#game-implementation}

### Performance Tiers

**Low (60fps target, mobile):**
- **Peony:** 50-100 particles
- **Simple single-color bursts**
- **Minimal trails**
- **No post-processing**

**Medium (60fps target, desktop):**
- **Chrysanthemum:** 100-300 particles with trails
- **Palms, willows:** 200-400 particles
- **Basic post-processing (bloom)**

**High (30-60fps, high-end):**
- **Kamuro:** 500-1000 particles
- **Multi-break effects**
- **Advanced trails and modifiers**
- **Full post-processing**

**Ultra (30fps, cinematic):**
- **Kamuro:** 1000-2000+ particles
- **Complex multi-stage effects**
- **Strobe, glitter, crackle combined**
- **HDR bloom, color grading**

### Particle Count Guidelines

| Effect | Particle Count | Lifetime | Complexity |
|--------|---------------|----------|------------|
| Peony | 50-200 | 1-2s | Low |
| Chrysanthemum | 100-300 + trails | 2-3s | Medium |
| Willow | 100-300 | 2-4s | Medium |
| Kamuro | 500-2000 | 1-2s | High |
| Crossette | 60-200 (after split) | 2-3s | High |
| Brocade | 300-800 | 2-3s | Very High |

### Common Patterns

**Simple burst (peony, chrysanthemum, dahlia):**
```
spawn_pattern: spherical_uniform
velocity: radial from center
lifetime: 1-3 seconds
trail: optional (chrysanthemum)
```

**Falling effect (willow, palm, waterfall):**
```
spawn_pattern: spherical or rising
velocity: radial (moderate to low)
gravity: strong
lifetime: 2-4 seconds
trail: long spark trails
```

**Specialty (kamuro, brocade, spider):**
```
spawn_pattern: varies by effect
particle_count: high (500-2000)
special_features: glitter, strobe, crackle
performance: intensive
```

### Audio Cues

**Launch:**
- **Consumer (1.75"):** Moderate thump (200-400 Hz)
- **Professional (3-6"):** Deep boom (80-200 Hz)
- **Large (8"+):** Very deep boom (40-100 Hz)

**Break:**
- **Peony:** Sharp pop
- **Chrysanthemum:** Sharp crack + sustained crackling
- **Crossette:** Sequential loud cracks (grid pattern)
- **Salute:** Extremely loud boom (bass heavy)

**Burn:**
- **Standard stars:** Quiet hiss
- **Glitter/crackle:** Loud crackling
- **Strobe:** Rapid popping
- **Large stars (dahlia):** Loud hiss

### Visual Priority

**For realistic game visuals, prioritize:**

1. **Peony** (baseline, most common)
2. **Chrysanthemum** (adds detail and richness)
3. **Willow/Palm** (falling effects, classic look)
4. **Brocade** (glitter trails, premium feel)
5. **Kamuro** (hero moments, Japanese style)

**Optional advanced:**
- Crossette (multi-stage complexity)
- Strobe (distinctive visual)
- Pistil (layered effects)

---

## Quick Reference

### Effect Categories

**Spherical Breaks:**
- Peony, Chrysanthemum, Dahlia

**Falling Effects:**
- Willow, Palm, Horsetail, Waterfall

**Specialty:**
- Brocade, Kamuro, Spider, Crossette

**Modifiers:**
- Pistil, Strobe, Glitter, Crackle, Fish

**Patterns:**
- Ring, Saturn, Multi-break

**Timing:**
- Rising tail, Delayed break, Salute

---

## Sources & References

**Visual Documentation:**
- Pyrotechnics Guild International (PGI): Effect classification
- American Pyrotechnics Association (APA): Consumer effects guide
- Japanese Fireworks Association: Traditional effects

**Field Observation:**
- Professional display recordings
- Consumer product catalogs
- Competition display documentation

**Technical References:**
- Natural Resources Canada: Display Fireworks Manual (effect descriptions)
- NFPA 1123: Shell effect standards
- UK HSE: Fireworks visual classification

---

**Last Updated:** 2026-06-08  
**Related:** [[01-mortar-tubes-complete|Mortar Tubes]] | [[02-rack-systems-complete|Rack Systems]] | [[04-chemistry-colors-complete|Chemistry & Colors]]
