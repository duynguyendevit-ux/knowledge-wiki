---
title: Fireworks Rack Systems - Technical Reference
tags: [fireworks, engineering, safety, configuration]
date: 2026-06-08
---

# Fireworks Rack Systems - Technical Reference

## Introduction

A fireworks rack is a structural assembly that holds multiple mortar tubes in a fixed geometric configuration. Racks serve three primary functions:

1. **Safety:** Maintain correct tube angles and spacing
2. **Efficiency:** Enable rapid sequential or simultaneous firing
3. **Choreography:** Create geometric break patterns

**Key Principle:** Rack configuration determines visual pattern; tube specifications determine height and power.

## Rack Classification

### By Tube Count
- **Small:** 1-6 tubes (testing, accents)
- **Medium:** 8-24 tubes (standard consumer/pro)
- **Large:** 25-50 tubes (finale racks)
- **Array:** 50+ tubes (synchronized displays)

### By Pattern Type
- **Straight/Linear:** Single row, uniform spacing
- **V-Fan:** Two angled rows diverging from center
- **W-Fan:** Three rows (center straight, sides angled)
- **Circular:** Tubes arranged in ring pattern
- **Custom:** Irregular patterns for specific effects

### By Construction
- **Consumer Modular:** Plastic injection-molded (HDPE)
- **Professional Bar:** Steel/aluminum rail systems
- **Wood Crate:** Plywood box frames
- **Ground-Set:** Individual buried tubes
- **Elevated:** Mounted on towers/platforms

## Engineering Principles

### Structural Requirements

**Load Distribution:**
```
Total Weight = (Tube Weight × Count) + (Shell Weight × Count) + Frame Weight

Typical example (12-shot consumer):
= (12 × 0.5kg) + (12 × 0.2kg) + 3kg
= 6kg + 2.4kg + 3kg
= 11.4kg total
```

**Base Stability:**
- Center of gravity must remain within base footprint
- Safety factor: 1.5-2.0× against tipping
- Wind loading: 40-60 km/h survival (outdoor displays)

**Tube Support:**
- Minimum contact: 20-30% of tube length
- Maximum unsupported span: 40cm between supports
- Deflection limit: <2° angle deviation under load

### Spacing Requirements

**NFPA 1123 Minimum Tube Separation:**
- **2" shells:** No minimum specified (practical: 2-3")
- **3" shells:** 2" clear space between tubes
- **4" shells:** 2" clear space
- **5-6" shells:** 3" clear space
- **8" shells:** 4" clear space

**Engineering Rationale:**
- Prevents sympathetic detonation (tube-to-tube ignition)
- Allows thermal dissipation between firings
- Provides access for inspection and fuse connection
- Enables safe malfunction handling

**Practical Spacing (Consumer Racks):**
- Tube OD: 2.4" (6.1cm)
- Clear space: 0.5-1.0" (1.3-2.5cm)
- Center-to-center pitch: 3.0-3.5" (7.6-8.9cm)

**Example: 12-shot straight rack**
```
Rack Length = (12 tubes × 3" pitch) + 2" end margins
           = 36" + 2"
           = 38" (96.5cm) total
```

### Fan Angle Calculations

**V-Fan Configuration:**
- Standard divergence: **15° per side** from center axis
- Total spread angle: 30°
- Reasoning: Creates visible separation without excessive ground footprint

**Geometry:**
```
For 12 tubes per row, 3" spacing:
Row length = 36" (91.4cm)

Horizontal spread at apex (100m height):
tan(15°) = spread / height
spread = 100m × tan(15°)
       = 100m × 0.268
       = 26.8m per side
Total spread = 53.6m at 100m altitude
```

**W-Fan Configuration:**
- Center row: 0° (vertical)
- Outer rows: 15° divergence
- Creates three distinct break zones
- Total spread: 3× single row width

### Material Selection by Load

