# Whole transcriptome, polysome, proteome, and purification analysis <!-- omit in toc -->

This document describes an end-to-end protocol for performing global transcriptome, proteome, and polysome analysis, along with RNA and protein-IP for a target of interest, all from a single cell lysate. 

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [1. Cell culture and harvest](#1-cell-culture-and-harvest)
  - [1.1 Reagents and materials](#11-reagents-and-materials)
  - [1.2 Solution recipes](#12-solution-recipes)
  - [1.3 Protocol](#13-protocol)
- [2. Sucrose gradient preparation](#2-sucrose-gradient-preparation)
  - [2.1 Reagents and materials](#21-reagents-and-materials)
  - [2.2 Solution recipes](#22-solution-recipes)
  - [2.3 Protocol](#23-protocol)
- [3. RNA and Protein Sample Preparation](#1-rna-and-protein-sample-preparation)
  - [3.1 Reagents and materials](#11-reagents-and-materials)
  - [3.2 Solution recipes](#12-solution-recipes)
  - [3.3 Protocol](#13-protocol)
- [4. Sucrose gradient fractionation](#4-sucrose-gradient-fractionation)
  - [4.1 Reagents and materials](#41-reagents-and-materials)
  - [4.2 Solution recipes](#42-solution-recipes)
  - [4.3 Protocol](#43-protocol)

<hr style="height:6pt; visibility:hidden;" />

<span id="1-cell-culture-and-harvest"></span>

## 1. Cell culture and harvest

Use whatever cell culture methods you are compfortable with here. This stage of the protocol is only given as an example of a process that is validated to work and is by no means the only way to achieve a successful result in this section.

<span id="11-reagents-and-materials"></span>

### 1.1 Reagents and materials

- 15mL tubes (VWR, CAT#89093-186)
- 50mL tubes (VWR, CAT#89093-190)
- Centrifuge with 15mL tube buckets (multiple vendors)
- TrypLE express (Thermo Fisher, CAT#12605028)
- DPBS, no calcium or magnesium (Thermo Fisher, CAT#14190144)
- Cycloheximide (Sigma, CAT#C7698)
- Dry ice

<span id="12-solution-recipes"></span>

### 1.2 Solution recipes

- Cell culture medium (provided only as an example)
  - DMEM (500mL)
  - FBS (50mL)
- 100mg/mL cycloheximide - 50mg in 500uL of DMSO

<span id="13-protocol"></span>

### 1.3 Protocol

This protocol assumes you have your cells growing in 15cm dishes. For other dish sizes, simply scale the reagents for your purpose. Generally, I will plate cells at a confluency of around 70% at 24h before I plan to harvest. This will ensure the majority of the cells on the dish are growing and actively translating. You do not want an over-confluent dish.

1. Label 1x15mL tube for each sample you plan to harvest.
2. Label a 50mL tube with 'TE' and another with 'Media'.
3. To the 'TE' 50mL tube, add 7mL of TrypLE express per sample you plan to harvest.
4. Remove the cell plate from the incubator and pipette 20uL of cycloheximide into the media in the dish (or a volume equivalent to what is present in the dish already, e.g. 15mL of media, add 15uL of cycloheximide stock).
5. Place the plate back in the incubator and leave it for 10-minutes.
6. Remove the cycloheximide treated plate from the incubator and remove the culture medium to the 50mL tube labeled 'Media' (any excess beyond 50mL can go to waste).
7. Add 6.5mL of TrypLE express to the plate and swirl the coat the bottom of the dish.
8. After a couple of minutes (depending on your cell line), detach the cells from the bottom of the dish by pipetting with a 10mL pipette.
9. With 6.5mL of media from the 'Media' tube, rinse and collect the detached cells and transfer to the appropriate 15mL tube.
10. Centrifuge the tube with the cells for 3-minutes at 200g.
11. Dump the supernatant to waste.
12. Add 5mL of DPBS to the tube with the cell pellet. There is no need to mix here.
13. Centrifuge the tube for 3-minutes at 200g.
14. Dump the supernatant to waste and spirate the remaining liquid to leave as little as possible.
15. Place the cell pellet on dry ice until frozen and keep at -80C until use.

<hr style="height:6pt; visibility:hidden;" />

<span id="2-sucrose-gradient-preparation"></span>

## 2. Sucrose gradient preparation

The gradient preparation protocol is based on the use of the SW-61Ti rotor type. If you have another rotor (e.g. SW-41Ti), just scale up the volumes. We opt to use a 'compact' gradient to help reduce processing volumes downstream. Use only RNase-free reagents.

<span id="21-reagents-and-materials"></span>

### 2.1 Reagents and materials

- 50mL tubes (VWR, CAT#89093-190)
- Ultra-clear tubes, 11x60mm, 4mL (Beckman, CAT#344062)
- BD Luer-lock syringes, 5mL (VWR, CAT#B309646)
- Blunt ended needles, 20-gauge, 15cm (VWR, CAT#20068-676)
- Nalgene Rapid-Flow filter units, 500mL, 0.2um filter (VWR, CAT#73520-984)
- RNaseZAP wipes (Thermo Fisher, CAT#AM9788)
- 1M HEPES pH 7.3 (Thermo Fisher, CAT#BP299-1)
- MgCl2 (Sigma, CAT#M8266)
- KCl (Sigma, CAT#P9333)
- Sucrose (Thermo Scientific, CAT#15503022)
- Nuclease-free water (Thermo Fisher, CAT#10977023)

<span id="22-solution-recipes"></span>

### 2.2 Solution recipes

- 2M KCl - 7.45g in 50mL of water
- 0.5M MgCl2 - 5.08g in 50mL of water
- Polysome base buffer (10X)
  - 200mM HEPES pH 7.3 (100mL of 1M stock)
  - 1.5M KCl (56.0g)
  - 150mM MgCl2 (7.1g)
  - water to 500mL
  - filter and store at +4C indefinitely
- 10% (w/v) sucrose - 4g in 36mL of water, 4mL of Polysome base buffer (filter and keep at +4C)
- 34% (w/v) sucrose - 13.6g in 36mL of water, 4mL of Polysome base buffer (filter and keep at +4C)
- 45% (w/v) sucrose - 18g in 36mL of water, 4mL of Polysome base buffer (filter and keep at +4C)

<span id="23-protocol"></span>

### 2.3 Protocol

Make sure you have read and understood the protocol below before proceeding. The gradients are the most important part of this protocol, so take your time here. Practice makes perfect and sucrose is cheap, so practice your technique in a waste tube before hand if you want. I like to make my gradients the day before I plan to run samples. The lysis protocol is based on the use of the 'short' lids during gradient preparation.

1. Prepare the sucrose solutions according to the recipe's above and allow the solutions to equilibrate to room temperature for 30-minutes or so.
2. Prep your workspace by cleaning it with an RNaseZap wipe.
3. Prepare a 50mL tube containing RNA clean water, and another containing a solution of 10% (v/v) RNaseZap.
4. Place an ultracentrifuge tube in the appropriate jig and mark the halfway point using a marker (this depends on which lids you will use, the short lids use the upper line on the jig).
5. Using a standard pipette, add 750uL of the 10% sucrose solution to each tube.
6. Attach a blunt needle to a syringe and draw 3mL of the 10% RNaseZap solution into the syringe and expel back into the same tube. Repeat this process 2-times for a total of 3 rinses.
7. Draw 3mL of RNA clean water into the syringe and expel to waste. Repeat this process 2-times for a total of 3 rinses.
8. Draw a small amount of the 34% sucrose into the syringe and discard to waste.
9. Draw approximately 3mL of 34% sucrose into the syringe, slowly to avoid bubbles, and quickly transfer the needle to the bottom of the ultracentrifuge tube and slowly fill the tube to the halfway point made with the marker. I generally like to fill just beyond the halfway mark (1-2mm), being consistent to do the same thing across each tube.
10. Repeat this process for each of the ultracentrifuge tubes.
11. Discard any remaining 34% sucrose solution and draw a small amount of 45% sucrose into the syringe and discard it to waste. 
12. Draw approximately 3mL of 45% sucrose into the syringe, slowly to avoid bubbles, and quickly transfer the needle to the bottome of the ultracentrifuge tube and slowly fill the tube to the halfway point. Be consistent.
13. Repeat this process for each of the ultracentrifuge tubes.
14. Rinse the syringe 3x with water, and then 3x with RNase ZAP water, blowing out any extra liquid, and place the needle in a bag to be autoclaved. Discard the used syringe.
15. Take a short or long tube cap (depending on which jig mark you used) and hold it with the hole in the cap facing your person. Hold the ultracentrifuge tube you plan to cap with your other hand along with a KimWipe. With the cap at a 45 degree angle, insert the cap into the tube such that any liquid that is expelled from the tube enters through the hold in the cap and goes into the top of the cap.
16. Pipette any extra sucrose solution that has expelled into the cap to waste and use the KimWipe in your hand to clean the sides of the tube, if necessary. Repeat this capping process for all tubes.
17. Place the prepared gradients in the cold room for use the next day. 

<hr style="height:6pt; visibility:hidden;" />

<span id="3-rna-and-protein-sample-preparation"></span>

## 3. RNA, polysome, and protein Sample Preparation

As the goal here is to measure RNA and proteins, make an effort to minimize potential keratin and RNase contamination (e.g. wear a lab coat and don't touch your tubes with un-gloved hands). I like to use the [Zymo RNA kit that works with Trizol](https://www.zymoresearch.com/pages/direct-zol-rna-purification-kits), but you can substitute virtually any RNA isolation kit you would like. The Trizol kit is nice because it works with sucrose and eliminates having to do any sort of precipitation.

<span id="31-reagents-and-materials"></span>

### 3.1 Reagents and materials

- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- Benchtop centrifuge with holder for microcentrifuge tubes (multiple vendors)
- SW60Ti rotor (Beckman)
- RNaseZAP wipes (Thermo Fisher, CAT#AM9788)
- DPBS (Thermo Scientific, CAT#14190144)
- HEPES (Sigma, CAT#H3375)
- NaOH, 10M (Sigma, CAT#72068)
- MgCl2 (Sigma, CAT#M8266)
- KCl (Sigma, CAT#P9333)
- NP-40 (Sigma, CAT#NP40)
- 5M NaCl (Thermo Scientific, CAT#AM9760G)
- 1M TrisCl, pH 7.5 (Thermo Scientific, CAT#15567027)
- TURBO DNase, 2U/uL (Thermo Fisher, CAT#AM2238)
- Tween20, 50% solution (Thermo Fisher, CAT#003005)
- Cycloheximide (Sigma, CAT#C7698)
- Deoxycholate (DOC) (Sigma, CAT#D6750)
- Dynabeads, protein G (Thermo Scientific, CAT#10003D)
- 20% SDS (Thermo Scientific, CAT#BP1311)
- cOmplete protease inhibitor tablets, EDTA free (Sigma, CAT#11836170001)
- Dithiothreitol (Bio-Rad, CAT#1610611)
- Chloroacetamide (Sigma, CAT#C0267)
- Benzonase nuclease, 25U/uL (Sigma, CAT#70664-10KUN)
- RNase A, 10mg/mL (Thermo Scientific, CAT#EN0531)
- Urea (Sigma, CAT#U5128)
- RiboLock RNase inhibitor (Thermo Scientific, CAT#EO0382)
- Nuclease-free water (Thermo Scientific, CAT#10977023)
- Direct-Zol RNA Kit (Zymo Research, CAT#R2061)
- Trypsin/rLysC mix (Promega, CAT#V5071)
- Thermomixer with 2mL tube block (Eppendorf)
- Thermoblock set to >95C (multiple vendors)
- Magnetic rack for 1.5mL or 2.0mL tubes (I like this rack: Promega, CAT#Z5342)
- Ethanol, absolute (whatever vendor sells this to your lab)
- SP3 beads (Thermo Scientific, CAT#65152105050250, CAT#45152105050250)
- Acetone (Sigma, CAT#179124)
- C18 SlitPlates (CAT#S2C18, Glygen Corp.)
- Acetonitrile, HPLC grade (CAT#51101, Thermo Scientific)
- Water, HPLC grade (CAT#51140, Thermo Scientific)
- Trifluoroacetic acid, HPLC grade (CAT#85183, Thermo Scientific)
- Formic acid, HPLC grade (CAT#85178, Thermo Scientific)
- 1.5mL snap-lock tubes (CAT#05-402-25, Thermo Scientific)
- Benchtop centrifuge with plate-holder rotor (multiple vendors)

<span id="32-solution-recipes"></span>

### 3.2 Solution recipes

- 100mM HEPES pH 8.5 - 2.5g of HEPES powder, 100mL of water, ~900uL of 10M NaOH
- 100mM HEPES pH 8.0 - 2.5g of HEPES powder, 100mL of water, ~700uL of 10M NaOH
- 2M KCl - 7.45g in 50mL of water
- 0.5M MgCl2 - 5.08g in 50mL of water
- 0.2M of dithiothreitol (DTT) - 15mg in 500uL of 100mM HEPES pH 8.5, prepare fresh
- 0.8M of chloroacetamide (CAA) - 37mg in 500uL of 100mM HEPES pH 8.5, prepare fresh
- 10% (v/v) NP-40 - 1mL in 9mL of water
- 10% (w/v) DOC - 1g in 10mL of water
- 10X cOmplete protease inhibitor stock - 1 tablet in 1mL of water
- 100mg/mL cycloheximide - 50mg in 500uL of DMSO
- 4M urea (240mg in 1mL of 100mM HEPES pH 8, prepare just before use)
- Lysis buffer A (need 550uL per sample, recipe for 4mL)
  - 20mM HEPES pH 7.3 (80uL of 1M stock)
  - 150mM KCl (304uL of 2M stock)
  - 5mM MgCl2 (40uL of 0.5M stock)
  - 0.5% (v/v) NP-40 (200uL of 10% stock)
  - 0.5% (v/v) DOC (200uL of 10% stock)
  - 0.5X cOmplete protease inhibitor (200uL of 10X stock)
  - 10U TURBO DNase per mL (20uL of 2U/uL stock)
  - 200ug/mL cycloheximide (8uL of 100mg/mL stock)
  - water to 1mL (2,948uL of clean water)
- Nuclease mix (need 10uL per sample, recipe for 100uL)
  - 100U benzonase (4uL of stock)
  - 50ug RNase A (5uL of stock)
  - water to 100uL
- Lysis buffer B (need 50uL per sample, recipe for 1mL)
  - 600mM HEPES pH 8.5 (600uL of 100mM stock)
  - 8% (v/v) SDS (400uL of 20% stock)
  - 10mM DTT (6mg of powder)
- 1X TBST (prepare fresh, recipe for 40mL)
  - Tris-Cl pH 7.5 (800uL of 1M stock)
  - NaCl (1.2mL of 5M stock)
  - Tween20 (40uL of 100% stock)
  - Water (38mL)
  - RiboLock RNase inhibitor (8uL) 
- 80% (v/v) ethanol (prepare fresh)
- Buffer A - 0.1% trifluoroacetic acid (TFA) in acetonitrile
- Buffer B - 0.1% TFA in water
- Rinse buffer - 0.1% formic acid in water
- Elution buffer - 0.1% formic acid in 60% acetonitrile
- Sample reconstitution buffer - 1% formic acid in water
- AxyMats Sealing mat for 96-well microplates (VWR, CAT#14-222-024)
- 96-well PCR microplates (VWR, CAT#14-222-326)

<span id="33-protocol"></span>

### 3.3 Protocol

Prior to starting, prepare sufficient Lysis buffer A and B for all of the samples to be processed. Make sure you have a Thermoblock heated to +95C or greater. Pre-chill the ultracentrifuge and a benchtop centrifuge to +6C. Weigh out the CAA and Urea powders into tubes, but don't reconstitute until just before you will use them. Prepare 12 tubes for each sample to be processed (two for lysate - 1.5mL tube, one for RNA - 1.5mL tube, one for protein - 2mL tube, 4 for IPs - 1.5mL tubes, and 4 for polysomes - 1.5mL tubes). 

1. To each protein tube, add 10uL of Nuclease mix. To each RNA tube, add 375uL of Trizol Lysis buffer (from Zymo kit).
2. To each cell pellet harvested previously, add 400uL of Lysis buffer A and pipette mix. 
2. Transfer 25uL of this total lysate to an RNA tube containing 375uL of Trizol lysis buffer. Vortex mix and freeze at -80C.
3. Transfer 75uL of this total lysate to a protein tube containing the nuclease mix and lysis buffer and pipette mix. Incubate for 10-minutes at +24C.
4. During this incubation, transfer the total lysate to a centrifuge and spin at 5,000g for 5-minutes at +6C.
5. After the spin, transfer the supernatant to a fresh 1.5mL tube and discard the nuclei pellet. Place on ice for now.
6. After the protein incubation is finished, add 25uL of Lysis buffer B to the protein lysate and pipette mix. 
7. Place the protein lysate in the pre-heated Thermoblock at +95C and incubate for 5-minutes.
8. During this incubation, transfer 125uL of the clarified lysate to the IP tube and add 5ug of your target antibody (for an IgG, prepare a non-tag expressing line alongside, or use a small aliquot of the lysate combined from all three replicates). Incubate for 1-hour at +24C with end-over-end rotation.
9. Remove the protein lysate from the Thermoblock and let sit at +24C for 10-minutes. Quick-spin the tubes at low speed to remove any condensation from the lid (e.g. 250g for 30 seconds).
10. During this incubation period, load 150uL of the clarified lysate onto your polysome gradients. 
11. Taking care, partially secure the bucket lids to the buckets now containing loaded gradients.
12. Carefully transfer the ice bucket with the gradients to the ultracentrifuge area along with the rotor. One by one and keeping them vertical throughout, pick up the buckets, secure the bucket lids (fingertight, tightening at the base of the lid), and load into the rotor. Repeat for all tubes and ensure the rotor buckets are loaded in their correct locations and properly.
13. Press 'Open Vent' on the ultracentrifuge. Once the vacuum has released, it will make a chime sound to indicate the lid can be opened.
14. Load the rotor into the unit taking care to keep it vertical (you don't want your gradients to shift).
15. Close the lid and press 'Start Vacuum'.
16. Press 'Start' to begin the spin. Stand and watch to make sure it hits the appropriate speed and that everything is OK.
17. Clean the ultracentrifuge tube caps with water and place back with the BioComp unit. Proceed to the next section to fractionate your sucrose gradients after the spin has finished.
18. Going back to the protain prep, reconstitute your CAA powder in 1000uL of HEPES pH 8.5.
19. Add 10uL of CAA to the protein lysate and vortex mix. Incubate at +24C for 30-minutes in the dark.
20. During this incubation, prepare your Protein G beads by rinsing 25uL per sample in 800uL of TBST for a total of 3x rinses. Reconstitute the rinsed beads in 25uL of TBST per sample.
21. To your incubated IP sample, add 25uL of rinsed protein G beads and incubate for an additional 1-hour at +24C with end-over-end rotation.
22. Going back to the protein prep, reconstitute your DTT in 100mM HEPES pH 8.5, and add 10uL to each tube of protein lysate and vortex mix. At this point you can freeze your protein samples at -80C indefinitely, use them directly in a Western blot (need to add loading buffer), or proceed with clean-up and disgestion as below.

For IP preparation:

1. Place IP samples on a magnetic rack and discard the supernatant. 
2. Rinse the IP beads 5x with 800uL of TBST and reconstitute the beads in 100uL of 100mM TrisCl pH 7.5.
3. Transfer 50uL of the IP to a fresh tube and add 5uL of proteinase K and incubate at +55C for 10-minutes.
4. To the remaining IP, add 2.5uL of RNaseA and 2.5uL of benzonase and incubate at room temperature for 20-minutes.
5. For the RNA IP, place the samples on the magnetic rack and recover the supernatant to a fresh 1.5mL tube and add 350uL of RNA lysis buffer (Zymo kit) and store at -80C until purification.
6. For the protein IP, rinse the IP beads 3x with TBST and reconstitute in 75uL of Lysis buffer A.
7. Add 25uL of Lysis buffer B and incubate at +55C for 10-minutes. 
8. Place samples on a magnetic rack and recover the supernatant to a fresh 2mL tube. Store at -80C until purification.  

For protein preparation:

1. Prepare the SP3 beads stock:
    1. Vortex the bead stock to re-suspend the material.
    2. Take 500uL of each of the bead stocks and combine in a fresh 2mL tube.
    3. Place on a magnetic rack and wait for beads to settle. Discard the supernatant.
    4. Reconstitute the beads in 1mL of water with pipetting and place back on the magnetic rack. After the beads settle, discard the supernatant.
    5. Repeat the above rinse one additional time for a total of 2 rinses.
    6. Reconstitute the beads in 500uL of water. The bead stock can be stored at +4C indefinitely.
2. Add 10uL of SP3 bead stock to each tube of protein lysate and gently shake the tube to mix.
3. Add 800uL of acetone to each tube of protein lysate and gently shake the tube to mix. Incubate at +24C for 5-minutes.
4. During the above incubation, prepare your digestion mixture:
    1. Reconstitute urea powder to 1mL with ~800uL of 100mM HEPES pH 8. Vortex mix.
    2. Reconstitute a trypsin/rLysC vial using 200uL of the provided reconstitution solution.
    3. Transfer 10uL of trypsin per sample to a fresh tube, and add 100uL of prepared urea per sample. Vortex mix and keep on ice.
5. Centrifuge the protein lysate tubes at 5,000g for 5-minutes.
6. Discard the supernatant from each tube and add 800uL of 80% ethanol. Gently shake the tube to mix.
7. Centrifuge the tubes at 5,000g for 5-minutes and discard the supernatant. Using a P200 micropipette, make sure you have removed as much liquid as possible from the tubes.
8. Add 100uL of the prepared trypsin/urea mix to each tube. Do not attempt to mix, vortex, or pipette.
9. Transfer the tubes to a shaking Thermomixer set at +30C and 1,000rpm, and digest for 2-4 hours.
10. Add 300uL of 100mM HEPES pH 8 to each tube and place back in the Thermomixer and incubate overnight at +30C and 1,000rpm mixing.
11. The next day, spin the tubes at 12,000g for 2-minutes. Add 8uL of acetonitrile to each tube and vortex mix.
12. Centrifuge the tubes again at 12,000g for 2-minutes, and then place on a magnetic rack.
13. Clean up your sample using a SlitPlate:
    1. Add 200uL of Buffer A to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
    2. Add 200uL of Buffer B to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
    3. Add 200uL of the peptide samples to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
    4. Repeat Step 3 to load the remainder of the sample.
    5. Add 200uL of Rinse buffer to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
    6. Add 180uL of Elution buffer to the SlitPlate wells and centrifuge at 250g for 3-minutes.
    7. Transfer the elution from the collection plate to fresh 1.5mL tubes for each sample.
14. Concentrate the peptide sample by evaporation. You can use a SpeedVac or a Lyophilizer for this purpose.
15. After the sample is evaporated, add 20uL of Sample reconstitution buffer to the tube, vortex, and then spin at 12,000g for 2-minutes.
16. Transfer the reconstituted peptides to a 96-well plate with a silicone mat lid.
17. Samples can be stored at this stage at -20C until analysis.

<hr style="height:6pt; visibility:hidden;" />

<span id="4-sucrose-gradient-fractionation"></span>

## 4. Sucrose gradient fractionation

Use only RNase-free reagents.

<span id="41-reagents-and-materials"></span>

### 4.1 Reagents and materials

- 96-well plate (many are suitable, I like Sigma, CAT#CLS3365)
- RNA clean water (Thermo Fisher, CAT#10977023)
- Absolute ethanol (multiple vendors)
- Ultra-clear tubes, 11x60mm, 4mL (Beckman, CAT#344062)
- BioComp Gradient Station (BioComp)

<span id="42-solution-recipes"></span>

### 4.2 Solution recipes

- 70% ethanol (70mL ethanol + 30mL water)
- 20% ethanol (20mL ethanol + 80mL water)

<span id="43-protocol"></span>

### 4.3 Protocol

1. When the ultracentrifuge is approximately 15-minutes from finished, turn on the laptop attached to the BioComp unit and load into Windows. Plug in the USB for the BioComp unit to the laptop.
2. Turn on the BioComp unit and the Gilson fraction collector attached to it.
3. On the BioComp unit, press 'SCAN'.
4. Open the Triax software on the laptop (shortcut is on the desktop). It will give an error about a warmup object, just ignore this and hit OK.
5. Choose your username and the appropriate rotor (SW60Ti in this case) and hit OK.
6. In the page that appears, enter your gradient settings in the boxes at the bottom. Press the 'Goto Scan Setup' button.
7. On this page you can specify how many fractions you would like. Always choose a number beyond what you actually want. For example, for 48 fractions across an entire polysome profile I will choose 64 fractions in the software. The other settings will auto-update from this setting.
8. Press the 'Goto Graph' button.
9. A prompt will appear asking you to name your sample, so do so.
10. A prompt will appear asking you to prepare for calibration. On the BioComp unit, press and hold the 'Rinse' key until the liquid from the syringe reservoir on the right side of the unit is almost entirely drained.
11. Fill the reservoir with 20mL of RNA clean water and hold the 'Rinse' key again until it is almost drained.
12. Fill the reservoir with 50mL of RNA clean water.
13. This time, while pressing and holding the 'Rinse' key, press OK in the software to do calibration and then OK to start the blanking process. Continue to hold the 'Rinse' key throughout the whole process until it says that blanking is complete. 
14. While holding the 'Rinse' key, open the gold screw on the top of the BioComp unit until it is completely open. Release the 'Rinse' key.
15. Press the 'Air' key on the BioComp unit for 10-seconds and then release it and close the gold screw.
16. Place a sample collection plate in the fraction collector.
17. Fill a blank ultracentrifuge tube with RNA clean water and place it in the BioComp gradient holder (if you are unsure how to use this, ask).
18. In the software, press 'Start Run'. Hit 'OK' on the two prompts that follow. The run should start.
19. Once the run is finished, hit 'OK' on the prompt that appears asking about using the air button to expel the remaining material.
20. Hit 'End' on the Gilson Fraction Collector and remove your fraction plate and replace it with a fresh plate. Collect your fractions to fresh 1.5mL tubes and store at -80C until purification.
21. Press and hold the 'Rinse' key to rinse the tubing and open the gold screw while doing this.
22. Press and hold the 'Air' key for 10-seconds and then release it and close the gold screw.
23. Press 'New Run' in the software. Press 'Yes' for identical sample, 'No' for doing another blank calibration and name your sample.
24. When the ultracentrifuge spin has finished, press the 'Open Vent' key and wait for the chime signaling that the door can be opened.
25. Remove the rotor from the unit, close the lid, and power off the machine.
26. Place the ultracentrifuge buckets with your gradients on ice.
27. Using tweezers, remove a sucrose gradient from a bucket and load it into the gradient holder on the BioComp.
28. Hit 'Start Run' in the software and 'OK' on the two prompts that follow.
29. Once the sample is finished, repeat steps 19 - 28 for any remaining samples.
30. When you are finished, repeat steps 19 - 28 with a blank tube of water (the same tube from the previous blank can be re-used).
31. Wipe the silicon trumpet clean with a KimWipe, as well as the BioComp unit itself if any sucrose has spilled.
36. Clean the gradient holder and the ultracentrifuge buckets with water.
37. On the BioComp unit, press and hold the 'Rinse' button to flush the remaining water from the reservoir while also opening the gold screw.
38. Press and hold the 'Air' key for 10-seconds then release and close the gold screw.
39. Add 20mL of 70% ethanol to the reservoir and use the 'Rinse' key to flush it through the BioComp unit.
40. Add 30mL of 20% ethanol to the reservoir and use the 'Rinse' key to flush 10mL of it through the BioComp unit. There should now be 20mL remaining for storage.
41. Turn the BioComp unit and Gilson fraction collector off. Turn off the laptop and unplug the USB.
42. The RNA from the sucrose fractions can be directly extracted using the Trizol reagent from the Zymo kit.

<hr style="height:6pt; visibility:hidden;" />