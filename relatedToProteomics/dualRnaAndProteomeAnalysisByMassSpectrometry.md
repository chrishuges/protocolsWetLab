# Dual RNA and proteome analysis by mass spectrometry <!-- omit in toc -->

This document describes an end-to-end protocol for quantitative whole-proteome analysis by mass spectrometry that also harvests matched material that can be used for RNA sequencing. This protocol can be used as a general guideline as there are many different ways of doing many of these individual steps and still achieving success. The topics covered include how to perform harvest and lysis of cell line material, clean-up of proteins, tryptic digestion, and final peptide clean-up. The protocol is designed to work with cell line material, but may be appropriate for tissues or other sources.

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [1. RNA and Protein Sample Preparation](#1-rna-and-protein-sample-preparation)
  - [1.1 Reagents and materials](#11-reagents-and-materials)
  - [1.2 Solution recipes](#12-solution-recipes)
  - [1.3 Protocol](#13-protocol)

<hr style="height:6pt; visibility:hidden;" />

<span id="1-rna-and-protein-sample-preparation"></span>

## 1. RNA and Protein Sample Preparation

This protocol assumes you have your cells growing in conventional 6-well dishes. If you are using a 10cm or bigger dish, I suggest harvesting your cells using trypsin and freezing the pellets and proceeding with the processing as below. For all the solutions described below and throughout this protocol in general, you should do your best to use sterile glassware and reagents. As the goal here is to measure RNA and proteins, make an effort to minimize potential keratin and RNase contamination (e.g. wear a lab coat and don't touch your tubes with un-gloved hands). I like to use the Zymo RNA kit here, but you can substitute virtually any RNA isolation kit you would like. 

<span id="11-reagents-and-materials"></span>

### 1.1 Reagents and materials

- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- Benchtop centrifuge with holder for microcentrifuge tubes (multiple vendors)
- DPBS (Thermo Scientific, CAT#14190144)
- HEPES (Sigma, CAT#H3375)
- NaOH, 10M (Sigma, CAT#72068)
- MgCl2 (Sigma, CAT#M8266)
- KCl (Sigma, CAT#P9333)
- NP-40 (Sigma, CAT#NP40)
- Deoxycholate (DOC) (Sigma, CAT#D6750)
- 20% SDS (Thermo Scientific, CAT#BP1311)
- cOmplete protease inhibitor tablets, EDTA free (Sigma, CAT#11836170001)
- Dithiothreitol (Bio-Rad, CAT#1610611)
- Chloroacetamide (Sigma, CAT#C0267)
- Benzonase nuclease, 25U/uL (Sigma, CAT#70664-3)
- RNase A, 10mg/mL (Thermo Scientific, CAT#EN0531)
- Urea (Sigma, CAT#U5128)
- Clean water (Thermo Scientific, CAT#10977023)
- Quick RNA Micoprep Kit (Zymo Research, CAT#R1050)
- Trypsin/rLysC mix (Promega, CAT#V5071)
- Thermomixer with 2mL tube block (Eppendorf)
- Thermoblock set to >95C (multiple vendors)
- Cell scrapers (multiple vendors)
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

<span id="12-solution-recipes"></span>

### 1.2 Solution recipes

- 100mM HEPES pH 8.5 - 2.5g of HEPES powder, 100mL of water, ~900uL of 10M NaOH
- 100mM HEPES pH 8.0 - 2.5g of HEPES powder, 100mL of water, ~700uL of 10M NaOH
- 2M KCl - 7.45g in 50mL of water
- 0.5M MgCl2 - 5.08g in 50mL of water
- 0.2M of dithiothreitol (DTT) - 15mg in 500uL of 100mM HEPES pH 8.5, prepare fresh
- 0.8M of chloroacetamide (CAA) - 37mg in 500uL of 100mM HEPES pH 8.5, prepare fresh
- 10% (v/v) NP-40 - 1mL in 9mL of water
- 10% (w/v) DOC - 1g in 10mL of water
- 10X cOmplete protease inhibitor stock - 1 tablet in 1mL of water
- 4M urea (240mg in 1mL of 100mM HEPES pH 8, prepare just before use)
- Lysis buffer A (need 200uL per sample, recipe for 1mL)
  - 20mM HEPES pH 8.5 (200uL of 100mM stock)
  - 150mM KCl (76uL of 2M stock)
  - 5mM MgCl2 (10uL of 0.5M stock)
  - 0.5% (v/v) NP-40 (50uL of 10% stock)
  - 0.5% (v/v) DOC (50uL of 10% stock)
  - 0.5X cOmplete protease inhibitor (50uL of 10X stock)
  - water to 1mL (565uL of clean water)
- Nuclease mix (need 10uL per sample, recipe for 100uL)
  - 100U benzonase (4uL of stock)
  - 50ug RNase A (5uL of stock)
  - water to 100uL
- Lysis buffer B (need 50uL per sample, recipe for 1mL)
  - 600mM HEPES pH 8.5 (600uL of 100mM stock)
  - 8% (v/v) SDS (400uL of 20% stock)
  - 10mM DTT (6mg of powder)
- 80% (v/v) ethanol (prepare fresh)
- Buffer A - 0.1% trifluoroacetic acid (TFA) in acetonitrile
- Buffer B - 0.1% TFA in water
- Rinse buffer - 0.1% formic acid in water
- Elution buffer - 0.1% formic acid in 60% acetonitrile
- Sample reconstitution buffer - 1% formic acid in water
- AxyMats Sealing mat for 96-well microplates (VWR, CAT#14-222-024)
- 96-well PCR microplates (VWR, CAT#14-222-326)

<span id="13-protocol"></span>

### 1.3 Protocol

Prior to starting, prepare sufficient Lysis buffer A and B for all of the samples to be processed. Make sure you have a Thermoblock heated to +95C or greater. Weigh out the CAA and Urea powders into tubes, but don't reconstitute until just before you will use them. Prepare 2 tubes for each sample to be processed (one for RNA, one for protein). To the RNA tubes, add 350uL of RNA lysis buffer to each.

1. Using a pipette, remove the culture medium from the growing cells on the 6-well plate.
2. Add 2mL of DPBS to each well and swirl the plate to rinse. Pipette up and discard the DPBS.
3. Add 200uL of Lysis buffer A to each well and rock the plate back and forth to ensure the cells are covered.
4. Working one well at a time, use a cell scraper to dislodge the cells and a micropipette to transfer 200uL of lysate to the protein tube. Repeat for each sample.
5. After you have harvested all of the samples in this manner, transfer 50uL of each lysate to the corresponding RNA tube containing RNA lysis buffer and vortex mix. These cells can be frozen at -80C for RNA extraction at a later time.
6. To the remaining 150uL of lysate in the protein tube, add 10uL of nuclease mix and pipette mix. Incubate for 10-minutes at +24C.
7. After incubation, add 50uL of Lysis buffer B to the protein lysate and pipette mix. 
8. Place the protein lysate in the pre-heated Thermoblock at +95C and incubate for 5-minutes.
9. Remove the protein lysate from the Thermoblock and let sit at +24C for 10-minutes. During this incubation, reconstitute your CAA powder in 500uL of HEPES pH 8.5.
10. Quick-spin the tubes at low speed to remove any condensation from the lid (e.g. 250g for 30 seconds).
11. Add 10uL of CAA to the protein lysate and vortex mix. Incubate at +24C for 30-minutes in the dark.
12. Reconstitute your DTT in 100mM HEPES pH 8, and add 10uL to each tube of protein lysate and vortex mix.
13. Prepare the SP3 beads stock:
  1. Vortex the bead stock to re-suspend the material.
  2. Take 500uL of each of the bead stocks and combine in a fresh 2mL tube.
  3. Place on a magnetic rack and wait for beads to settle. Discard the supernatant.
  4. Reconstitute the beads in 1mL of water with pipetting and place back on the magnetic rack. After the beads settle, discard the supernatant.
  5. Repeat the above rinse one additional time for a total of 2 rinses.
  6. Reconstitute the beads in 500uL of water. The bead stock can be stored at +4C indefinitely.
14. Add 10uL of SP3 bead stock to each tube of protein lysate and gently shake the tube to mix.
15. Add 800uL of acetone to each tube of protein lysate and gently shake the tube to mix. Incubate at +24C for 5-minutes.
16. During the above incubation, prepare your digestion mixture:
  1. Reconstitute urea powder to 1mL with ~800uL of 100mM HEPES pH 8. Vortex mix.
  2. Reconstitute a trypsin/rLysC vial using 200uL of the provided reconstitution solution.
  3. Transfer 10uL of trypsin per sample to a fresh tube, and add 100uL of prepared urea per sample. Vortex mix and keep on ice.
17. Centrifuge the protein lysate tubes at 5,000g for 5-minutes.
18. Discard the supernatant from each tube and add 800uL of 80% ethanol. Gently shake the tube to mix.
19. Centrifuge the tubes at 5,000g for 5-minutes and discard the supernatant. Using a P200 micropipette, make sure you have removed as much liquid as possible from the tubes.
20. Add 100uL of the prepared trypsin/urea mix to each tube. Do not attempt to mix, vortex, or pipette.
21. Transfer the tubes to a shaking Thermomixer set at +24C and 1,000rpm, and digest for 2-4 hours.
22. Add 300uL of 100mM HEPES pH 8 to each tube and place back in the Thermomixer and incubate overnight at +24C and 1,000rpm mixing.
23. The next day, spin the tubes at 12,000g for 2-minutes. Add 8uL of acetonitrile to each tube and vortex mix.
24. Centrifuge the tubes again at 12,000g for 2-minutes, and then place on a magnetic rack.Remove cell pellet from the -80C freezer and allow to slowly thaw at room temperature (+21C).
25. Clean up your sample using a SlitPlate:
  1. Add 200uL of Buffer A to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
  2. Add 200uL of Buffer B to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
  3. Add 200uL of the peptide samples to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
  4. Repeat Step 3 to load the remainder of the sample.
  5. Add 200uL of Rinse buffer to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
  6. Add 180uL of Elution buffer to the SlitPlate wells and centrifuge at 250g for 3-minutes.
  7. Transfer the elution from the collection plate to fresh 1.5mL tubes for each sample.
26. Concentrate the peptide sample by evaporation. You can use a SpeedVac or a Lyophilizer for this purpose.
27. After the sample is evaporated, add 20uL of Sample reconstitution buffer to the tube, vortex, and then spin at 12,000g for 2-minutes.
28. Transfer the reconstituted peptides to a 96-well plate with a silicon mat lid.
29. Samples can be stored at this stage at -20C until analysis.
