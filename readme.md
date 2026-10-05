# Panasonic Lumix DMC-GM5 Replacement Mode Dial Plate

A replacement for the printed plate on the Panasonic Lumix DMC-GM5 mode dial, for cameras whose original plate is missing or worn. The design recreates the mode symbols on a thin circular FR4 plate that can be attached to the existing dial.

## Files

- `Panasonic_GM5_Refined_Silkscreen.svg` — refined vector artwork at actual size, 13.8 × 13.8 mm.
- `cover.kicad_pcb` — circular board outline and front silkscreen artwork.
- `cover.kicad_pro` — KiCad project settings. The board was saved with KiCad 10; no schematic is needed.

## Making the plate

1. Check a 13.8 mm diameter, 0.6 mm thick template on your camera, including the thickness of your intended adhesive. Confirm clearance and alignment with every mode position.
2. Open `cover.kicad_pcb` in KiCad. Export RS-274-X Gerbers for `F.Cu`, `B.Cu`, `F.Mask`, `B.Mask`, `F.SilkS`, `B.SilkS`, and `Edge.Cuts`. Disable X2 if the manufacturer requires classic RS-274-X. The outline is the cut edge; it is not a printed ring.
3. Order a **13.8 mm diameter × 0.6 mm thick FR4 disc**, with black solder mask on the **front only**, white front silkscreen, and a **bare FR4 back**. There are no copper features or holes, so no drill file is needed. Select thickness and colours separately in the order form.
4. Explicitly ask the manufacturer to confirm front-only solder mask and review the fine symbols. Copper, mask-opening, and back-silkscreen layers are intentionally empty; the empty mask files alone do not communicate the different front/back finishes.
5. Dry-fit the finished plate, align the symbols with the dial positions, then attach it with a suitable thin adhesive.

The artwork was refined for small-detail readability, then resized to the current 13.8 mm outline. KiCad design checks pass with zero violations. Physical fit and printed-detail quality still need confirmation on a fabricated sample.
