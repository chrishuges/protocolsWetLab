# Total proteome analysis by mass spectrometry <!-- omit in toc -->

This protocol was last updated - May 11, 2020 by Chris Hughes.

This document describes an end-to-end protocol for quantitative whole-proteome analysis by mass spectrometry. This protocol can be used as a general guideline as there are many different ways of doing many of these individual steps and still achieving success. The topics covered include how to perform harvest and lysis of cell line material, clean-up of proteins, tryptic digestion, TMT labeling, high pH C18 reversed phase fractionation, nanospray column preparation, MS data acquisition, and data analysis. The assumed starting material is cell-line derived, but is also appropriate for tissues (non-FFPE).

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [1. Cell line harvest](#1-cell-line-harvest)
  - [1.1 Reagents and materials](#11-reagents-and-materials)
  - [1.2 Solution recipes](#12-solution-recipes)
  - [1.3 Protocol](#13-protocol)
- [2. Cell pellet lysis](#2-cell-pellet-lysis)
  - [2.1 Reagents and materials](#21-reagents-and-materials)
  - [2.2 Solution recipes](#22-solution-recipes)
  - [2.3 Protocol](#23-protocol)
- [3. SP3 protein clean-up and digestion](#3-sp3-protein-clean-up-and-digestion)
  - [3.1 Reagents and materials](#31-reagents-and-materials)
  - [3.2 Solution recipes](#32-solution-recipes)
  - [3.3 Protocol](#33-protocol)
- [4. Tandem mass tag labeling](#4-tandem-mass-tag-labeling)
  - [4.1 Reagents and materials](#41-reagents-and-materials)
  - [4.2 Solution recipes](#42-solution-recipes)
  - [4.3 Protocol](#43-protocol)
- [5. HPLC peptide fractionation](#5-hplc-peptide-fractionation)
  - [5.1 Reagents and materials](#51-reagents-and-materials)
  - [5.2 Solution recipes](#52-solution-recipes)
  - [5.3 Protocol](#53-protocol)
- [6. Preparing a nanospray chromatography column](#6-preparing-a-nanospray-chromatography-column)
  - [6.1 Reagents and materials](#61-reagents-and-materials)
  - [6.2 Solution recipes](#62-solution-recipes)
  - [6.3 Protocol](#63-protocol)
- [7. Mass spectrometry analysis](#7-mass-spectrometry-analysis)
  - [7.1 Reagents and materials](#71-reagents-and-materials)
  - [7.2 Solution recipes](#72-solution-recipes)
  - [7.3 Protocol](#73-protocol)
- [8. Data processing](#8-data-processing)
  - [8.1 Software tools](#81-software-tools)
  - [8.2 Protocol](#82-protocol)
  - [8.3 Example shell script for data analysis](#83-example-shell-script-for-data-analysis)
- [Notes](#notes)

<hr style="height:6pt; visibility:hidden;" />

<span id="1-cell-line-harvest"></span>

## 1. Cell line harvest

This protocol assumes you have your cells growing in 15cm dishes. For other dish sizes, simply scale the reagents for your purpose. For all the solutions described below and throughout this protocol in general, you should do your best to use sterile glassware and reagents.

<span id="11-reagents-and-materials"></span>

### 1.1 Reagents and materials

- 15mL tubes (VWR, CAT#89093-186) - need 1 per sample
- 50mL tubes (VWR, CAT#89093-190) - need 3 in total
- Centrifuge with 15mL tube buckets (multiple vendors)
- TrypLE express (Thermo Fisher, CAT#12605028)
- DPBS, no calcium or magnesium (Thermo Fisher, CAT#14190144)
- Dry ice

<span id="12-solution-recipes"></span>

### 1.2 Solution recipes

- Cell culture medium (provided only as an example)
  - DMEM (500mL)
  - FBS (50mL)

<span id="13-protocol"></span>

### 1.3 Protocol

This protocol assumes you have your cells growing in 15cm dishes. For other dish sizes, simply scale the reagents for your purpose.

1. Label 1x15mL tube for each sample you plan to harvest.
2. Label a 50mL tube with 'TE', another with 'Media', and a last with 'PBS'.
3. To the 'TE' 50mL tube, add 8mL of TrypLE express per sample you plan to harvest.
4. To the 'PBS' 50mL tube, add 5mL of DPBS per sample you plan to harvest.
5. Remove the cell plate from the incubator and ipette the media the cells are growing in into the 50mL tube labeled 'Media'.
6. Add 8mL of TrypLE express to the plate and place back into the incubator (see [**Note 1**](#note1)).
7. Once the cells have started to detach, remove the plate from the incubator.
8. With 4mL of media from the 'Media' tube, rinse and collect the detached cells and transfer to the appropriate 15mL tube.
9. Centrifuge the tube with the cells for 3-minutes at 250g.
10. Dump the supernatant to waste (I use an old media bottle for this).
11. Add 5mL of DPBS from the 'PBS' tube to the tube with the cell pellet. There is no need to mix here.
12. Centrifuge the tube for 30-seconds at 250g.
13. Dump the supernatant to waste and spirate the remaining liquid to leave as little as possible.
14. Place the cell pellet on dry ice until frozen and keep at -80C until use.

<hr style="height:6pt; visibility:hidden;" />

<span id="2-cell-pellet-lysis"></span>

## 2. Cell pellet lysis

Two different options are described for lysis here. The first uses a nuclease to degrade nucleic acids, and the second uses mechanical disruption via a FastPrep instrument. Use whatever is appropriate for the equipment you have on hand. As the goal here is to measure proteins, make an effort to minimize potential keratin contamination (e.g. wear a lab coat and don't touch your tubes with un-gloved hands).

<span id="21-reagents-and-materials"></span>

### 2.1 Reagents and materials

- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- Benchtop centrifuge with holder for microcentrifuge tubes (multiple vendors)
- 1M HEPES pH 7.3 (Thermo Scientific, CAT#BP299-1)
- NP-40 (Sigma, CAT#NP40)
- Deoxycholate (DOC) (Sigma, CAT#D6750)
- 20% SDS (Thermo Scientific, CAT#BP1311)
- cOmplete protease inhibitor tablets, EDTA free (Sigma, CAT#11836170001)
- Dithiothreitol (Bio-Rad, CAT#1610611)
- Chloroacetamide (Sigma, CAT#C0267)
- Benzonase nuclease, 25U/uL (Sigma, CAT#70664-3)
- Clean water (Thermo Scientific, CAT#10977023)
- Thermomixer with 2mL tube block (Eppendorf)
- FastPrep 5G instrument (MP Biomedicals)
- Lysing matrix Y tubes (MP Biomedicals, CAT#116960100)

<span id="22-solution-recipes"></span>

### 2.2 Solution recipes

- 0.2M of dithiothreitol (DTT) - 15mg in 500uL of 1M HEPES, pH 7.3, prepare fresh and keep on ice
- 0.4M of chloroacetamide (CAA) - 18mg in 500uL of 1M HEPES, pH 7.3, prepare fresh and keep on ice
- 10% (v/v) NP-40 - 1mL in 9mL of water
- 10% (w/v) DOC - 1g in 10mL of water
- 10X cOmplete protease inhibitor stock - 1 tablet in 1mL of water
- Lysis buffer A (need 200uL per sample, recipe for 1mL)(see [**Note 2**](#note2))
  - 100mM HEPES pH 7.3 (100uL of 1M stock)
  - 0.5% (v/v) NP-40 (50uL of 10% stock)
  - 0.5% (v/v) DOC (50uL of 10% stock)
  - 0.5X cOmplete protease inhibitor (50uL of 10X stock)
  - 100U/mL TURBO DNase (4uL of 20U/uL stock)
  - water to 1mL (746uL of clean water)
- Lysis buffer B (need 200uL per sample, recipe for 1mL)
  - 100mM HEPES pH 7.3 (100uL of 1M stock)
  - 1% (v/v) SDS (50uL of 20% stock)
  - 10mM DTT (50uL of 0.2M stock)
  - water to 1mL (800uL of clean water)

<span id="23-protocol"></span>

### 2.3 Protocol

1. Remove cell pellet from the -80C freezer and allow to slowly thaw at room temperature (+21C).
2. If there is any residual culture media visible on top of the pellet as it thaws, try to remove it with a 200uL pipette.
3. Once the pellet has almost thawed entirely, but still remains partially frozen, pipette 200uL of initial lysis buffer into the tube and pipette mix. Transfer the cell mixture to a fresh 2mL tube.
4. Incubate the cell suspension at +37C for 15-minutes in a ThermoMixer with shaking at 1,000rpm.
5. After the incubation, add 200uL of secondary lysis buffer and pipette mix.
6. Incubate the lysate at +60C for 30-minutes in a ThermoMixer with shaking at 1,000rpm.
7. Remove the tube from the ThermoMixer and allow to cool for a few minutes to room temperature.
8. Add 40uL of 0.4M CAA stock and pipette mix. Incubate at room temperature in the dark for 30-minutes.
9. Add 20uL of 0.2M DTT stock and pipette mix. Incubate at room temperature for 15-minutes.
10. The cell pellets can be frozen at this point at -80C indefinitely.

<hr style="height:6pt; visibility:hidden;" />

<span id="3-sp3-protein-clean-up-and-digestion"></span>

## 3. SP3 protein clean-up and digestion

<span id="31-reagents-and-materials"></span>

### 3.1 Reagents and materials

- 1M HEPES pH 7.3 (Thermo Scientific, CAT#BP299)
- Ethanol, absolute (whatever vendor sells this to your lab)
- SP3 beads (Thermo Scientific, CAT#65152105050250, CAT#45152105050250) (see [**Note 3**](#note3))
- Trypsin/rLysC mix (Promega, CAT#V5073)
- 1.5mL or 2.0mL Safe-Lock tubes (Fisher Scientific, CAT#05-402-25 or CAT#05-402-7)
- Thermomixer capable of holding 1.5mL or 2.0mL tubes (Eppendorf)
- Benchtop centrifuge (capable of holding 1.5mL or 2mL microfuge tubes)
- Magnetic rack for 1.5mL or 2.0mL tubes (I like this rack: Promega, CAT#Z5342)
- Sonicating water bath (optional)
- Clean water (Thermo Fisher, CAT#10977023)

<span id="32-solution-recipes"></span>

### 3.2 Solution recipes

- 100mM HEPES, pH 7.3 (100uL of 1M stock combined with 900uL of water)
- 80% (v/v) ethanol (prepare fresh)

<span id="33-protocol"></span>

### 3.3 Protocol

For all stages of this protocol, discussion of various aspects related to performance or compatibility can be found in PMID: 30464214.

1. Prepare your sample by bringing 100ug of protein from the lysate to a total volume of 190uL using 100mM HEPES pH 7.3.
2. Prepare the SP3 beads stock (see [**Note 4**](#note4)):
   1. Vortex the bead stock to re-suspend the material.
   2. Take 500uL of each of the bead stocks and combine in a fresh 2mL tube.
   3. Place on a magnetic rack and wait for beads to settle. Discard the supernatant.
   4. Reconstitute the beads in 1mL of water with pipetting and place back on the magnetic rack. After the beads settle, discard the supernatant.
   5. Repeat the above rinse one additional time for a total of 2 rinses.
   6. Reconstitute the beads in 500uL of water. The bead stock can be stored at +4C indefinitely.
3. Add 10uL of SP3 beads to the sample and pipette mix.
4. Add 200uL of ethanol to the sample and gently shake the tube with your hand to mix the phases. Do not vortex.
5. Place in a shaking incubator at room temperature for 5-minutes.
6. Centrifuge the tube at 50g for 30-seconds to bring any liquid down from the top of the tube.
7. Place the tube on a magnetic rack and wait for the beads to settle. Discard the supernatant.
8. Remove the tube from the rack and reconstitute the beads in 800uL of 80% ethanol. Gently rinse the beads by pipetting.
9. Place the tube on a magnetic rack and wait for the beads to settle. Discard the supernatant.
10. Repeat **Steps 8 - 10** one additional time for a total of 2 rinses.
11. Place the tube back on the magnetic rack an wait for the beads to settle.
12. Discard the supernatant taking care to remove any residual ethanol remaining. It is not necessary to air dry the tubes.
13. For digestion:
    1. Prepare a digestion solution by combining 2ug of trypsin in 100uL of 100mM HEPES, pH 7.3 (see [**Note 5**](#note5)).
    2. Add 100uL of the digestion solution to the sample and pipette mix (see [**Note 6**](#note6)).
    3. Incubate at +37C in a shaking incubator or ThermoMixer overnight (around 14-hours).
    4. After digestion, gently shake the tube to reconstitute the beads.
    5. Centrifuge the tube at 20,000g for 2-minutes.
    6. Place on the magnetic rack and wait for the beads to settle.
    7. Transfer the supernatant to a fresh 1.5mL tube.
    8. The peptide sample can be stored at -80C indefinitely.

<hr style="height:6pt; visibility:hidden;" />

<span id="4-tandem-mass-tag-labeling"></span>

## 4. Tandem mass tag labeling

<span id="41-reagents-and-materials"></span>

### 4.1 Reagents and materials

- TMT 11-plex kit, 5mg per label (Thermo Scientific, CAT#A34808)
- Acetonitrile, HPLC grade (Thermo Scientific, CAT#51101)
- Glycine (Thermo Scientific, CAT#15527013)
- RNA clean water (Thermo Fisher, CAT#10977023)
- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- Benchtop centrifuge (capable of holding 1.5mL or 2mL microfuge tubes)

<span id="42-solution-recipes"></span>

### 4.2 Solution recipes

- 1M glycine (750mg in 10mL of water)

<span id="43-protocol"></span>

### 4.3 Protocol

1. Prepare the TMT label stocks:
   1. Spin the TMT label tubes at 12,000g for 2-minutes.
   2. Add 500uL of acetonitrile to each label and vortex to dissolve the powder (final concentration of label is 10ug/uL)(see [**Note 7**](#note7)).
2. To a protein digest prepared from 100ug of protein previously processed with SP3, add 20uL of TMT label (2:1 ratio) and pipette mix followed by a brief vortex (see [**Note 8**](#note8)).
3. Incubate the tubes at room temperature (+21C) for 30-minutes.
4. After incubation, add an addition 20uL of TMT label to the tubes and vortex briefly.
5. Incubate the tubes at room temperature for 30-minutes.
6. Add 20uL of 1M glycine to the tubes and vortex.
7. The samples are now labeled and my be stored at -80C indefinitely.

<hr style="height:6pt; visibility:hidden;" />

<span id="5-hplc-fractionation"></span>

## 5. HPLC peptide fractionation

This portion of the protocol includes pre-concentration of the sample, peptide clean-up, re-concentration, and HPLC fractionation.

<span id="51-reagents-and-materials"></span>

### 5.1 Reagents and materials

- Lyophilizer or SpeedVac centrifuge (multiple vendors)
- C18 TopTips (CAT#TT3C18, Glygen Corp.)
- Acetonitrile, HPLC grade (CAT#51101, Thermo Scientific)
- Water, HPLC grade (CAT#51140, Thermo Scientific)
- Trifluoroacetic acid, HPLC grade (CAT#85183, Thermo Scientific)
- Formic acid, HPLC grade (CAT#85178, Thermo Scientific)
- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- HPLC system for fractionation (we use an Agilent 1100 system)
- HPLC column heater (HotSleeve+, Analytical Sales and Services, CAT#HSI-25L)
- 96-well collection plates for HPLC fractionation (Thermo Scientific, CAT#14-223-345) **check this plate**...it is important to use the right one otherwise the fraction collector will overheat
- HPLC fractionation column (Phenomenex, CAT#00F-4496-E0)
- HPLC guard column (Phenomenex, CAT#AF0-5727)
- Ammonium bicabonate (Sigma, CAT#A6141)
- Dimethylsulfoxide (Sigma, CAT#D8418)

<span id="52-solution-recipes"></span>

### 5.2 Solution recipes

- Buffer A - 0.1% trifluoroacetic acid (TFA) in acetonitrile
- Buffer B - 0.1% TFA in water
- Rinse Buffer - 0.1% formic acid in water
- Elution Buffer - 0.1% formic acid in 60% acetonitrile
- HPLC mobile phase A - 20mM ammonium bicarbonate - 790mg in 500mL HPLC grade water
- HPLC mobile phase B - 100% acetonitrile
- 1% formic acid with 1% DMSO - 10uL of formic acid, 10uL of DMSO, and 80uL of water

<span id="53-protocol"></span>

### 5.3 Protocol

First, labeled TMT peptide mixtures need to be concentrated to reduce the levels of solvent in the mixture. This can be performed as separate tubes, or as one combined multiplex. This protocol is based on doing each labeled sample separately. Prior to HPLC fractionation, it is a good idea to verify the functionality of your system using an appropriate standard, such as a BSA digest.

1. Poke an approximately 1cm diameter hole in the lid of each sample tube and transfer the tubes to the -80C freezer.
2. Turn on the lyophilizer and allow the vaccuum chamber to chill.
3. Add the frozen samples to the lyophilizer and turn on the vaccuum. Leave for about 4 to 6-hours.
4. Remove the sample tubes from the lyophilizer (there should be only white material remaining), and reconstitute the first sample tube in 600uL of water.
5. Transfer the 600uL to the next sample tube and reconstitute. Perform this same task until all samples are reconstituted in the same 600uL. Set the sample tube aside.
6. Using a pipette, add 600uL of Buffer A to a TopTip and elute the added liquid to the waste at a flow rate of 1 drop per second (see [**Note 9**](#note9)).
7. Repeat the previous step one additional time for a total of 2 rinses.
8. Add 600uL of Buffer B to the TopTip and elute to waste as above.
9. Repeat the previous step one additional time for a total of 2 rinses.
10. Add the sample to the TopTip and elute to waste as above.
11. Rinse the loaded TopTip with 600uL of Rinse Buffer.
12. Repeat the previous step two additional times for a total of 3 rinses.
13. Elute the peptides with 600uL of the Elution Buffer into a fresh 1.5mL tube.
14. Repeat the previous step one additional time for a total of 2 elutions.
15. Poke an approximately 1cm diameter hole in the lid of the elution tube and transfer it to the -80C freezer.
16. Turn on the lyophilizer and allow the vaccuum chamber to chill.
17. Add the frozen samples to the lyophilizer and turn on the vaccuum. Leave overnight, or for about 12-hours.
18. Remove the sample tube from the lyophilizer (there should be only white material remaining), and reconstitute in 350uL of water.
19. Turn on the HPLC system:
    1. Open the black knob on the front (turn to the left) and set the flow rate to 5mL/min of 100% B. Flush for 3-minutes.
    2. Change the flow rate to 100% A and flush for an additional 3-minutes.
    3. Set the column heater to +50C and wait for it to heat up.
    4. Set the flow rate to 1mL/min at 100% B and close the black knob (turn to the right). Allow the system to stabilize (approximately 5-minutes).
    5. Set the composition to 50% B and allow the system to stabilize (approximately 5-minutes).
    6. Set the composition to 5% B and allow the system to stabilize (approximately 5-minutes). The column pressure should be around 250bar in these conditions.
20. The method conditions are going to depend entirely on your system, but with this setup, the gradient used is:
    1. Time = 0, %B = 5, Flow = 1mL/min
    2. Time = 5, %B = 5, Flow = 1mL/min
    3. Time = 7, %B = 8, Flow = 1mL/min
    4. Time = 20, %B = 16, Flow = 1mL/min
    5. Time = 45, %B = 40, Flow = 1mL/min
    6. Time = 46, %B = 80, Flow = 1mL/min
    7. Time = 50, %B = 80, Flow = 1mL/min
    8. Time = 60, %B = 5, Flow = 1mL/min
    9. A DAD is used to measure absorbance at 280, 254, and 214nm.
    10. Fractions are collected using an embedded module from 8 - 45 minutes, for a total of 48-fractions.
21. Centrifuge your lyophilized sample at 20,000g for 2-minutes.
22. Recover 325uL of the supernatant to a glass HPLC vial that is suitable for your system.
23. Run a fractionation, injecting 300uL of your sample (our system has a 900uL injection loop).
24. Transfer the fractions to 2mL tubes where they are concatenated to a final set of 36 using a scheme:
    1. Fraction 1 = A1 + D1
    2. Fraction 2 = A2 + D2
    3. Fraction 12 = A12 + D12
    4. Fraction 13 = B1
    5. Fraction 14 = B2
    6. Fraction 36 = C12
25. Poke an approximately 1cm diameter hole in the lid of the fraction tubes and transfer them to the -80C freezer.
26. Turn on the lyophilizer and allow the vaccuum chamber to chill.
27. Add the frozen samples to the lyophilizer and turn on the vaccuum. Leave overnight, or for about 12-hours.
28. Once the fractions have reached dryness, add 20uL of the 1% formic acid, 1% DMSO solution. Do not try to pipette mix.
29. Vortex the tubes for 10-seconds and then centrifuge for 2-minutes at 12,000g.
30. Repeat the previous step one additional time.
31. Samples can be frozen at this stage at -80C indefinitely.

<hr style="height:6pt; visibility:hidden;" />

<span id="6-preparing-a-nanospray-chromatography-column"></span>

## 6. Preparing a nanospray chromatography column

<span id="61-reagents-and-materials"></span>

### 6.1 Reagents and materials

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

<span id="62-solution-recipes"></span>

### 6.2 Solution recipes

- nanoLC mobile phase A - 0.1% formic acid in water
- nanoLC mobile phase B - 0.1% formic acid in acetonitrile

<span id="63-protocol"></span>

### 6.3 Protocol

1. Turn on the laser puller to allow it to heat up (allow for 10-minutes).
2. Trim a 150um ID capillary to a length of 60cm using a ceramic cutter provided with the FRIT-KIT.
3. Trim 200um ID capillaries to a length of 15cm.
4. Using the butane torch burn the coating off of the middle of the 60cm capillary to a length of approximately 5cm (see [**Note 10**](#note10)).
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

<span id="7-mass-spectrometry-analysis"></span>

## 7. Mass spectrometry analysis

<span id="71-reagents-and-materials"></span>

### 7.1 Reagents and materials

- Acetonitrile, HPLC grade (Thermo Scientific, CAT#51101)
- Water, HPLC grade (Thermo Scientific, CAT#51140)
- Formic acid, HPLC grade (CAT#85178, Thermo Scientific)
- 96-well autosampler plates for nanoLC (Fisher Scientific, CAT#14-222-326)
- 96-well mats for autosampler plates (Fisher Scientific, CAT#14-222-024)
- MicroTee Assembly (IDEX-HS, CAT#P-775)
- MicroCross Assembly (IDEX-HS, CAT#P-777)
- MicroTight Sleeve Green (IDEX-HS, CAT#F-185X)
- NanoLC column oven (AgileSleeve+, Analytical Sales and Services, CAT#ASI1532H)
- NanoLC system (we use an Easy nLC1000 from Thermo Scientific)
- Mass spectrometer ion source (we use a modified version of the UWPR ion source).
- Mass spectrometer (we use an Orbitrap Fusion Lumos)

<span id="72-reagents-and-materials"></span>

### 7.2 Solution recipes

- nanoLC mobile phase A - 0.1% formic acid in water
- nanoLC mobile phase B - 0.1% formic acid in 80% acetonitrile

<span id="73-reagents-and-materials"></span>

### 7.3 Protocol

We like to use a direct on-column setup on our nanoLC system prior to the MS. Our Easy nLC is modified such as to have a 10uL sample loop, and the factory column-out capillary (20um ID x 50cm length) is replaced with a 50um ID x 20cm version. We use a liquid junction prepared as part of the modified UWPR source. For peptide separation we use a 25cm column packed with 1.9um C18 beads as described above. Ensure your system is operating correctly using your standard of choice.

1. Transfer your fractionated peptide samples to a 96-well autosampler plate and seal with the appropriate mat.
2. In the method editor software for the LC in a standard 60-minute run, the parameters used are as follows (this will depend on your column configuration!):
   1. Sample loading - pressure max of 400 bar for 6uL.
   2. Pre-column equilibration - pressure max of 400 bar for 3uL.
   3. Gradient (see [**Note 11**](#note11)):
      1. Time = 0, Duration = 0, %B = 3, Flow = 800nL/min
      2. Time = 2, Duration = 2, %B = 7, Flow = 800nL/min
      3. Time = 43, Duration = 41, %B = 35, Flow = 800nL/min
      4. Time = 43.25, Duration = 0.25, %B = 80, Flow = 800nL/min
      5. Time = 46.25, Duration = 3, %B = 80, Flow = 800nL/min
      6. Time = 46.5, Duration = 0.25, %B = 3, Flow = 800nL/min
      7. Time = 52, Duration = 5.5,  %B = 3, Flow = 800nL/min
   4. MS data acquisition (for a TMT multiplex analysis with MS2 scanning only, depending on your system):
      1. Global
         1. Spray voltage = 2400
         2. S-lens = 60
         3. Transfer tube temperature = +325C
         4. Default charge state = 2
      2. MS1
         1. 400 - 1200 scan range
         2. AGC target = 4e5
         3. Max injection time = 86ms
         4. Resolution  = 50K
      3. Dependent scan selection
         1. Monoisotopic precursor selection = Peptide
         2. Charge state = 2 - 4, include undetermined charge states
         3. Dynamic exlusion = 1 time, 15-seconds, 10ppm tolerance, exclude isotopes, dependent scan on single charge state disabled.
      4. MS2
         1. Quadrupole isolation = TRUE
         2. Isolation window = 2m/z
         3. HCD activation = 40% energy
         4. Auto: m/z Normal scan range
         5. Resolution = 50K
         6. Fixed first mass = 110m/z
         7. AGC target = 1.2e5
         8. Max injection time = 86ms
         9. Inject ions for all available time = FALSE
      5. Overall max allowable cycle time = 2-seconds
   5. MS data acquisition (for a TMT multiplex analysis with SPS-MS3 scanning, depending on your system):
      1. Global
         1. Spray voltage = 2400
         2. S-lens = 60
         3. Transfer tube temperature = +325C
         4. Default charge state = 2
      2. MS1
         1. 400 - 1200 scan range
         2. AGC target = 4e5
         3. Max injection time = 86ms
         4. Resolution  = 50K
      3. Dependent scan selection
         1. Monoisotopic precursor selection = Peptide
         2. Charge state = 2 - 4, include undetermined charge states
         3. Dynamic exlusion = 1 time, 15-seconds, 10ppm tolerance, exclude isotopes, dependent scan on single charge state disabled.
      4. MS2
         1. Quadrupole isolation = TRUE
         2. Isolation window = 2m/z
         3. CID activation = 30% energy
         4. Scan rate = Rapid
         5. AGC target = 1e4
         6. Max injection time = 45ms
         7. Inject ions for all available time = FALSE
      5. MS3 scan selection
         1. Precursor selection range = 400 - 1200m/z
         2. Precursor ion exclusion = 20ppm high, 5ppm low
         3. Isobaric tag loss exclusion = TMT
      6. MS3
         1. MS2 isolation window = 2
         2. MS3 isolation window = 2
         3. Number of SPS ions = 10
         4. HCD activation = 50% energy
         5. Resolution = 50K
         6. Mass range = 110 - 750m/z
         7. AGC target = 1.2e5
         8. Max injection time = 86ms
         9. Inject ions for all available time = FALSE
      7. Overall max allowable cycle time = 2-seconds
3. Inject 4uL of each of your fractions for analysis using one of the above described approaches.

<hr style="height:6pt; visibility:hidden;" />

<span id="8-data-processing"></span>

## 8. Data processing

Data processing can take many shapes depending on what you have done or what you have available, or what type of computation tools you are comfortable with. The pipeline detailed below is the one that I use and find the give accurate and reproducible data. It is also free. The shell script referenced below will execute all of these processed with a single command. This protocol assumes you are using the command line on a linux server.

<span id="81-software-tools"></span>

### 8.1 Software tools

- RawTools [(link)](https://github.com/kevinkovalchik/RawTools)
- SearchGUI [(link)](https://github.com/compomics/searchgui)
- PeptideShaker [(link)](https://github.com/compomics/peptide-shaker)

<span id="82-protocol"></span>

### 8.2 Protocol

Download RawTools, SearchGUI, and PeptideShaker to a directory on the server and remember the location, (you can use `wget` to download those programs to the linux server).

```
$ mkdir software
$ cd software
$ wget https://github.com/kevinkovalchik/RawTools/releases/download/2.0.2/RawTools-2.0.2.zip
$ wget http://genesis.ugent.be/maven2/eu/isas/searchgui/SearchGUI/3.3.16/SearchGUI-3.3.16-mac_and_linux.tar.gz
$ wget http://genesis.ugent.be/maven2/eu/isas/peptideshaker/PeptideShaker/1.16.42/PeptideShaker-1.16.42.zip
```

Extract the files.

```
$ unzip RawTools-2.0.2.zip
$ gunzip SearchGUI-3.3.16-mac_and_linux.tar.gz
$ tar -xvf SearchGUI-3.3.16-mac_and_linux.tar
$ unzip PeptideShaker-1.16.42.zip
```

Create the shell script file.

```
$ touch tmt-data-processing.sh
$ chmod +x tmt-data-processing.sh
```

Copy the text in the text file called 'ms2TmtDataProcessing.txt in this protocols directory and paste it into your created shell script file.

```
$ vim tmt-data-processing.sh
Press 'i' to make edits to the file. Paste the text. Press 'Esc'. Type ':wq' and hit Enter.
```

Open the shell script again and edit the paths to suite your system.

```
$ pwd
Copy the output of that command.
$ vim tmt-data-processing.sh
The specific variables that need to be changed are: sample_tag, desired_base_location, and data_storage_location.
You may also want to edit the parameters for different tools if you have not done an MS2 only analysis, or you are not using a human sample.
```

Run the script and output a log file called data-processing.txt.

```
$ ./tmt-data-processing.sh |& tee data-processing.txt
```

### 8.3 Example shell script for data analysis

This script is purely for example purposes and is designed to work in my own environment. You will need to modify paths to data and software tools for this to work on your own system.

```
#! /bin/bash

##############################################################
#this first part calls the help if the user triggers it
usage(){
printf "
This script will process proteomic data to generate PeptideShaker Reports.\n
The sample tag and desired base location parameters should be edited before running the script.\n
All results will be written to the folder created based on the sample tag and base location.\n\n"
}

if [[ $1 == -h ]] || [[ $1 == --help ]];
then
  usage
  exit
fi


##############################################################
##############################################################
#users must edit the below variables

#this is the text that will identify your files
sample_tag="some text that will identify your raw file names"

#this is the desired location for the output of the data processing process
desired_base_location="/path/to/where/you/want/the/processed/data/to/be/stored/"

#this is the base location where your raw data is stored
data_storage_location="/path/to/where/the/raw/data/is/stored/"

#this is text that will be appended to your output folder that is created for this analysis
folder_adapter="ms-analysis_"

#users do not need to edit the statement below
folder_to_create="$desired_base_location$folder_adapter$sample_tag"



##############################################################
##############################################################
#locations of software tools
crap_database="/path/to/contaminants/database.fasta"
rawtools_location="/path/to/RawTools.exe"
searchGUI_location="/path/to/SearchGUI-X.X.XX.jar"
peptideshaker_location="/path/to/PeptideShaker-X.XX.XX.jar"



##############################################################
##############################################################
####first we need to make the location for the data storage
making_a_dir="mkdir $folder_to_create"

#check if directory does not exist and create it if it doesn't
if [ ! -d "$folder_to_create" ];
then
  printf "Creating the processing directory.\n"
  eval $making_a_dir
fi

#move into the processing directory
eval "cd $folder_to_create"
printf "\nData processing proceeding in the directory: $PWD\n\n"



##############################################################
##############################################################
####set up the database to use
uniprot_version=$( date +%b%Y )
database_extension="_concatenated_target_decoy"

#check if the database exists, and if not, get it
if [ ! -f "./uniprot-human-crap_$uniprot_version$database_extension.fasta" ]; then
    printf "Database not found!\n\n"
    eval "wget ftp://ftp.uniprot.org/pub/databases/uniprot/current_release/knowledgebase/reference_proteomes/Eukaryota/UP000005640_9606.fasta.gz"
    eval "gunzip UP000005640_9606.fasta.gz"
    eval "mv UP000005640_9606.fasta ./uniprot-human_$uniprot_version.fasta"
    eval "cat ./uniprot-human_$uniprot_version.fasta $crap_database > ./uniprot-human-crap_$uniprot_version.fasta"
    eval "java -cp $searchGUI_location eu.isas.searchgui.cmd.FastaCLI -in ./uniprot-human-crap_$uniprot_version.fasta -decoy"
    printf "Database created and ready to use.\n\n"
else
  printf "\nDatabase file exists: ./uniprot-human-crap_$uniprot_version$database_extension.fasta\n\n"
fi



##############################################################
##############################################################
####set up the parameters file
fixed_modifications='"Carbamidomethylation of C, TMT 11-plex of peptide N-term"'
variable_modifications='"Oxidation of M, TMT 11-plex of K"'

#####call the parameters file creation
calling_parameters='java -cp "$searchGUI_location" eu.isas.searchgui.cmd.IdentificationParametersCLI -out ./OT-MS1_HCD-OT-MS2_human-trypsin_stdMods-TMT_"$uniprot_version".par -db ./uniprot-human-crap_"$uniprot_version""$database_extension".fasta -prec_tol 20 -frag_tol 0.05 -db_pi ./uniprot-human-crap_"$uniprot_version""$database_extension".fasta -fixed_mods "$fixed_modifications" -variable_mods "$variable_modifications"'

####call the command
if [ ! -f "./OT-MS1_HCD-OT-MS2_human-trypsin_stdMods-TMT_$uniprot_version.par" ]; then
  printf "\nParameters file does not exist. Creating it.\n\n"
  eval "$calling_parameters"
else
  printf "Parameters file exists: OT-MS1_HCD-OT-MS2_human-trypsin_stdMods-TMT_$uniprot_version.par.\n\n"
fi



##############################################################
##############################################################
####run rawtools to get MGF files
##first find the raw files you want to process
file_list=()
  while IFS= read -d $'\0' -r file ; do
    file_list=("${file_list[@]}" "$file")
  done < <(find $data_storage_location -name "*$sample_tag*" -print0 | sort -z)

###now execute rawtools on each of these
for i in "${file_list[@]}"; do
  sample_id=$(basename "$i" ".raw")
  if [ -f "$sample_id.raw.mgf" ]; then
    printf "MGF output for $sample_id already exists, skipping file.\n\n"
  else
    rawtools_execution="mono $rawtools_location -f $i -quxmR -o $PWD -r TMT11"
    eval $rawtools_execution
  fi
done


##############################################################
##############################################################
####run the searchGUI analysis
file_list=()
  while IFS= read -d $'\0' -r file ; do
    file_list=("${file_list[@]}" "$file")
  done < <(find $PWD -name "*.mgf" -print0 | sort -z)

###now execute on each of these
for i in "${file_list[@]}"; do
  if [ -f "${i::-4}_searchgui_out.zip" ]; then
    sample_id=$(basename "$i" ".zip")
    printf "Search output for $sample_id already exists, skipping file.\n\n"
  else
    searchgui_execution="java -Xmx120g -cp $searchGUI_location eu.isas.searchgui.cmd.SearchCLI -spectrum_files $i -output_folder $PWD -id_params ./OT-MS1_HCD-OT-MS2_human-trypsin_stdMods-TMT_$uniprot_version.par -output_option 1 -xtandem 1"
    eval $searchgui_execution
  fi
done


##############################################################
##############################################################
####write the reports
file_list=()
  while IFS= read -d $'\0' -r file ; do
    file_list=("${file_list[@]}" "$file")
  done < <(find $PWD -name "*.zip" -print0 | sort -z)

###now execute on each of these
for i in "${file_list[@]}"; do
  sample_id=$(basename "$i" ".zip")
  while ! [ -f "${PWD}/n_${sample_id}_1_Default_PSM_Report.txt" ]; do
    printf "\nNo peptide shaker reports output exists for $sample_id, so it will be created.\n"
    #peptide shaker execution
    peptideshaker_execution="java -Xmx120g -cp $peptideshaker_location eu.isas.peptideshaker.cmd.PeptideShakerCLI -experiment n -sample $sample_id -replicate 1 -identification_files $i -spectrum_files $PWD -id_params ./OT-MS1_HCD-OT-MS2_human-trypsin_stdMods-TMT_$uniprot_version.par -out $i.out.cpsx"
    eval $peptideshaker_execution
    #reports output
    reports_execution="java -Xmx120g -cp $peptideshaker_location eu.isas.peptideshaker.cmd.ReportCLI -in $i.out.cpsx -out_reports $PWD -reports 0,3"
    eval $reports_execution
  done
  printf "\nFinished all exporting reports for $sample_id.\n\n"
done

####final output
eval "rm *.html"
eval "scp /path/to/where/this/script/is/stored/data-processing.txt $PWD"
printf "\n\nFinished processing a total of ${#file_list[@]} files!\n\n"
```

<hr style="height:6pt; visibility:hidden;" />

<span id="notes"></span>

## Notes

<span id="note1"></span>

**Note 1** - Depending on your cell line, the time you leave it in here will vary. For example, for HEK293 cells I will only leave it for 1 - 2 minutes, but for U2OS I would leave it for longer.

<span id="note2"></span>

**Note 2** - Scale the amount of lysis solution here depending on how big your cell pellets are. Generally, you want the amount of lysis solution you add to be 2X the volume your pellet occupies.

<span id="note3"></span>

**Note 3** - Other beads can be substituted here, such as BangsLabs Magnefy beads (CAT#MFY0001), or other carboxylate modified particles. Other companies, such as MagReSyn also offer HILIC beads which are also compatible.

<span id="note4"></span>

**Note 4** - The bead stock from the vendor is 50mg/mL. We recommend using the beads at a 10:1 (ug of beads : ug of protein) ratio. This is far in excess of what is necessary, but will improve rinsing and elution efficiency by reducing the amount of 'clumping' that happens during binding.

<span id="note5"></span>

**Note 5** - I generally aim to have a trypsin:protein, ug:ug ratio of around 1:100, depending on the volume. For a larger volume I would likely scale this down to a 1:25 ratio. But these are personal preferences and digestion should be efficient at the values you would typically use in your lab.

<span id="note6"></span>

**Note 6** - The beads may need to be sonicated for 30-seconds in a water bath to help disaggregate them. If you noticed a large amount of clumping of the beads during the binding phase, this can be beneficial for ensuring an efficienct digestion.

<span id="note7"></span>

**Note 7** - For short or long term storage of the reconstituted TMT labels, you should close the lid and wrap it in parafilm to that no air will enter the tube. The tubes should then be stored at -80C. Tubes stored in this format can be freeze-thawed numerous times without a decrease in label performance. The labels can also be aliquoted and stored in the same manner if desired.

<span id="note8"></span>

**Note 8** - Pay attention to your labeling layout to avoid interference between channels. For example, for a 9 sample experiment where you have 3 conditions, each in triplicate, lay your samples out in the format:

Label | Sample
---------|----------
 126 | sampleA replicate1
 127N | sampleB replicate1
 127C | sampleA replicate2
 128N | sampleB replicate2
 128C | sampleA replicate3
 129N | sampleB replicate3
 129C | empty
 130N | empty
 130C | sampleC replicate1
 131N | sampleC replicate2
 131C | sampleC replicate3

<span id="note9"></span>

**Note 9** - When a TopTip is first used, there will generally be some beads stuck to the side of the upper TopTip walls. Try to rinse the beads on the upper TopTip wall to join the rest of the bead bed.

<span id="note10"></span>

**Note 10** - It is not necessary to completely burn off the coating with the torch. Overheating the capillary with the torch will cause it to become brittle. Take care to rotate the capillary in your fingers while heating to avoid overheating the capillary.

<span id="note11"></span>

**Note 11** - The flow rate during equilibration and loading should be around 1.2uL/min when using column heating at +50C. The method is 52-minutes long as generally the injection and equilibration steps take around 8-minutes to complete, so the method rounds out at 60-minutes total time. The backpressure at 800nL/min should be around 225bar when using column heating at +50C. I usually aim to inject 4uL of each fraction here based on the processing amounts above. Peak widths should be around 6 - 9 seconds at 10% peak height with this setup.
