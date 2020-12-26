# Prusa MK3S Bear Y-Axis Linear Rail Upgrade

<p align="center">
  <img src="img/linear_rail_mod_header.jpg" width="70%">
</p>

## This guide is a work in progress
It is incomplete and subject to change. Use at your own risk.

## ⚠️ CAUTION! ⚠️

Before you begin, make sure you are using [MK3S Bear Upgrade V2.0](https://github.com/gregsaun/prusa_i3_bear_upgrade) or newer because the Y-axis uses the belt holder under the carriage to bump into the Y-axis motor holder. Without this upgrade, it will not pass Prusa's Self Test.

If you're using the [SKR Bear firmware](https://github.com/codiac2600/SKR-Bear-Marlin) this won't be an issue.

## Bill of Materials

| QTY | Length | Description                      | Source                                                                                                                                                                                                                                         |
| :-: | :----: | :------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2   | 370mm  | MGN12 linear rail **\***         |                                                                                                                                                                                                                                                |
| 3   |        | MGN12H carriage block **\***     |                                                                                                                                                                                                                                                |
| 2   | 331mm  | 2020 V-slot extrusion            |                                                                                                                                                                                                                                                |
| 18  | 8mm    | M3 button head or cap head screw | [Amazon](https://amzn.com/B07B8FBT46/) / [OpenBuilds](https://openbuildspartstore.com/button-head-screws-m3-25-pack/) / [McMaster-Carr](https://www.mcmaster.com/91239A113) / [AliExpress](https://www.aliexpress.com/item/4000038065691.html) |
| 6   | 6mm    | M3 flat head screw               | [McMaster-Carr](https://www.mcmaster.com/91294A126) / [AliExpress](https://www.aliexpress.com/item/33049019185.html)                                                                                                                           |
| 18  |        | M3 t-nuts                        | [Amazon](https://amzn.com/B07SDFCTD4/) / [OpenBuilds](https://openbuildspartstore.com/tee-nuts-m3-10-pack/) / [AliExpress](https://www.aliexpress.com/item/32825357262.html)                                                                   |
| 20  | 8mm    | M5 screws                        | [Amazon](https://amzn.com/B07B2RV4K6/) / [OpenBuilds](https://openbuildspartstore.com/low-profile-screws-m5-10-pack/) / [McMaster-Carr](https://www.mcmaster.com/91239A222) / [AliExpress](https://www.aliexpress.com/item/4000038065691.html) |
| 20  |        | M5 t-nuts                        | [Amazon](https://amzn.com/B01HKMF2EE/) / [OpenBuilds](https://openbuildspartstore.com/tee-nuts-m5-10-pack/) / [AliExpress](https://www.aliexpress.com/item/32965780205.html)                                                                   |

**\*** _If you are located in the USA, 2x 370mm MGN12 linear rails with dual carriage blocks from [Printed Solid](https://www.printedsolid.com/products/ldo-linear-rail-mgn12h-with-one-carriage-in-300-400-500-700mm-lengths?variant=31423201149013) will work. You will have one spare carriage block._

### Optional Bill of Materials
| QTY | Description                  | Source                                                                                                    |
| :-: | :--------------------------- | :-------------------------------------------------------------------------------------------------------- |
| 6   | 2028 aluminum corner bracket | [Amazon](https://amzn.com/B07B8FBT46/) / [AliExpress](https://www.aliexpress.com/item/4000767697780.html) |

## Printed Parts

Print all the parts below:

| QTY | Description                                                               |
| :-: | :------------------------------------------------------------------------ |
| 3   | [Bearing Spacer](stl/bearing-spacer.stl)                                  |
| 4   | [Rail Guard](stl/front-rail-guard-1-2.stl)                                |
| 2   | [MGN12 Linear Rail Alignment Tool](stl/linear_rail_alignment_tool-v1.stl) |
| 1   | [2020 Extrusion Build Helper](stl/build_helper_y-mgn12-mod-v3.stl)           |
| 6   | [Corner Bracket](stl/corner-bracket-1.0-vv.stl) **\*\***                  |

**\*\*** _Not needed if you purchased 6x 2028 aluminum corner brackets._


### Recommended Print Settings

- Filament material: PETG/ABS/ASA/PC/Nylon (Not PLA)
- Infill: 30% Gyroid
- Resolution: 0.2mm
- Supports: No
- Raft: No

## Assembly Guide

### This guide is a work in progress
It is incomplete and subject to change. Use at your own risk.

### Step 1 - Prepare Printer

Remove your bed, Y carriage, 8mm rods & bearings, and front & rear Y rod holders. You will only reuse your bed & Y carriage for this mod.

### Step TK - Prepare linear rails

Install 2x MGN12H carriage blocks on one MGN rail and 1x MGN12H carriage block on the second linear rail.

### Step TK - Mount linear rails to 2020 Extrusion

Attach linear rails to each 331mm 2020 V-slot extrusion using 9x M3x8 screws and M3 t-nuts. Use 2x printed [MGN12 Linear Rail Alignment Tools](stl/linear_rail_alignment_tool-v1.stl) to help align the linear rails on the 2020 extrusion.

### Step TK - Mount 2020 Extrusion to Bear Frame

Mount assembled linear rail and extrusion to the Bear frame using 6x M5x8 screws, 6x M5 t-nuts, and 6x printed [Corner Brackets](stl/corner-bracket-1.0-vv.stl) with 2x brackets in the front and 1x in the back, opposite of the Y-axis motor.

Ensure the linear rail with 2x MGN12H carriage blocks are on the left.

Leave the rightmost extrusion and rail loose for adjustment later.

Loosen all M5 screws on the leftmost linear rail.

### Step TK

Use [2020 Extrusion Build Helper](stl/build_helper_y-mgn12-mod.stl) to align the left 2020 extrusion/linear rail assembly 50mm to the right of the frame, front and back. Tighten the M5 screws making sure the 2020 extrusion stays aligned.

Install the four printed [Rail Guards](stl/front-rail-guard-1-2.stl) with 8x M5x8 screws & 8x M5 t-nuts to prevent the bed from sliding off the rails. Do not fully tighten M5 screws.

### Step TK

Attach printed [Bearing Spacers](stl/bearing-spacer.stl) to each bearing block with the small end oriented toward the back.

### Step TK

Attach the printed [Bearing Spacers](stl/bearing-spacer.stl) to each MGN12 carriage using 6x M3-6 flathead screws.

Attach the Y carriage to the printed [Bearing Spacers](stl/bearing-spacer.stl) using 6x M3-8 screws. Shift the rightmost rail and extrusion so it lines up without binding.

### Step TK

Tighten the 2020 V-slot extrusion to the frame.

### Step TK

Loosen all screws on rightmost linear rail.

### Step TK

Move the carriage as far forward as possible and tighten the most forward screw on the rail to the extrusion.

### Step TK

Slide the carriage as far back it would go and tighten the back most M3 8mm screw.

### Step TK

Tighten all M3 & M5 screws.

### Step TK

Reinstall bed.

_Repeat Steps TK-TK if your bed isn't sliding smoothly._