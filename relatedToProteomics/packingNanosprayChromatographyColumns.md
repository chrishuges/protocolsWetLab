# Packing chromatography columns with integrated nanospray tips <!-- omit in toc -->

This protocol was last updated - May 15, 2020 by Chris Hughes.

This document describes a protocol for making chromatography columns that have integrated nanospray tips. Although this protocol describes packing into pulled capillaries, it can also be used as a guideline for packing into standard fritted capillaries to make trap, or analytical columns. A key aspect of this protocol is that it utilizes an extra nanoLC pump in order to push beads from a packed reservoir into the column. I acknowledge that not everyone will have access to an extra instrument, and in this case you can just use the packing bomb for the whole procedure. However, the nanoLC does not need to be top-of-the-line. The system we use is quite old, has a pressure max around 5,000 psi, and is no longer capable of providing a reliable gradient. We acquired it for free from a lab where it was just taking up space on a shelf.

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [Reagents and materials](#reagents-and-materials)
- [Solution recipes](#solution-recipes)
- [Protocol](#protocol)
- [Notes](#notes)

<hr style="height:6pt; visibility:hidden;" />

<span id="reagents-and-materials"></span>

## Reagents and materials

- Acetonitrile, HPLC grade (Thermo Scientific, CAT#51101)
- Water, HPLC grade (Thermo Scientific, CAT#51140)
- Methanol, HPLC grade (Sigma, CAT#34860-4L)
- Formic acid, HPLC grade (CAT#85178, Thermo Scientific)
- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- Laser puller (Sutter Instruments, CAT#P-2000)
- 200um internal diameter fused silica (Molex, CAT#TSP200350)
- 150um internal diameter fused silica (Molex, CAT#TSP150375)
- Standard metal benchtop tube heating block (for example, VWR, CAT#75838-282)
- Sonicating water bath (multiple vendors)
- Handheld butane torch (Home Depot sells these for a few dollars)
- Standard internal union (VICI, CAT#ZU.5)
- MicroTight Sleeve Red (IDEX-HS, CAT#F-180)
- Capillary packing bomb (Western Fluids, CAT#nanoBaume)
- NanoLC for column packing (we use an old Eksigent nanoLC system)
- Reprosil-Pur, Basic C18 material (Dr. Maisch, CAT#r119.b9.)
- Spinbar Micro Stir Bar (VWR, CAT#58948-377)
- Glass vials (Canadian Life Sceince, CAT#VT009M-1232)
- Screw tops for glass vials (Canadian Life Science, CAT#C397-09B)
- Fused silica frit kit (Next Advance, CAT#FRIT-KIT)
- Acetone (Sigma, CAT#650501)

<span id="solution-recipes"></span>

## Solution recipes

- nanoLC mobile phase A - 0.1% formic acid in water
- nanoLC mobile phase B - 0.1% formic acid in acetonitrile

<span id="protocol"></span>

## Protocol

1. Turn on the laser puller to allow it to heat up (allow for 10-minutes).
2. Trim a 150um ID capillary to a length of 60cm using a ceramic cutter provided with the FRIT-KIT.
3. Trim 200um ID capillaries to a length of 15cm.
4. Using the butane torch burn the coating off of the middle of the 60cm capillary to a length of approximately 5cm (see [**Note 1**](#note1)).
5. Use a KimWipe wetted with methanol to clean the coating off of the burned area.
6. Pull the capillary using the laser puller to form two nanospray tips. A typical program would be:
   1. Heat = 320, Vel = 40, Del = 200
   2. Heat = 310, Vel = 30, Del = 200
   3. Heat = 300, Vel = 25, Del = 200
   4. Heat = 290, Vel = 20, Del = 200
7. Prepare a frit mixture by mixing 30uL of Kasil-1624 and 10uL of formamide from the FRIT-KIT. Vortex to mix.
8. Using a ceramic capillary cutting tile, gentle 'shave' the nanospray tip by stroking at a 45 degree angle on the tile for a couple of passes.
9. Dip the shaved tip in the prepared frit mixture for a second.
10. Wipe the tip clean with a wet KimWipe.
11. Dip one end of the 200um ID capillaries in the frit mixture and wipe the end clean with a KimWipe.
12. Place the fritted capillaries on a room temperature heating block horizontally using a glass bottle to hold them secure. It is important that the block is not already hot!
13. Turn on the heating block to +90C and allow the frits to polymerize for 30-minutes.
14. Prepare the bead slurry by mixing 10mg of the Reprosil-Pur bead material with 1mL of acetone in a glass vial. Vortex to mix and sonicate for 5-minutes.
15. Rinse a fritted 200um ID capillary with acetone using the capillary packing bomb (I like to use a pressure of 100psi at all times).
16. Fill the 200um ID capillary with the prepared bead slurry using the capillary packing bomb.
17. While the 200um ID capillary is packing, shave the fritted 150um nanospray capillary using the cutting tile, as described above.
18. Attach the 150um capillary to the packing nanoLC system at a flow rate of 1uL/min at 60% acetonitrile with 0.1% formic acid. If the tip is not flowing, shave it some more to open it.
19. Once the 200um capillary is packed, gently and slowly release the pressure, and attach it in a reverse manner using the VICI union to the 150um capillary. The configuration here should be: nanoLC pump -> frit -> 200um ID capillary -> union -> 150um ID capillary -> fritted nanospray tip. In this way, the pump will push the beads into the 150um capillary. Gentle mechanical tapping of the union with a wrench can aid in flow.
20. Once a length approximately 25cm has been reached on the 150um capillary column, adjust the flow rate to achieve a pressure of at least 5,000 psi to finish packing.
21. Disconnect the column and attach it to the nanoLC system, or store in 50% methanol for later use.  

<hr style="height:6pt; visibility:hidden;" />

<span id="notes"></span>

## Notes

<span id="note1"></span>

**Note 1** - It is not necessary to completely burn off the coating with the torch. You just need to get it frayed to the point where it can be wiped off. Overheating the capillary with the torch will cause it to become brittle. Take care to rotate the capillary in your fingers while heating to avoid overheating the capillary.
