# RNA binding protein site analysis with CLIP <!-- omit in toc -->

This protocol was last updated - May 18, 2020 by Chris Hughes.

This document describes a protocol for preparing performing an analysis of RNA binding protein (RBP) interaction sites on RNA. This protocol is based on the single-end, monitored eCLIP, and irCLIP2 protocols described previously (PMID: 28766298, 30252095, 31610236). Compared to these protocols, I use modifications at various steps during processing, as well as in the sequencing adapter configuration. Libraries made with this protocol can be sequenced on Illumina platforms, such as NextSeq, using single- or paired-end reads.

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [1. Cell culture and harvest](#1-cell-culture-and-harvest)
  - [1.1 Reagents and materials](#11-reagents-and-materials)
  - [1.2 Solution recipes](#12-solution-recipes)
  - [1.3 Protocol](#13-protocol)
- [2. Cell lysis, immunoprecipitation, and ligation](#2-cell-lysis-immunoprecipitation-and-ligation)
  - [2.1 Reagents and materials](#21-reagents-and-materials)
  - [2.2 Solution recipes](#22-solution-recipes)
  - [2.3 Oligos](#23-oligos)
  - [2.4 Protocol](#24-protocol)
- [3. SDS-PAGE and RNA isolation](#3-sds-page-and-rna-isolation)
  - [3.1 Reagents and materials](#31-reagents-and-materials)
  - [3.2 Solution recipes](#32-solution-recipes)
  - [3.3 Protocol](#33-protocol)
- [4. Phosphorylation, biotin capture, reverse transcription, and linker ligation](#4-phosphorylation-biotin-capture-reverse-transcription-and-linker-ligation)
  - [4.1 Reagents and materials](#41-reagents-and-materials)
  - [4.2 Solution recipes](#42-solution-recipes)
  - [4.3 Oligos](#43-oligos)
  - [4.4 Protocol](#44-protocol)
- [5. Library amplification and size selection](#5-library-amplification-and-size-selection)
  - [5.1 Reagents and materials](#51-reagents-and-materials)
  - [5.2 Solution recipes](#52-solution-recipes)
  - [5.3 Oligos](#53-oligos)
  - [5.4 Protocol](#54-protocol)

<hr style="height:6pt; visibility:hidden;" />

<span id="1-cell-culture-and-harvest"></span>

## 1. Cell culture and harvest

Use whatever cell culture methods you are compfortable with here. This stage of the protocol is only given as an example of a process that is validated to work and is by no means the only way to achieve a successful result in this section.

<span id="11-reagents-and-materials"></span>

### 1.1 Reagents and materials

- 15mL tubes (VWR, CAT#89093-186) - need 1 per sample
- 50mL tubes (VWR, CAT#89093-190) - need 3 in total
- Centrifuge with 15mL tube buckets (multiple vendors)
- TrypLE express (Thermo Fisher, CAT#12605028)
- DPBS, no calcium or magnesium (Thermo Fisher, CAT#14190144)
- Stratalinker UV Crosslinker, 254nm (Stratagene)
- Dry ice

<span id="12-solution-recipes"></span>

### 1.2 Solution recipes

- Cell culture medium (provided only as an example)
  - DMEM (500mL)
  - FBS (50mL)

<span id="13-protocol"></span>

### 1.3 Protocol

This protocol assumes you have your cells growing in 15cm dishes. For other dish sizes, simply scale the reagents for your purpose. Because you need to crosslink, I recommend only processing one to two plates at a time.

1. Label 1x15mL tube for each sample you plan to harvest.
2. Label a 50mL tube with 'TE', another with 'Media', and a last with 'PBS'.
3. To the 'TE' 50mL tube, add 8mL of TrypLE express per sample you plan to harvest.
4. To the 'PBS' 50mL tube, add 5mL of DPBS per sample you plan to harvest.
5. Remove the cell plate from the incubator and pipette the media the cells are growing in into the 50mL tube labeled 'Media'.
6. Carefully add 10mL of room temperature (+21C) DPBS to the plate, swirl, and discard the DPBS rinse to the waste.
7. Carefully add 5mL of room temperature DPBS to the plate and place on an ice block in the Stratalinker (make sure the plate is flat). Crosslink at 200mJ/cm2.
8. Remove the DPBS and add 8mL of TrypLE express to the plate and place back into the incubator.
9. Once the cells have started to detach, remove the plate from the incubator.
10. With 4mL of media from the 'Media' tube, rinse and collect the detached cells and transfer to the appropriate 15mL tube.
11. Centrifuge the tube with the cells for 3-minutes at 250g.
12. Dump the supernatant to waste.
13. Add 5mL of DPBS from the 'PBS' tube to the tube with the cell pellet. There is no need to pipette mix here.
14. Centrifuge the tube for 30-seconds at 250g.
15. Dump the supernatant to waste and spirate the remaining liquid to leave as little as possible.
16. Place the cell pellet on dry ice until frozen and keep at -80C until use.

<hr style="height:6pt; visibility:hidden;" />

<span id="2-cell-lysis-immunoprecipitation-and-ligation"></span>

## 2. Cell lysis, immunoprecipitation, and ligation

You should use an antibody that you have validated has good selectivity for your RBP of interest.

<span id="21-reagents-and-materials"></span>

### 2.1 Reagents and materials

- 1.5mL or 2.0mL Safe-Lock tubes (Fisher Scientific, CAT#05-402-25 or CAT#05-402-7)
- Benchtop centrifuge with holder for microcentrifuge tubes (multiple vendors)
- ThermoMixer with a 2mL block (Eppendorf)
- RNaseZAP wipes (Thermo Fisher, CAT#AM9788)
- TURBO DNase, 2U/uL (Thermo Fisher, CAT#AM2238)
- RNaseIn, 40U/uL (Promega, CAT#N2511)
- 1M TrisCl pH 7.5 (Thermo Fisher, CAT#15567027)
- 5M NaCl (Thermo Scientific, CAT#AM9760G)
- 0.5M EDTA (Thermo Scientific, CAT#15575020)
- NP-40 (Sigma, CAT#NP40)
- Deoxycholate (DOC) (Sigma, CAT#D6750)
- MgCl2 (Sigma, CAT#M8266)
- cOmplete protease inhibitor tablets, EDTA free (Sigma, CAT#11836170001)
- RNase 1, 100U/uL (Thermo Scientific, CAT#AM2294)
- RNA clean water (Thermo Scientific, CAT#10977023)
- FastPrep 5G instrument (MP Biomedicals)
- Lysing matrix D 2mL tubes (MP Biomedicals, CAT#116913050)
- Sucrose (Thermo Scientific, CAT#15503022)
- 20% SDS (Thermo Scientific, CAT#BP1311)
- Protein A/G magnetic beads (Thermo Scientific, CAT#88802)
- Bovine serum albumin, fraction V (Sigma, CAT#A2153)
- Dithiothreitol (Bio-Rad, CAT#1610611)
- PEG-8000 (Promega, CAT#V3011)
- QuickCIP (NEB, CAT#M0525L)
- T4 PNK (NEB, CAT#M0201L)
- T4 RNA Ligase 2, truncated KQ (NEB, CAT#M0373L)
- 10mM ATP (NEB, CAT#P0756S)
- T4 RNA ligase 1 (NEB, CAT#M0437M)

<span id="22-solution-recipes"></span>

### 2.2 Solution recipes

- 10% (v/v) NP-40 - 1mL in 9mL of water
- 10% (w/v) DOC - 1g in 10mL of water
- 50% (w/v) sucrose - 5g in 10mL of water (filter and keep at +4C)
- 10X cOmplete protease inhibitor stock - 1 tablet in 1mL of water
- 50% (w/v) PEG-8000 - 12.5g in 25mL of water
- 0.2M of dithiothreitol (DTT) - 15mg in 500uL of water, prepare fresh and keep on ice
- 0.5M MgCl2 - 5.08g in 50mL of water
- Diluted RNase 1 - 3uL of 100U/uL stock in 900uL of water
- Lysis buffer (need 1mL per sample)
  - 50mM Tris-Cl pH 7.5 (50uL of 1M stock)
  - 150mM NaCl (30uL of 5M stock)
  - 10% (w/v) sucrose (200uL of 50% stock)
  - 0.5% (v/v) NP-40 (50uL of 10% stock)
  - 0.5% (v/v) DOC (50uL of 10% stock)
  - 0.1% (v/v) SDS (5uL of 20% stock)
  - 0.5X cOmplete protease inhibitor (50uL of 10X stock)
  - 20U/mL TURBO DNase (10uL of 2U/uL stock)
  - 200U/mL SUPERaseIn (5uL of 40U/uL stock)
  - water to 1mL (550uL of pre-chilled water)
- Rinse buffer A (make 50mL)
  - 50mM Tris-Cl pH 7.5 (2.5mL of 1M stock)
  - 100mM NaCl (1mL of 5M stock)
  - 0.5% (v/v) NP-40 (2.5mL of 10% stock)
  - 0.5% (v/v) DOC (2.5mL of 10% stock)
  - 0.1% (v/v) SDS (250uL of 20% stock)
  - water to 50mL (42mL of pre-chilled water)
- Rinse buffer B (make 50mL)
  - 50mM Tris-Cl pH 7.5 (2.5mL of 1M stock)
  - 100mM NaCl (1mL of 5M stock)
  - 0.5% (v/v) NP-40 (2.5mL of 10% stock)
  - 0.5% (v/v) DOC (2.5mL of 10% stock)
  - 0.1% (v/v) SDS (250uL of 20% stock)
  - 0.1mg/mL BSA (5mg)
  - water to 50mL (42mL of pre-chilled water)
- Rinse buffer C (make 50mL)
  - 50mM Tris-Cl pH 7.5 (2.5mL of 1M stock)
  - 1M NaCl (10mL of 5M stock)
  - 5mM EDTA (500uL of 0.5M stock)
  - 0.5% (v/v) NP-40 (2.5mL of 10% stock)
  - 0.5% (v/v) DOC (2.5mL of 10% stock)
  - 0.1% (v/v) SDS (250uL of 20% stock)
  - water to 50mL (32mL of pre-chilled water)
- Rinse buffer D (make 50mL)
  - 50mM Tris-Cl pH 7.5 (2.5mL of 1M stock)
  - 10mM MgCl2 (1mL of 0.5M stock)
  - water to 50mL (46.5mL of pre-chilled water)
- PNK buffer 1 (make 1mL per sample)
  - 50mM Tris-Cl pH 7.5 (50uL of 1M stock)
  - 10mM MgCl2 (20uL of 0.5M stock)
  - 1mM DTT (5uL of 200mM stock)
  - water to 1mL (925uL)
- RNL buffer 1 (make 1mL per sample)
  - 50mM Tris-Cl pH 7.5 (50uL of 1M stock)
  - 10mM MgCl2 (20uL of 0.5M stock)
  - 1mM DTT (5uL of 200mM stock)
  - 20% (v/v) PEG-8000 (400uL of 50% stock)
  - water to 1mL (525uL)
- PNK buffer 2 (make 1mL per sample)
  - 50mM Tris-Cl pH 7.5 (50uL of 1M stock)
  - 10mM MgCl2 (20uL of 0.5M stock)
  - 1mM DTT (5uL of 200mM stock)
  - 1mM ATP (100uL of 10mM stock)
  - water to 1mL (825uL)
- RNL buffer 2 (make 1mL per sample)
  - 50mM Tris-Cl pH 7.5 (50uL of 1M stock)
  - 10mM MgCl2 (20uL of 0.5M stock)
  - 1mM DTT (5uL of 200mM stock)
  - 1mM ATP (100uL of 10mM stock)
  - 20% (v/v) PEG-8000 (400uL of 50% stock)
  - water to 1mL (425uL)

<span id="23-oligos"></span>

### 2.3 Oligos

- Ribo_3DNALinker_v4 (100nmol scale, RNase-free HPLC purified)
  - /5rApp/NNNGTCNNNTAGNNNAGATCGGAAGAGCACACGTCT/3ddC/
  - reconstitute to 20uM and aliquot. Store at -20C.
- Clip_5RNALinker_v4 (100nmol scale, RNase-free HPLC purified)
  - /5BiotinTEG/rCrArGrUrCrCrGrArCrGrArUrC
  - reconstitute to 20uM and aliquot. Store at -20C.

<span id="24-protocol"></span>

### 2.4 Protocol

Read this protocol before starting to make sure you are prepared for the steps as they come. All of the buffers should be cold (+4C). Pre-chill a benchtop centrifuge to +4C before starting. Pre-heat a Thermomixer to +37C before starting.

1. Prepare the antibody-conjugated beads (all rinses are 5-minutes at room temperature (+21C)):
   1. Wash 125uL of protein A/G beads with 500uL of Rinse buffer A in a 2mL tube. Discard the supernatant.
   2. Repeat the previous step two more times for a total of 3 rinses.
   3. Reconstitute the washed beads in 125uL of Rinse buffer A and transfer 25uL of this to a fresh 2mL tube (set this tube aside).
   4. Add 10ug of your target antibody to the remaining 100uL of beads in Rinse buffer A. Rotate slowly at room temperature for 1-hour.
   5. Rinse the conjugated beads twice with 500uL of Rinse buffer B (with BSA).
   6. Rinse the conjugated beads three times with Rinse buffer A.
   7. Reconstitute the beads in 100uL of Rinse buffer A until use. Keep on ice.
2. Prepare your lysate and perform IP:
   1. Slowly thaw cell pellet at room temperature until a small amount of frozen material remains.
   2. Add 1mL of Lysis buffer to the pellet and pipette mix. Incubate on ice for 5-minutes.
   3. Transfer the lysate to a Lysing matrix D tube and disrupt on a FastPrep (6M/s, 45 seconds, 1 cycle).
   4. Centrifuge the lysate at 12,000g for 2-minutes and recover the 900uL of supernatant to a fresh 2mL tube.
   5. Add 6uL of Diluted RNase 1. Pipette mix and incubate at +37C for 5-minutes.
   6. Centrifuge the lysate at 12,000g for 5-minutes at +4C.
   7. Transfer the supernatant to the tube containing 25uL of rinsed protein A/G beads prepared above. Incubate with slow rotation at +4C for 30-minutes.
   8. Recover the supernatant lysate and combine with the 100uL of conjugated beads prepared above. Incubate with slow rotation at +4C for overnight.
   9. The next day, recover 20uL of the lysate-bead mix to a fresh 2mL tube (**SampleInput**) and another 20uL to a different 2mL tube (**ImagingInput**). Store at +4C.
   10. Separate the remaining supernatant from the beads and transfer to a fresh 2mL tube. This can be saved as a backup or for Western blotting.
   11. Rinse the remaining beads twice with 500uL of Rinse buffer C. Discard the supernatant each time.
   12. Rinse the beads twice in 500uL of Rinse buffer A. Discard the supernatant each time.
   13. Rinse the beads twice with 500uL of Rinse buffer D. Discard the supernatant each time.
   14. Rinse the beads once with 500uL of PNK buffer 1. Discard the supernatant.
3. Perform on-bead treatment and ligation:
    1. Reconstitute the rinsed beads in 50uL of PNK buffer 1. Add 2uL of QuickCIP and 1uL of T4 PNK (10 Units of each) and pipette mix. Incubate at +37C for 30-minutes.
    2. Remove the supernatant and rinse once with 500uL of Rinse buffer C. Discard the supernatant.
    3. Rinse the beads twice in 500uL of Rinse buffer A. Discard the supernatant each time.
    4. Rinse the beads twice with 500uL of Rinse buffer D. Discard the supernatant each time.
    5. Rinse the beads once in 500uL of RNL buffer. Discard the supernatant.
    6. Reconstitute the rinsed beads in 45uL of RNL buffer 1. Add 5uL of Ribo_3DNALinker_v4 followed by 1uL of T4 RNA Ligase 2 truncated KQ (200 Units). Pipette mix and incubate at room temperature for 4-hours with gentle rotation.
    7. Remove the supernatant and rinse once with 500uL of Rinse buffer C. Discard the supernatant.
    8. Rinse the beads twice in 500uL of Rinse buffer A. Discard the supernatant each time.
    9. Rinse the beads twice with 500uL of Rinse buffer D. Discard the supernatant each time.
    10. Rinse the beads once in 500uL of PNK buffer 2. Discard the supernatant.
    11. Reconstitute the rinsed beads in 50uL of PNK buffer 2. Add 2uL of T4 PNK (20 Units) and pipette mix. Incubate at +37C for 30-minutes.
    12. Rinse the beads twice in 500uL of Rinse buffer A. Discard the supernatant each time.
    13. Rinse the beads twice with 500uL of Rinse buffer D. Discard the supernatant each time.
    14. Rinse the beads once in 500uL of RNL buffer 2. Discard the supernatant.
    15. Reconstitute the rinsed beads in 45uL of RNL buffer 2. Add 5uL of Clip_5RNALinker_v4 and 2uL of T4 RNA ligase 1 (60 Units). Pipette mix and incubate at room temperature overnight with gentle agitation.
    16. Remove the supernatant and rinse the beads twice in 500uL of Rinse buffer A. Discard the supernatant each time.
    17. Rinse the beads twice with 500uL of Rinse buffer D. Discard the supernatant each time.
    18. Reconstitute in 100uL of Rinse buffer D and keep on ice until SDS-PAGE.

<hr style="height:6pt; visibility:hidden;" />

<span id="3-sds-page-and-rna-isolation"></span>

## 3. SDS-PAGE and RNA isolation

<span id="31-reagents-and-materials"></span>

### 3.1 Reagents and materials

- 1.5mL or 2.0mL Safe-Lock tubes (Fisher Scientific, CAT#05-402-25 or CAT#05-402-7)
- Benchtop centrifuge with holder for microcentrifuge tubes (multiple vendors)
- ThermoMixer with a 2mL block (Eppendorf)
- RNaseZAP wipes (Thermo Fisher, CAT#AM9788)
- NuPAGE LDS Sample Buffer (4X) (Thermo Scientific, CAT#NP0007)
- PageRuler Prestained Protein Ladder, 10 to 180 kDa (Thermo Scientific, CAT#26616)
- NuPAGE 4 to 12%, Bis-Tris, 1.5 mm, Mini Protein Gel, 10-well (Thermo Scientific, CAT#NP0335BOX)
- NuPAGE MOPS SDS Running Buffer (20X) (Thermo Scientific, CAT#NP0001)
- XCell SureLock Mini-Cell Electrophoresis System (Thermo Scientific)
- 1M TrisCl pH 7.5 (Thermo Fisher, CAT#15567027)
- MgCl2 (Sigma, CAT#M8266)
- RNA clean water (Thermo Scientific, CAT#10977023)
- Dithiothreitol (Bio-Rad, CAT#1610611)
- NuPAGE Transfer Buffer (20X) (Thermo Scientific, CAT#NP0006)
- Amersham Protran Premium Western blotting membranes, nitrocellulose (Sigma, CAT#GE10600008)
- PVDF Transfer Membrane, 0.45 μm (Thermo Scientific, CAT#88518)
- Methanol, HPLC-grade (Sigma, CAT#34860-4L-R)
- TrueBlot Anti-Rabbit IgG HRP (Cedarlane, CAT#18-8816-31)
- DPBS, no calcium, no magnesium (Thermo Scientific, CAT#14190144)
- Powdered milk (grocery store)
- Tween 20 (Sigma, CAT#P9416)
- Tris base (Sigma, CAT#93362)
- NaCl (Sigma, CAT#71376)
- 12N HCl (Sigma, CAT#H1758)
- Pierce ECL Western Blotting Substrate (Thermo Scientific, CAT#32109)
- CL-XPosure Film (Thermo Scientific, CAT#34089)
- 0.5M EDTA (Thermo Scientific, CAT#15575020)
- 5M NaCl (Thermo Scientific, CAT#AM9760G)
- Proteinase K Solution (20 mg/mL) (Thermo Scientific, CAT#AM2546)
- Urea (Sigma, CAT#U5378)
- Razorblades (any will do)
- Acid-Phenol:Chloroform, pH 4.5 (with IAA, 125:24:1) (Thermo Scientific, CAT#AM9720)
- Phenol:Chloroform:Isoamyl Alcohol 25:24:1, Saturated with 10mM Tris, pH 8.0, 1mM EDTA (Sigma, CAT#P3803-100ML)
- Phaselock gel (heavy) (VWR, CAT#CA10847-802)
- RNA Clean & Concentrator-5 kit (Cedarlane, CAT#R1015)
- Absolute ethanol (wherever your institute normally procures this from)

<span id="32-solution-recipes"></span>

### 3.2 Solution recipes

- 1M of dithiothreitol (DTT) - 75mg in 500uL of water, prepare fresh and keep on ice
- 0.5M MgCl2 - 5.08g in 50mL of water
- Diluted marker - 2uL PageRuler Prestained Protein Ladder, 3uL NuPAGE LDS Sample Buffer (4X), 6uL water
- Rinse buffer D (make 50mL)
  - 50mM Tris-Cl pH 7.5 (2.5mL of 1M stock)
  - 10mM MgCl2 (1mL of 0.5M stock)
  - water to 50mL (46.5mL of pre-chilled water)
- 10X TBS (make 1L)
  - 200mM Tris base (24g)
  - 1.5M NaCl (88g)
  - water to 500mL
  - adjust to pH 7.6 with 12N HCl
  - water to 1L
- 1X TBST (make 1L)
  - 1X TBS (100mL)
  - water to 1L (900mL)
  - Tween 20 (1mL)
- 5% milk in TBST (make 100mL)
  - powdered milk (5g)
  - TBST to 100mL
- Proteinase K buffer 1 (make 10mL)
  - 100mM Tris-Cl pH 7.5 (1mL of 1M stock)
  - 10mM EDTA (200uL of 0.5M stock)
  - 50mM NaCl (100uL of 5M stock)
  - water to 10mL (8.7mL)
- Proteinase K buffer 2 (make 10mL)
  - 100mM Tris-Cl pH 7.5 (1mL of 1M stock)
  - 10mM EDTA (200uL of 0.5M stock)
  - 50mM NaCl (100uL of 5M stock)
  - 7M urea (4.2g)
  - water to 10mL

<span id="33-protocol"></span>

### 3.3 Protocol

Read this protocol before starting to make sure you are prepared for the steps as they come. All of the buffers should be cold (+4C). Pre-heat a Thermomixer to +70C before starting.

1. From the 100uL bead mix in Rinse buffer D, transfer 20uL to a fresh 2mL tube (**ImagingIp**).
2. Remove the remaining 80uL of supernatant from the beads and resuspend in 20uL of Rinse buffer D (**SampleIp**).
3. At this point, you should have 4 samples: SampleInput, SampleIp, ImagingInput, ImagingIp, each with 20uL of volume. Keep on ice.
4. For SDS-PAGE (you will have 2 gels, one for samples, one for imaging):
   1. To each of these samples, add 7.5uL of NuPAGE™ LDS Sample Buffer (4X) and 3uL of 1M DTT and pipette mix.
   2. Incubate the samples at +70C with mixing at 1,000rpm for 10-minutes.
   3. Prepare the gels and pre-run for 10-minutes at 150V.
   4. Load samples on the gel with 10uL of the PageRuler marker on each end, alternating samples with Diluted marker (10uL each lane). For samples, load the entire 30uL. Run at 150V for 75-minutes.
5. Perform the transfer:
   1. For the imaging gel, activate a PVDF membrane in methanol and transfer to 1X Transfer buffer.
   2. For the sample gel, transfer nitrocellulose membrane to 1X Transfer buffer.
   3. Assemble transfer stacks, from bottom to top (black side (negative) of stack holder on bottom): (negative) 1× sponge – 2× Whatman – gel – membrane – 2× Whatman – 1× sponge (positive).
   4. Transfer overnight at 30V.
   5. The next day, remove the sample gel membrane, rinse quickly once with DPBS, then wrap in Saran wrap and store at −20C.
6. To develop the imaging gel membrane:
   1. Block membrane in 5% milk in TBST at room temperature for 30-minutes.
   2. Probe with primary antibody at appropriate concentration (typically 0.2 μg/mL) in 5% milk in TBST, at room temperature for 1-hour.
   3. Wash three times with TBST, for 5-minutes each.
   4. Probe with secondary antibody: 1:4000 Rabbit TrueBlot HRP in 5% milk in TBST and incubate at room temperature for 1–3 hours.
   5. Wash three times with TBST, for 5-minutes each.
   6. Develop with ECL, 30-seconds to 5-minutes, and image with western blot film.
7. Cutting the sample gel membrane:
   1. Place membrane on clean glass/metal surface.
   2. Using a fresh razor blade, cut desired lane from the RBP band to a region ~75kDa above your target.
   3. Slice the membrane piece into ~1–2 mm pieces.
   4. Transfer slices to a 2mL tube on ice. Remember to also cut the same region from your SampleInput lane.
8. RNA extraction:
   1. To the membrane pieces, add 180uL of Proteinase K buffer 1 and 20uL of Proteinase K (20mg/mL). Incubate at +37C for 20-minutes in a ThermoMixer at 1,000rpm.
   2. Add 180uL of Proteinase K buffer 2 and 20uL of Proteinase K (20mg/mL) and incubate for an additional 20-minutes at +37C with mixing at 1,000rpm.
   3. Add 400uL of Acid phenol chloroform to the SampleInput tubes and 400uL of Phenol chloroform (non-acidic) to the SampleIp tubes and mix well. Incubate at +37C for 5-minutes.
   4. Transfer liquid (no membrane pieces) to a Phaselock gel (heavy) tube and incubate in ThermoMixer at 1,000 rpm, +37C for 5-minutes.
   5. Centrifuge at 13,000g for 15-minutes at room temperature.
   6. Transfer the aqueous (top) layer to a new 15 mL (or at least 3 mL volume) conical tube.
   7. Add 2 volumes RNA binding buffer from the RNA Clean and Concentrator kit (typically ~800uL).
   8. Add equal volume 100% ethanol and mix (typically ~1200uL).
   9. Transfer 750uL of mixed sample to a Zymo-Spin column.
   10. Centrifuge for 30-seconds at 12,000g and discard the flow-through.
   11. Repeat spins by reloading an additional 750uL volume until all sample has been spun through the column.
   12. Add 400uL of RNA Prep Buffer, centrifuge for 30-seconds at 12,000g, and discard the flow-through.
   13. Add 700uL of RNA Wash Buffer, centrifuge for 30-seconds at 12,000g, and discard the flow-through.
   14. Add 400uL of RNA Wash Buffer, centrifuge for 30-seconds at 12,000g, and discard the flow-through.
   15. Centrifuge for additional 2-minutes at 12,000g.
   16. Transfer column to a new 1.5mL tube, add 25uL of water to the column, incubate for 1-minute, and then centrifuge for 30-seconds at 12,000g.
   17. Samples can be stored at −80C.

<hr style="height:6pt; visibility:hidden;" />

<span id="4-phosphorylation-biotin-capture-reverse-transcription-and-linker-ligation"></span>

## 4. Phosphorylation, biotin capture, reverse transcription, and linker ligation

<span id="41-reagents-and-materials"></span>

### 4.1 Reagents and materials

- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- PCR microtubes (any vendor is fine)
- Benchtop centrifuge with holder for microcentrifuge tubes (multiple vendors)
- ThermoMixer with a 2mL block (Eppendorf)
- PCR Thermocycler (multiple vendors)
- RNaseZAP wipes (Thermo Scientific, CAT#AM9788)
- Dithiothreitol (Bio-Rad, CAT#1610611)
- PEG-8000 (Promega, CAT#V3011)
- QuickCIP (NEB, CAT#M0525L)
- T4 PNK (NEB, CAT#M0201L)
- T4 RNA Ligase 2, truncated KQ (NEB, CAT#M0373L)
- 10mM ATP (NEB, CAT#P0756S)
- Dynabeads MyOne Silane (Thermo Scientific, CAT#37002D)
- RLT buffer (Qiagen, CAT#79216)
- TURBO DNase, 2U/uL (Thermo Fisher, CAT#AM2238)
- RNaseIn, 40U/uL (Promega, CAT#N2511)
- 1M TrisCl pH 7.5 (Thermo Fisher, CAT#15567027)
- 5M NaCl (Thermo Scientific, CAT#AM9760G)
- 0.5M EDTA (Thermo Scientific, CAT#15575020)
- Dynabeads MyOne Streptavidin C1 (Thermo Scientific, CAT#65001)
- Absolute ethanol (wherever your institute purchases this from)
- NP-40 (Sigma, CAT#NP40)
- Exonuclease I, 20U/uL (E. coli) (NEB, CAT#M0293S) - comes with 10X Exo1 buffer
- 1N NaOH (Sigma, CAT#S2770-100ML)
- 1N HCl (Sigma, CAT#H9892-100ML)
- T4 RNA ligase 1 (NEB, CAT#M0437M)

<span id="42-solution-recipes"></span>

### 4.2 Solution recipes

- 50% (w/v) PEG-8000 - 12.5g in 25mL of water
- 0.2M of dithiothreitol (DTT) - 15mg in 500uL of water, prepare fresh and keep on ice
- 80% ethanol (10mL of ethanol in 40mL of water)
- 10% (v/v) NP-40 - 1mL in 9mL of water
- 2X PNK buffer 1 (make 1mL)
  - 100mM Tris-Cl pH 7.5 (100uL of 1M stock)
  - 20mM MgCl2 (40uL of 0.5M stock)
  - 2mM DTT (10uL of 200mM stock)
  - water to 1mL (850uL)
- 2X RNL buffer 1 (make 1mL)
  - 100mM Tris-Cl pH 7.5 (100uL of 1M stock)
  - 20mM MgCl2 (40uL of 0.5M stock)
  - 2mM DTT (10uL of 200mM stock)
  - 40% (w/v) PEG-8000 (800uL of 50% stock)
  - water to 1mL (50uL)
- Streptavidin solution A (make 10mL)
  - 100mM NaOH (1mL from 1N stock)
  - 50mM NaCl (100uL from 5M stock)
  - 0.1% NP-40 (100uL from 10% stock)
- Streptavidin solution B (make 10mL)
  - 100mM NaCl (200uL of 5M stock)
  - 0.1% NP-40 (100uL from 10% stock)
- 2X B&W buffer (make 10mL)
  - 10mM TrisCl pH 7.5 (100uL of 1M stock)
  - 1mM EDTA (20uL of 0.5M stock)
  - 2M NaCl (4mL of 5M stock)
  - 0.2% NP-40 (200uL of 10% stock)
- 1X B&W buffer (make 5mL) - 2.5mL of 2X B&W buffer with 2.5mL of water
- 10uM Ribo_RTPrimer_v4 - 10uL of 100uM stock in 90uL of water
- SuperScript™ IV Reverse Transcriptase (Thermo Scientific, CAT#18090050) - this includes 5X SSIV buffer and 0.1M DTT
- Deoxynucleotide (dNTP) Solution Mix, 10mM (NEB, CAT#N0447S)
- 2X RT master mix (make 10uL per sample)
  - 2X SSIV buffer (4uL of 5X stock)
  - 1mM dNTPs (1uL of 10mM stock)
  - 10mM DTT (1uL of 0.1M stock)
  - 4U/uL RNaseIn (1uL of 40U/uL stock)
  - 20U/uL SSIV (1uL of 200U/uL stock)
  - water (2uL)
- RNL buffer 2 (make 1mL)
  - 50mM Tris-Cl pH 7.5 (50uL of 1M stock)
  - 10mM MgCl2 (20uL of 0.5M stock)
  - 1mM DTT (5uL of 200mM stock)
  - 1mM ATP (100uL of 10mM stock)
  - 20% (v/v) PEG-8000 (400uL of 50% stock)
  - water to 1mL (425uL)
- 3' linker mix - mix equal parts of 40uM stocks of Clip_3DNALinker2_v4a and Clip_3DNALinker2_v4b

<span id="43-oligos"></span>

### 4.3 Oligos

- Ribo_3DNALinker_v4 (100nmol scale, RNase-free HPLC purified)
  - /5rApp/NNNGTCNNNTAGNNNAGATCGGAAGAGCACACGTCT/3ddC/
  - reconstitute to 20uM and aliquot. Store at -20C.
- Ribo_RTPrimer_v4 (100nmol scale, desalting purification)
  - AGACGTGTGCTCTTCCGATCT
  - reconstitute at 100uM. Store at -20C.
- Clip_3DNALinker2_v4a (100nmol scale, HPLC purified)
  - /5Phos/NNNGTANNNTCGNNNAGATCGGAAGAGCGTCGTG/3ddC/
  - reconsitute to 40uM and aliquot. Store at -20C.
- Clip_3DNALinker2_v4b (100nmol scale, HPLC purified)
  - /5Phos/NNNACTNNNGATNNNAGATCGGAAGAGCGTCGTG/3ddC/
  - reconsitute to 40uM and aliquot. Store at -20C.

<span id="44-protocol"></span>

### 4.4 Protocol

The starting point for this stage of the protocol is the 10uL purified RNA sample from above.

1. First we need to 3' dephosphorylate the SampleInput RNA:
   1. Add 25uL of 2X PNK buffer 1 to the input sample only and then add 2uL of QuickCIP and 1uL of T4 PNK (10 Units of each) and pipette mix. Incubate for 30-minutes at +37C.
   2. In a separate tube, rinse 20uL of MyONE Silane beads (per sample) with 500uL of RLT buffer. Discard the supernatant.
   3. Resuspend the beads in 365uL of RLT buffer and add to the input sample. Pipette mix.
   4. Add 10uL of 5M NaCl to the sample and pipette mix.
   5. Add 400uL of ethanol and rotate the tubes to mix for 15-minutes at room temperature (+21C).
   6. Place tubes on magnetic rack and discard the supernatant.
   7. Rinse the beads three times with 800uL of 80% ethanol. Discard supernatants to the waste.
   8. Add 40uL of water to the beads and incubate at room temperature for 5-minutes.
   9. Recover 20uL of this sample and store at -20C as a backup. Keep the other 20uL with the beads.
2. Now perform 3' adapter ligation of the SampleInput RNA:
   1. Add 25uL of 2X RNL buffer 1 to the bead sample, and then add 5uL of Ribo_3DNALinker_v4 followed by 1uL of T4 RNA Ligase 2 truncated KQ (200 Units). Pipette mix and incubate at room temperature for 4-hours with gentle rotation.
   2. Resuspend the beads in 365uL of RLT buffer and add to the input sample. Pipette mix.
   3. Add 10uL of 5M NaCl to the sample and pipette mix.
   4. Add 400uL of ethanol and rotate the tubes to mix for 15-minutes at room temperature (+21C).
   5. Place tubes on magnetic rack and discard the supernatant.
   6. Rinse the beads three times with 800uL of 80% ethanol. Discard supernatants to the waste.
   7. Add 10uL of water to the beads and incubate at room temperature for 5-minutes.
   8. Recover 8uL of the sample from the beads and keep at on ice or at -20C until reverse transcription.
3. SampleIp RNA can now be enriched on biotin beads to remove unligated fragments:
   1. Wash 10uL of Streptavidin C1 beads twice with 200uL of Streptavidin solution A, then 200uL of Streptavidin solution B. Discard the supernatants.
   2. Resuspend the beads in 25uL of 2X B&W buffer and add to the eluted SampleIp RNA. Incubate for 20-minutes at room temperature in a ThermoMixer with mixing at 1,000rpm.
   3. Was the beads three times with 200uL of 1X B&W buffer and twice with 200uL of Streptavidin solution B. Discard the supernatants.
   4. Resuspend the beads in 10uL of water and incubate the samples at +90C for 5-minutes in a Thermocycler with mixing at 1,000rpm.
   5. Recover 8uL of the SampleIp RNA to a fresh tube and proceed to reverse transcription.
4. To perform reverse transcription for SampleIp and SampleInput:
   1. In PCR tubes, add 2uL of 10uM Ribo_RTPrimer_v4, incubate at +70C for 5-minutes and then place on ice to cool.
   2. Add 10uL of the 2X RT master mix and pipette mix. Incubate in a Thermocycler at +55C for 30-minutes.
   3. Add 2.5uL of 10X Exo1 buffer followed by 2.5uL of Exonuclease I. Pipette mix and incubate at +37C for 15-minutes.
   4. Add 1uL of 0.5M EDTA to stop the reaction.
   5. Add 3uL of 1M NaOH and incubate at +70C in a Thermocycler for 12-minutes.
   6. Add 3uL of 1M HCl to neutralize the reaction.
   7. Magnetically separate 20uL of MyONE Silane beads per sample, and remove the supernatant.
   8. Rinse the beads once with 500uL of RLT buffer, and discard the supernatant.
   9. Reconstitute the beads in 370uL of RLT buffer and combine with the sample.
   10. Add 10uL of 5M NaCl to the sample and pipette mix.
   11. Add 400uL of ethanol and rotate the tubes to mix for 15-minutes at room temperature (+21C).
   12. Place tubes on magnetic rack and discard the supernatant.
   13. Rinse the beads three times with 800uL of 80% ethanol. Discard supernatants to the waste.
5. To ligate linkers to all samples:
    1. Reconstitute the rinsed beads in 45uL of RNL buffer 2. Add 5uL of 3' linker mix and 2uL of T4 RNA ligase 1 (60 Units). Pipette mix and incubate at room temperature overnight with gentle agitation.
    2. Reconstitute the beads in 340uL of RLT buffer and combine with the sample.
    3. Add 10uL of 5M NaCl to the sample and pipette mix.
    4. Add 400uL of ethanol and rotate the tubes to mix for 15-minutes at room temperature (+21C).
    5. Place tubes on magnetic rack and discard the supernatant.
    6. Rinse the beads three times with 800uL of 80% ethanol. Discard supernatants to the waste.
    7. Add 25uL of water to the beads and incubate at room temperature for 5-minutes.
    8. Recover the samples and store at -20C until PCR library construction.

<hr style="height:6pt; visibility:hidden;" />

<span id="5-library-amplification-and-size-selection"></span>

## 5. Library amplification and size selection

<span id="51-reagents-and-materials"></span>

### 5.1 Reagents and materials

- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- PCR microtubes (any vendor is fine)
- Benchtop centrifuge with holder for microcentrifuge tubes (multiple vendors)
- Centrifuge with buckets for microwell plates (multiple vendors)
- ThermoMixer with a 2mL block (Eppendorf)
- PCR Thermocycler (multiple vendors)
- SYBR Select Master Mix (Thermo Scientific, CAT#4472908)
- NEBNext Ultra II Q5 Master Mix (NEB, CAT#M0544L)
- MicroAmp Optical 384-Well Reaction Plate with Barcode (Thermo Scientific, CAT#4309849)
- MicroAmp Optical Adhesive Film (Thermo Scientific, CAT#4360954)
- Monarch PCR & DNA Cleanup Kit (5 μg) (NEB, CAT#T1030S)
- SYBR Gold Nucleic Acid Gel Stain (10,000X Concentrate in DMSO) (Thermo Scientific, CAT#S11494)
- Novex Hi-Density TBE Sample Buffer (5X) (Thermo Scientific, CAT#LC6678)
- Novex TBE Running Buffer (5X) (Thermo Scientific, CAT#LC6675)
- Novex TBE Gels, 6%, 10 well (Thermo Scientific, CAT#EC6265BOX)
- pBR322 DNA-MspI Digest (NEB, CAT#N3032S)


<span id="52-solution-recipes"></span>

### 5.2 Solution recipes

- qPCR primer mix - 10uL of PCR_P5Primer_v4, 10uL of PCR_P7Primer_v4i1, 80uL water
- Gel ladder - mix 5uL of pBR322 DNA-MspI Digest, 5uL of Novex Hi-Density TBE Sample Buffer, and 15uL of water

<span id="53-oligos"></span>

### 5.3 Oligos

- PCR_P5Primer_v4 (4nmol scale, Ultramer)
  - /5Phos/AATGATACGGCGACCACCGAGATCTACACTCTTTCCCTACACGACGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i1 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATCGTGATGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i2 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATACATCGGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i3 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATGCCTAAGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i4 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATTGGTCAGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i5 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATCACTGTGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i6 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATATTGGCGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i7 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATGATCTGGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i8 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATTCAAGTGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i9 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATCTGATCGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i10 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATAAGCTAGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i11 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATGTAGCCGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.
- PCR_P7Primer_v4i12 (4nmol scale, Ultramer)
  - /5Phos/CAAGCAGAAGACGGCATACGAGATTACAAGGTGACTGGAGTTCAGACGTGTGCTCTTCCGATC*T
  - reconstitute to 100uM and store at -20C.

<span id="54-protocol"></span>

### 5.4 Protocol

The starting point for this stage of the protocol is the 25uL purified cDNA samples from above.

1. First, determine the amplification levels of the different libraries:
   1. Combine 1uL of RNA sample, 1uL of qPCR primer mix, 8uL of water, and 10uL of SYBR Select master mix and pipette mix.
   2. Add sample to 384-well qPCR plate and seal with optical adhesive film. Centrifuge at 250g for 5-minutes.
   3. Analyze on an RT-qPCR instrument with using the cycle settings:
      1. +95C for 10-seconds
      2. 55-cycles of:
      3. +95C for 15-seconds
      4. +60C for 30-seconds
      5. +72C for 30-seconds
      6. Melt curve analysis
      7. +4C forever
   4. Note the Ct values for the samples (SampleIp optimal cycles = Ct - 4, SampleInput optimal cycles = Ct - 1).
2. Perform a test amplification to see that the insert size is correct:
   1. In a PCR tube, combine 1uL of sample, 1uL of 10uM qPCR primer mix, 8uL of water, and 10uL of Q5 PCR master mix and pipette mix.
   2. Amplify in a Thermocycler with the cycle settings:
      1. +98C for 30-seconds
      2. X-cycles of:
      3. +98C for 10-seconds
      4. +65C for 75-seconds
      5. +65C for 5-minutes
      6. +4C forever
   3. Add 5uL of 5X Novex Hi-Density TBE Sample Buffer to the PCR reaction and run on a TBE gel.
   4. Stain the gel in SYBR Gold and visualize the result.
3. Perform library amplification (SampleIp optimal cycles = Ct - 6, SampleInput optimal cycles = Ct - 2).:
   1. In a PCR tube, combine 12.5uL of sample, 2.5uL of 10uM primer mix (with your barcode of interest), and 12.5uL of Q5 PCR master mix and pipette mix.
   2. Amplify in a Thermocycler with the cycle settings:
      1. +98C for 30-seconds
      2. X-cycles of:
      3. +98C for 10-seconds
      4. +65C for 75-seconds
      5. +65C for 5-minutes
      6. +4C forever
   3. Purify the PCR product with a Monarch PCR purification kit and elute in 20uL of water.
   4. Add 5uL of 5X Novex Hi-Density TBE Sample Buffer to the PCR reaction and run on a TBE gel. Use 5uL of the Gel ladder per lane as a marker.
   5. Stain the gel in SYBR Gold and visualize the result.



