# Proteomic analysis of extracellular vesicles <!-- omit in toc -->

This document describes an end-to-end protocol for quantitative analysis of EV proteomes by mass spectrometry. The protocol also provides an avenue to enrich RNA from the same isolated material. This protocol is also appropriate for harvesting material for other assays, such as qPCR or Western blotting, and does not require any specialized equipment (e.g. sonicator). This protocol can be used as a general guideline as there are many different ways of doing many of these individual steps and still achieving success. The topics covered include how to perform lysis of material, clean-up of proteins, tryptic digestion, and final peptide clean-up.

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [1. RNA and Protein Sample Preparation](#1-rna-and-protein-sample-preparation)
  - [1.1 Reagents and materials](#11-reagents-and-materials)
  - [1.2 Solution recipes](#12-solution-recipes)
  - [1.3 Protocol](#13-protocol)

<hr style="height:6pt; visibility:hidden;" />

<span id="1-rna-and-protein-sample-preparation"></span>

## 1. RNA and Protein Sample Preparation

For all the solutions described below and throughout this protocol in general, you should do your best to use sterile glassware and reagents. As the goal here is to measure RNA and proteins, make an effort to minimize potential keratin and RNase contamination (e.g. wear a lab coat and don't touch your tubes with un-gloved hands). I like to use the Zymo RNA kit to purify total RNA, but you can substitute virtually any RNA isolation kit you would like.

<span id="11-reagents-and-materials"></span>

### 1.1 Reagents and materials

- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- Benchtop centrifuge with holder for microcentrifuge tubes (multiple vendors)
- 1M TrisCl pH 7.5 (Thermo Scientific, CAT#J60636.K2)
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
- Direct-Zol RNA microprep kit (Zymo Research, CAT#R2061)
- Trypsin/rLysC mix (Promega, CAT#V5071)
- Thermomixer with 2mL tube block (Eppendorf)
- Thermoblock set to >95C (multiple vendors)
- Cell scrapers (multiple vendors)
- Magnetic rack for 1.5mL or 2.0mL tubes (I like this rack: Promega, CAT#Z5342)
- Ethanol, absolute (whatever vendor sells this to your lab)
- SP3 beads (Thermo Scientific, CAT#65152105050250, CAT#45152105050250)
- Acetone (Sigma, CAT#179124)
- Strata-X microelution SPE plates (CAT# 8M-S100-4GA, Phenomenex)
- Methanol, HPLC grade (CAT#610090040, Thermo Scientific)
- Water, HPLC grade (CAT#51140, Thermo Scientific)
- Trifluoroacetic acid, HPLC grade (CAT#85183, Thermo Scientific)
- Formic acid, HPLC grade (CAT#85178, Thermo Scientific)
- 1.5mL snap-lock tubes (CAT#05-402-25, Thermo Scientific)
- Benchtop centrifuge with plate-holder rotor (multiple vendors)

<span id="12-solution-recipes"></span>

### 1.2 Solution recipes

- 100mM TrisCl pH 7.5 - 1mL of 1M stock, 9mL of water
- 2M KCl - 7.45g in 50mL of water
- 0.5M MgCl2 - 5.08g in 50mL of water
- 0.1M of dithiothreitol (DTT) - 15mg in 1mL of 100mM TrisCl pH 7.5, prepare fresh
- 0.4M of chloroacetamide (CAA) - 37mg in 1mL of 100mM TrisCl pH 7.5, prepare fresh
- 10% (v/v) NP-40 - 1mL in 9mL of water
- 10% (w/v) DOC - 1g in 10mL of water
- 10X cOmplete protease inhibitor stock - 1 tablet in 1mL of water
- 4M urea (240mg in 1mL of 100mM HEPES pH 8, prepare just before use)
- Lysis buffer A (need 200uL per sample, recipe for 1mL)
  - 20mM TrisCl pH 7.5 (200uL of 100mM stock)
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
  - 600mM TrisCl pH 7.5 (600uL of 100mM stock)
  - 8% (v/v) SDS (400uL of 20% stock)
  - 10mM DTT (6mg of powder)
- 80% (v/v) ethanol (prepare fresh)
- Buffer A - methanol
- Buffer B - 0.1% trifluoroacetic acid (TFA) in water
- Rinse buffer - 0.1% formic acid, 4% methanol, in water
- Elution buffer - 0.1% formic acid in 60% methanol
- Sample Reconstitution Solution - 1% formic acid in water
- AxyMats Sealing mat for 96-well microplates (VWR, CAT#14-222-024)
- 96-well PCR microplates (VWR, CAT#14-222-326)

<span id="13-protocol"></span>

### 1.3 Protocol

This protocol assumes you have isolated EV material in the form of an ultracentrifuged pellet. Prior to starting, prepare sufficient Lysis buffer A and B for all of the samples to be processed. Make sure you have a Thermoblock heated to +95C or greater. Weigh out the CAA and Urea powders into tubes, but don't reconstitute until just before you will use them. Prepare 2 tubes for each sample to be processed (one for RNA - 1.5mL tube, one for protein - 2mL tube). To the RNA tubes, add 350uL of RNA lysis buffer to each (the RNA lysis buffer should be included with whatever kit you are using, or use a Trizol solution that is included with the Direct-Zol kit instead).

If you are not interested in RNA, you can use 150uL of Lysis Buffer A directly in Step 1 and skip Step 2. If you are worried about having sufficient material, you can use 75uL of Lysis Buffer A in Step 3, and 25uL of Lysis Buffer B in Step 4 and process your entire lysate in Step 11.

1. Add 200uL of Lysis buffer A to each EV pellet and reconstitute by pipetting. Keep in the ultracentrifuge tube on ice.
2. After you have harvested all of the samples in this manner, transfer 50uL of each lysate to the corresponding RNA tube containing RNA lysis buffer and vortex mix. These cells can be frozen at -80C for RNA extraction at a later time. This harvested RNA can be used for virtually any RNA assay (e.g. qPCR, RNA-seq).
3. To the remaining 150uL of lysate in the protein tube, add 10uL of nuclease mix and pipette mix. Incubate for 10-minutes at +24C without shaking.
4. After incubation, add 50uL of Lysis buffer B to the protein lysate and pipette mix.
5. Place the protein lysate in the pre-heated Thermoblock at +95C and incubate for 5-minutes.
6. Remove the protein lysate from the Thermoblock and let sit at +24C for 10-minutes. During this incubation, reconstitute your CAA powder in 1mL of 100mM TrisCl pH 7.5. It may be difficult to get this entirely into solution, but just get as much as you can.
7. Quick-spin the tubes at low speed to remove any condensation from the lid (e.g. 250g for 30 seconds). At this point, the protein lysate is compatible with Western blotting. I will usually add 6uL of 6X SDS Loading Buffer to 24uL of my sample, and run 20-30uL on a gel. 
8. Add 10uL of CAA to the protein lysate and vortex mix. Incubate at +24C for 30-minutes in the dark.
9. Reconstitute your DTT in 100mM TrisCl pH 7.5, and add 10uL to each tube of protein lysate and vortex mix. This is a good stop point. The samples here can be stored at -80C indefinitely, or directly used for other protocols such as Western blotting, as mentioned above.
10. To perform clean-up prior to digestion, prepare the SP3 beads stock (if you don't have an existing stock, otherwise skip to Step 14):
    1. Vortex the two 15mL containers of bead stocks from the manufacturer to re-suspend the material.
    2. Take 500uL of each of the bead stocks and combine in a fresh 2mL tube.
    3. Place on a magnetic rack and wait for beads to settle. Discard the supernatant.
    4. Reconstitute the beads in 1mL of water with pipetting and place back on the magnetic rack. After the beads settle, discard the supernatant.
    5. Repeat the above rinse one additional time for a total of 2 rinses.
    6. Reconstitute the beads in 500uL of water. This is your bead stock and it can be stored at +4C indefinitely.
11. To a fresh 2mL tube for each sample, add 10uL of SP3 bead stock and 90uL of your prepared lysate and mix by gentle shaking. The remaining lysate can be stored at -80C for validation assays (e.g. Western blotting), or as a backup sample if your protein digestion fails.
12. Add 400uL of acetone to each tube of protein lysate and gently shake the tube to mix (want to achieve 80% v/v of acetone, so scale accordingly). Incubate at +24C for 5-minutes.
13. During the above incubation, prepare your digestion mixture:
    1. Reconstitute urea powder to 1mL with ~800uL of 100mM TrisCl pH 7.5. Vortex mix.
    2. Reconstitute a 20ug trypsin/rLysC vial using 100uL of the provided reconstitution solution.
    3. Transfer 5uL of trypsin per sample to a fresh tube, and add 100uL of prepared urea per sample. Vortex mix and keep on ice.
14. Centrifuge the protein lysate tubes at 5,000g for 5-minutes at room temperature.
15. Discard the supernatant from each tube and add 800uL of 80% ethanol. Pipette mix to reconstitute the beads.
16. Centrifuge the tubes at 5,000g for 5-minutes and discard the supernatant. Using a P200 or P20 micropipette, make sure you have removed as much leftover liquid from the rinse as possible from the tubes.
17. Add 100uL of the prepared trypsin/urea mix to each tube. Do not attempt to mix, vortex, or pipette.
18. Transfer the tubes to a shaking Thermomixer set at +24C and 1,000rpm, and digest for 2-4 hours.
19. Add 300uL of 100mM TrisCl pH 7.5 to each tube and place back in the Thermomixer and incubate overnight at +24C and 1,000rpm mixing.
20. The next day, spin the tubes at 12,000g for 2-minutes and then place on a magnetic rack.
21. Clean up your sample using a Strata-X SPE plate:
    1. Add 200uL of Buffer A to the SPE plate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
    2. Add 200uL of Buffer B to the SPE plate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
    3. Add 200uL of the peptide samples to the SPE plate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
    4. Repeat Step 3 to load the remainder of the sample.
    5. Add 200uL of Rinse buffer to the SPE plate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
    6. Add 200uL of Elution buffer to the SPE plate wells and centrifuge at 250g for 3-minutes.
    7. Transfer the elution from the collection plate to fresh 1.5mL tubes for each sample.
22. Concentrate the peptide sample by evaporation. You can use a SpeedVac or a Lyophilizer for this purpose.
23. After the sample is evaporated, add 20uL of Sample Reconstitution Solution to the tube, vortex, and then spin at 12,000g for 2-minutes.
24. Transfer 10uL of the reconstituted peptides to a 96-well plate with a silicone mat lid. Freeze the remainder of the peptide material at -80C.
25. Samples for MS analysis in the 96-well plate can be stored at this stage at -20C until analysis.
