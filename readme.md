# Panasonic Lumix DMC-GM5 Replacement Mode Dial Plate

The Panasonic Lumix DMC-GM5 has mode symbols printed directly on the mode dial. These markings can wear off with use. This project restores them with a thin circular plate carrying the mode symbols, glued or attached to the top of the existing dial.

## Files

- `Panasonic_GM5_Refined_Silkscreen.svg` — refined vector artwork at actual size, 13.8 × 13.8 mm.
- `cover.kicad_pcb` — circular board outline and front silkscreen artwork.
- `cover.kicad_pro` — KiCad project settings. The board was saved with KiCad 10; no schematic is needed.

## Making the plate as a PCB

The method below describes ordering the plate through PCBWay. It can also be used with similar PCB manufacturing services; confirm their export requirements and available finishes before ordering.

1. Open `cover.kicad_pcb` in KiCad. Export RS-274-X Gerbers for `F.Cu`, `B.Cu`, `F.Mask`, `B.Mask`, `F.SilkS`, `B.SilkS`, and `Edge.Cuts`. Disable X2 if the manufacturer requires classic RS-274-X. The outline is the cut edge; it is not a printed ring.
2. Order a **13.8 mm diameter × 0.6 mm thick FR4 disc**, with black solder mask on the **front only**, white front silkscreen, and a **bare FR4 back**. There are no copper features or holes, so no drill file is needed. Select thickness and colours separately in the order form.
3. Explicitly ask the manufacturer to confirm front-only solder mask and review the fine symbols. Copper, mask-opening, and back-silkscreen layers are intentionally empty; the empty mask files alone do not communicate the different front/back finishes.
4. Dry-fit the finished plate on top of the existing mode dial, align the symbols with the dial positions, then glue or attach it with a suitable thin adhesive.

The artwork was refined for small-detail readability, then resized to the current 13.8 mm outline. KiCad design checks pass with zero violations. Physical fit and printed-detail quality still need confirmation on a fabricated sample.
