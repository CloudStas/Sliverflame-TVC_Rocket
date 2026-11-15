# Throttle arms: SendCutSend laser cutting and bending

Both throttle arms are the **same part**. One is the other turned 180° around the rocket axis, so order **2** of it.

| File | Use |
|---|---|
| [Throttle_Arm_formed.step](Throttle_Arm_formed.step) | Bent 3D part, single solid. **Upload this one.** SendCutSend reads the bend from it. |
| [Throttle_Arm_flat.dxf](Throttle_Arm_flat.dxf) | Flat pattern in mm, 1:1, all on one layer. The dashed line is the centre of the bend. Use this if the STEP upload gives an error. |

## Order settings
- **Material:** Mild Steel (1008 cold rolled), **.059" (1.50 mm)**
- **Quantity:** 2
- **Units:** mm
- **Bending:** on. One 90° bend. With the DXF the app finds the bend from the dashed line. If it asks for a direction, the flange bends **up**, toward you as the DXF is drawn.

## Bend numbers (SendCutSend table for mild steel .059")
| | SendCutSend | This part |
|---|---|---|
| K-factor | .40 | .40 |
| Inside radius | .063" (1.6 mm) | 1.6 mm |
| Bend deduction @ 90° | .1080" | 2.744 mm = .1080" |
| Min formed flange | .309" (7.85 mm) | flange 13.0 mm, base 8.65 mm at its shortest |
| Features clear of die (half of .472") | 6.0 mm | pushrod hole edge 7.5 mm from the bend line |

Flat size: 43.0 × 35.8 mm (1.69" × 1.41"). Each arm weighs about 9.6 g.

## What changed from the Onshape model (CAD/Throttle_Arms.step)
In the Onshape model, the straight edge of the paddle runs into the bend along its whole length. That edge strip is only bent part of the way. A press brake can't make that, because SendCutSend can't form partial bends. Here the bend only spans the 10.9 mm flange. There's a 1.5 mm relief slot between the flange and the paddle, and the paddle edge stays flat out to the same line (y = -0.15). The two closed paddles still leave the same 0.3 mm gap. The flange, the pivot hole (Ø3.3) and the pushrod hole (Ø1.6) are unchanged.

The 1.6 mm pushrod hole will need a small drill to clean up the laser dross.