**Consumer Racks (1.75" shells, 6-36 tubes):**
- **Frame:** HDPE injection molded or wood
- **Tube holders:** Molded HDPE sleeves
- **Base:** Integrated plastic or plywood
- **Weight capacity:** 10-25kg total
- **Lifespan:** 50-100 uses (HDPE), 10-20 uses (wood)

**Professional Bar Racks (3"-6" shells, 4-12 tubes):**
- **Frame:** Steel box tube or aluminum I-beam
- **Tube mounts:** Welded steel rings or clamps
- **Base:** Steel legs with ground stakes
- **Weight capacity:** 50-150kg
- **Lifespan:** 500+ uses

**Professional Crates (3"-6" shells, 6-15 tubes):**
- **Frame:** 3/4" (19mm) plywood with 2×4 bracing
- **Tube support:** Wood blocks or foam inserts
- **Base:** Integrated plywood floor
- **Weight capacity:** 50-100kg
- **Lifespan:** 5-20 shows (repairable)

## Standard Rack Configurations

### Consumer Straight Racks

#### 6-Shot Straight
- **Dimensions:** 18" L × 13" W × 5" H (46 × 33 × 13 cm)
- **Tube size:** 1.91" ID × 12" length
- **Tube spacing:** 3" (7.6cm) center-to-center
- **Weight (empty):** 3.5-4.5kg
- **Weight (loaded):** 5.5-6.5kg
- **Pattern:** Single horizontal line
- **Typical use:** Small backyard shows, testing

#### 12-Shot Straight
- **Dimensions:** 36" L × 13" W × 5" H (91 × 33 × 13 cm)
- **Tube size:** 1.91" ID × 12" or 15" length
- **Tube spacing:** 3" (7.6cm) center-to-center
- **Weight (empty):** 6-8kg
- **Weight (loaded):** 9-11kg
- **Pattern:** Single horizontal line
- **Typical use:** Standard consumer displays

**Design Features:**
- Injection-molded HDPE base
- Integrated tube sleeves (no separate mounting)
- Drainage holes (prevent water accumulation)
- Carry handles on ends
- Stackable design (3-4 racks high for storage)

### Consumer V-Fan Racks

#### 24-Shot V-Fan
- **Dimensions:** 36" L × 26" W × 5" H (91 × 66 × 13 cm)
- **Layout:** 2 rows × 12 tubes
- **Angle:** 15° divergence from center axis
- **Tube spacing:** 3" (7.6cm) within row
- **Row separation:** 8-10" (20-25cm)
- **Weight (loaded):** 18-22kg
- **Pattern:** Two diverging lines
- **Spread at 50m apex:** ~26m wide

**Row Angle Calculation:**
```
Inner edge to center: ~13" (33cm)
Outer edge to center: ~31" (79cm)

Angle = arctan((31-13) / row_length)
      = arctan(18 / 36)
      = arctan(0.5)
      ≈ 26.5° total spread
      ≈ 13° per side from horizontal center

Tube angles: 15° from vertical
```

### Consumer W-Fan Racks

#### 24-Shot W-Fan
- **Dimensions:** 36" L × 36" W × 5" H (91 × 91 × 13 cm)
- **Layout:** 3 rows × 8 tubes
- **Center row:** 0° (vertical)
- **Outer rows:** 15° divergence
- **Weight (loaded):** 18-22kg
- **Pattern:** Three-zone break

#### 36-Shot W-Fan
- **Dimensions:** 36" L × 45" W × 5" H (91 × 114 × 13 cm)
- **Layout:** 3 rows × 12 tubes
- **Weight (loaded):** 26-30kg
- **Pattern:** Three-zone wide break
- **Typical use:** Consumer finale

**Visual Effect:**
- Center row: Vertical column
- Side rows: Outer wings
- Combined: W-shaped break pattern
- Width advantage: 1.5× wider than straight, 1.2× wider than V-fan

### Professional Bar Racks

#### 3" Display Bar (8-tube)
- **Dimensions:** 30" L × 6" W × 48" H (76 × 15 × 122 cm)
- **Frame:** 1.5" steel square tube
- **Tube mounts:** 3.5" OD clamp rings
- **Tube spacing:** 3.5" (8.9cm) center-to-center
- **Weight (empty):** 15-20kg
- **Weight (loaded):** 30-40kg
- **Base:** Folding legs with stake points

#### 4" Display Bar (6-tube)
- **Dimensions:** 24" L × 8" W × 60" H (61 × 20 × 152 cm)
- **Frame:** 2" steel square tube
- **Tube mounts:** 4.5" OD clamp rings
- **Tube spacing:** 4" (10.2cm) center-to-center
- **Weight (empty):** 20-25kg
- **Weight (loaded):** 45-60kg

#### 5" Display Bar (4-tube)
- **Dimensions:** 20" L × 10" W × 72" H (51 × 25 × 183 cm)
- **Frame:** 2" steel square tube (reinforced)
- **Tube mounts:** 5.5" OD clamp rings
- **Tube spacing:** 5" (12.7cm) center-to-center
- **Weight (empty):** 25-30kg
- **Weight (loaded):** 60-80kg

**Bar Rack Advantages:**
- Reusable (500+ shows)
- Adjustable tube angles (clamp rotation)
- Quick tube replacement
- Weather-resistant (galvanized steel)
- Stackable for transport

**Bar Rack Disadvantages:**
- Heavy (difficult to move when loaded)
- Expensive ($100-300 USD per rack)
- Requires tools for assembly
- Overkill for consumer shells

### Professional Crate Racks

#### 3" Crate (12-tube)
- **Dimensions:** 36" L × 14" W × 24" H (91 × 36 × 61 cm)
- **Frame:** 3/4" plywood with 2×4" pine bracing
- **Tube support:** Foam inserts or wood blocks
- **Tube arrangement:** 2 rows × 6 tubes
- **Weight (empty):** 10-15kg
- **Weight (loaded):** 35-50kg

#### 4" Crate (9-tube)
- **Dimensions:** 30" L × 18" W × 30" H (76 × 46 × 76 cm)
- **Layout:** 3 rows × 3 tubes (grid pattern)
- **Weight (loaded):** 50-70kg

#### Mixed Crate (3", 4", 5" combination)
- **Common config:** 4×3" + 4×4" + 2×5"
- **Dimensions:** 36" L × 24" W × 32" H (91 × 61 × 81 cm)
- **Weight (loaded):** 60-90kg
- **Visual effect:** Staggered timing creates layered breaks

**Crate Design Features:**
- Diagonal corner bracing (prevents racking)
- Rope handles (4-person carry)
- Open top (allows fuse access)
- Reinforced bottom (distributes ground load)
- Repairable (replace damaged panels)

**Crate Disadvantages:**
- Limited reuse (5-20 shows)
- Bulky storage
- Moisture damage (wood warping)
- Fire risk (wood frame)

### Modular Rack Systems

#### ARC Sleeve System (Consumer)
- **Module size:** 17.5" L × 3" W (44.5 × 7.6 cm)
- **Capacity:** 6 tubes per sleeve
- **Tube pitch:** 2.9" (7.4cm) center-to-center
- **Connection:** Sliding dovetail rails
- **Scalability:** Connect 2-12 sleeves per rail
- **Advantages:**
  - Compact storage
  - Flexible configuration
  - Damaged modules replaceable
  - Cost-effective ($15-25 per 6-tube module)

**Example Configurations:**
- 2 sleeves = 12-shot straight
- 3 sleeves = 18-shot straight
- 4 sleeves × 2 rows = 48-shot double straight
- 6 sleeves × 3 rows = 108-shot finale array

## Safety Standards & Regulations

### NFPA 1123 Requirements

**Rack Construction:**
- Non-combustible or fire-resistant materials
- Secure tube mounting (no loose tubes)
- Stable base (tip-over test: 30° without failure)
- Clear identification (shell size, tube count)

**Chain-Fused Rack Limits:**
- **≤3" shells:** Max 15 tubes per chain
- **4" shells:** Max 12 tubes per chain
- **5-6" shells:** Max 10 tubes per chain
- **>6" shells:** No chain-fusing allowed (individual electric match)

**Rationale:**
- Limits maximum instantaneous explosive weight
- Allows malfunction isolation
- Reduces crew exposure time

**Rack Placement:**
- Minimum 15' (4.6m) separation between racks (3-4" shells)
- Minimum 25' (7.6m) separation (5-6" shells)
- Minimum 50' (15.2m) separation (8"+ shells)

### Spectator Safety Distances

**NFPA 1123 Minimum Distances:**

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

Example for 6" shell:
= 6 × 70 feet
= 420 feet
= 128 meters
```

**Fallout Radius:**
- Area where burning debris may land
- Typically ±50% of minimum distance
- Requires clear zone (no combustibles, vehicles, structures)

### European Standards (EN 15947-5)

**Additional Requirements:**
- CE marking on professional racks
- Tube pressure testing documentation
- Angle deviation testing (±2° tolerance)
- Wind load certification (60 km/h minimum)

**Differences from US:**
- Stricter reinforcement for 7"+ tubes
- Mandatory secondary containment (sand boxes, blast shields)
- Lower chain-fuse limits (8 tubes max for 4" shells)

## Rack Setup & Operation

### Ground Preparation

**Level Surface:**
- Maximum slope: 2° (3.5% grade)
- If sloped, tilt racks uphill (maintain vertical tube angle)
- Use shims or sandbags for leveling

**Soil Conditions:**
- Firm soil: Direct placement OK
- Soft soil: Use plywood base plates (24" × 24" minimum)
- Sand: Bury rack legs 6-12" deep
- Concrete: Use sandbags for stability (no staking)

**Weather Considerations:**
- Wind >40 km/h: Guy wires or sandbag weights
- Rain: Cover fuses, inspect tubes for water
- Cold (<0°C): Check HDPE for brittleness
- Heat (>35°C): Reduce firing rate (prevent tube overheating)

### Tube Angle Verification

**Tools:**
- Digital inclinometer (±0.5° accuracy)
- Plumb bob (low-tech backup)
- Laser level (multi-tube verification)

**Acceptable Tolerances:**
- **Consumer displays:** ±5°
- **Professional displays:** ±2°
- **Competition/sync shows:** ±1°

**Correction Methods:**
- Shims under rack legs
- Adjustable clamps (bar racks)
- Sand banking (ground-set tubes)

### Loading Sequence

**Safety Protocol:**
1. Verify rack stability
2. Inspect tubes (cracks, obstructions)
3. Load shells (heaviest at bottom if mixed sizes)
4. Verify shell orientation (fuse up)
5. Connect fuses/igniters
6. Final angle check
7. Clear personnel (minimum 50' during firing)

**Shell Insertion:**
- Lower gently (avoid dropping)
- Verify full seating (shell base touches tube bottom)
- Check fuse clearance (no pinching at muzzle)

### Firing Sequence

**Manual Firing (Hand-lit fuses):**
1. Light fuses from upwind side
2. Move lateral to rack (never directly in front)
3. Maintain 15-20' distance during burn
4. Count shots (verify all tubes fired)

**Electric Firing:**
1. Test continuity (each igniter)
2. Arm firing panel
3. Initiate sequence
4. Monitor for misfires
5. Wait 15 minutes before approaching misfires

**Chain-Fused Firing:**
1. Single ignition point
2. Fuse burns sequentially tube-to-tube
3. Timing: 0.5-2 seconds between tubes
4. No electrical required
5. Cannot stop mid-sequence

## Rack Storage & Maintenance

### Post-Show Inspection

**Tube Checks:**
- Cracks from thermal stress
- Deformation from overpressure
- Muzzle damage from shell scraping
- Fuse hole enlargement

**Frame Checks:**
- Wood: Cracks, char damage, loose joints
- Steel: Weld cracks, rust, deformation
- HDPE: Melting, warping, stress whitening

**Cleaning:**
- Remove ash, debris, unburned powder
- Wash HDPE with soap and water
- Wire-brush steel frames (remove rust)
- Inspect while clean (easier to spot damage)

### Storage Conditions

**Indoor (Ideal):**
- Temperature: 10-30°C
- Humidity: 30-60%
- UV protection: No direct sunlight
- Ventilation: Prevent mold/mildew

**Outdoor (Acceptable):**
- Cover with tarp (UV-resistant)
- Elevate off ground (prevent moisture wicking)
- Secure against wind
- Inspect monthly for weather damage

**Stacking Limits:**
- Consumer HDPE racks: 4-5 high (prevent bottom deformation)
- Professional bar racks: Lay flat (2 high maximum)
- Crates: 2 high only (wood crushing risk)

### Retirement Criteria

**Mandatory Retirement:**
- Any crack in tube body
- Deformation >5% of nominal diameter
- Muzzle damage >1" (2.5cm)
- Frame structural failure (broken welds, cracked wood)
- Heat damage (melting, charring >30% surface)

**Recommended Retirement:**
- HDPE consumer: After 100 firings
- HDPE professional: After 200 firings
- Wood crates: After 20 shows
- Steel bar racks: After visible deformation

## Game Development Guidelines

### Visual Representation

**Rack Hierarchy (by prominence):**
1. **Hero racks:** High-detail, foreground, player-interactive
2. **Supporting racks:** Medium detail, mid-ground, ambient
3. **Background racks:** Low detail, distant, atmosphere

**Level of Detail (LOD) by Distance:**
- **0-5m:** Full geometry (screws, welds, labels)
- **5-15m:** Simplified geometry (major features only)
- **15-50m:** Proxy mesh (basic shape)
- **>50m:** Billboard/sprite

### Geometric Accuracy

**Consumer Racks:**
- Use straight/V-fan/W-fan patterns
- 3" tube spacing (consistent)
- Matte black or orange plastic material
- Height: 30-40cm (matches tube length)

**Professional Bar Racks:**
- Steel construction (metallic shader)
- 4-8 tubes per rack
- Folding legs with ground stakes
- Height: 120-180cm (tall, imposing)

**Professional Crates:**
- Wood construction (weathered wood texture)
- Rope handles, diagonal bracing
- Mixed tube sizes (visual variety)
- Height: 60-90cm

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

**Post-Fire State:**
- Smoke continues (30-60 seconds)
- Char marks around muzzle
- Heat shimmer above tubes
- Occasional ember glow

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

## Sources & References

**Standards & Regulations:**
- NFPA 1123: Code for Fireworks Display (2020)
- EN 15947-5: Pyrotechnic articles - Display fireworks
- Natural Resources Canada: Display Fireworks Manual
- California Fire Marshal: Fireworks Safety Guidelines

**Manufacturer Specifications:**
- American Wholesale Fireworks: Rack catalogs
- Pyro Supply: Professional bar racks
- Great Lakes Mortar Racks: Consumer HDPE racks
- PyroBoom: Modular ARC systems

**Field Documentation:**
- Pyrotechnics Guild International (PGI): Safety guidelines
- UK HSE: Fireworks storage and use
- Australian Standard AS 2187.2: Explosives - Storage and use

---

**Related:** [[fireworks/index|Fireworks Index]] | [[mortar-tubes|Mortar Tubes]] | [[effects-types|Effects Types]]
