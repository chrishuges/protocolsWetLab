# In gel digestion for protein identification <!-- omit in toc -->

This document describes a protocol for SDS-PAGE separation of a protein sample, extraction, digestion, and mass spectrometry analysis for identification. Although the protocol mainly describes extraction of a single protein band, it could also be used for extraction and preparation of multiple bands from a single lane. This protocol starts after the gel has been run and in theory should be compatible with virtually any SDS-PAGE gel.

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
- Acetic acid (Sigma, CAT#A6283)
- Brilliant blue (Sigma, CAT#B7920)
- Ammonium bicabonate (Sigma, CAT#A6141)
- Dithiothreitol (Bio-Rad, CAT#1610611)
- Chloroacetamide (Sigma, CAT#C0267)
- Trypsin/rLysC mix (Promega, CAT#V5073)
- C18 TopTips (CAT#TT3C18, Glygen Corp.)
- Trifluoroacetic acid, HPLC grade (CAT#85183, Thermo Scientific)
- Formic acid, HPLC grade (CAT#85178, Thermo Scientific)
- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- Thermomixer capable of holding 1.5mL or 2.0mL tubes (Eppendorf)
- Dimethylsulfoxide (Sigma, CAT#D8418)
- Benchtop centrifuge (capable of holding 1.5mL or 2mL microfuge tubes)
- Sonicating water bath (optional)
- Razor blade (or some sort of clean cutting tool)
- Small, clean glass plate (this is useful for cutting the gel on)

<span id="solution-recipes"></span>

## Solution recipes

- Gel fixing solution (make 500mL)
  - Methanol - 250mL
  - Water - 200mL
  - Acetic acid - 50mL
- Gel destaining solution (make 500mL)
  - Methanol - 225mL
  - Water - 225mL
  - Acetic acid - 50mL
- Coomassie concentrated solution
  - Methanol - 30mL
  - Acetic acid - 6mL
  - Brilliant blue - 1.2g
- Gel staining solution (make 500mL)
  - Methanol - 250mL
  - Water - 200mL
  - Acetic acid - 50mL
- Gel piece destaining solution (make 50mL)
  - 100mM ammonium bicarbonate (ABC) - 395mg
  - 20% (v/v) acetonitrile - 10mL
  - Water to 50mL - 40mL
- 100mM ABC - 395mg in 50mL of water
- 0.2M of dithiothreitol (DTT) - 15mg in 500uL of 1M HEPES, pH 7.3, prepare fresh and keep on ice
- 0.4M of chloroacetamide (CAA) - 18mg in 500uL of 1M HEPES, pH 7.3, prepare fresh and keep on ice
- 0.02M of dithiothreitol (DTT) - 100uL of 0.2M stock in 900uL of water, prepare fresh and keep on ice
- 0.04M of chloroacetamide (CAA) - 100uL of 0.4M stock in 900uL of water, prepare fresh and keep on ice
- 5% formic acid - 500uL of formic acid in 10mL of water
- Buffer A - 0.1% trifluoroacetic acid (TFA) in acetonitrile
- Buffer B - 0.1% TFA in water
- Rinse Buffer - 0.1% formic acid in water
- Elution Buffer - 0.1% formic acid in 60% acetonitrile
- 1% formic acid with 1% DMSO - 10uL of formic acid, 10uL of DMSO, and 80uL of water

<span id="protocol"></span>

## Protocol

This protocol generally takes 2-3 days. I tried to break it up into major sections based on this.

1. For staining of the gel:
   1. Remove gel from glass plates and place carefully in a container with gel fixing solution (enough to cover the gel).
   2. Incubate the gel in fixing solution on a rotary mixer for 30-minutes and discard the fixing solution afterwards.
   3. Add gel staining solution (enough to cover the gel) and stain the gel for 30-minutes and discard the staining solution afterwards.
   4. Add gel destaining solution and shake until no visible background remains (2-3 hours). The destaining can be accelerated by changing the destain liquid frequently, or adding a folded up KimWipe to the container.
   5. Keep the gel in fixing solution for long term storage at this stage if desired.
2. To prepare gel bands for extraction and perform digestion:
   1. Prepare sufficient tubes for the number of gel bands you would like to cut out and add 200uL of the gel piece destain solution to each.
   2. Place the gel on cutting surface (such as a glass plate) and cut out your band of interest using a clean razor blade.
   3. Cut the extracted gel piece into small cubes (~1mm) and insert into the tube with gel piece destain solution in it.
   4. Destain the gel pieces until no blue remains! This process can be accelerated by changing the gel piece destain solution frequently.
   5. Remove and discard the destain and add 500uL of acetonitrile. Mix well by vortexing.
   6. Once the gel pieces have turned completely white, discard the acetonitrile.
   7. Add 50uL of DTT from the 0.02M stock to the gel pieces (or enough to cover the gel pieces) and incubate for 30-minutes at room temperature (+21C).
   8. Remove and discard any excess liquid and add 50uL of CAA from the 0.04M stock to the gel pieces (or the same volume that was added for DTT) and incubate for 30-minutes at room temperature in the dark.
   9. Discard any excess liquid in the tubes and add 500uL of acetonitrile and mix until the gel pieces are completely white.
   10. Discard the acetonitrile and add 200uL of 100mM ABC and mix until the gel pieces are clear again.
   11. Discard the excess ABC solution from the tubes and add 500uL of acetonitrile and mix until the gel pieces are completely white.
   12. Discard the excess acetonitrile.
   13. Prepare a trypsin digestion solution in 100mM ABC such that each gel tube will receive enough trypsin to digest your protein (see [**Note 1**](#note1)).
   14. Add 50uL of the digestion solution to the tubes (or enough to cover the gel pieces) and incubate for 10-minutes at room temperature.
   15. Add enough 100mM ABC to ensure the gel pieces are completely immersed in liquid and incubate overnight at +37C in a Thermomixer with mixing at 1,000rpm.
3. To extract the generated peptides from the gel pieces:
   1. Spin digest tubes for 1-minute at 10,000g and transfer the liquid to a fresh labeled tube for each sample.
   2. Add 100uL of 5% formic acid to the tubes and sonicate in a water bath for 10-minutes (see [**Note 2**](#note2)).
   3. Spin the tubes for 1-minute at 10,000g and transfer the liquid to the tubes containing the other material for the sample.
   4. Repeat the previous two steps one addition time for a total of 2 extractions with 5% formic acid.
   5. Add 200uL of acetonitrile to the tubes and sonicate in a water bath for 10-minutes.
   6. Spin the tubes for 1-minute at 10,000g and transfer the liquid to the tubes containing the other material for the sample.
   7. Poke an approximately 1cm diameter hole in the lid of each sample tube and transfer the tubes to the -80C freezer.
   8. Turn on the lyophilizer and allow the vaccuum chamber to chill.
   9. Add the frozen samples to the lyophilizer and turn on the vaccuum. Leave for about 4 to 6-hours.
   10. Reconstitute the dried samples in 100uL of Buffer B.
4. To desalt samples prior to mass spectrometry analysis (see [**Note 3**](#note3)):
    1. Using a pipette, add 100uL of Buffer A to the TopTip and elute the added liquid to the waste at a flow rate of 1 drop per second (see [**Note 4**](#note4)).
    2. Repeat the previous step one additional time for a total of 2 rinses.
    3. Add 600uL of Buffer B to the TopTip and elute to waste as above.
    4. Repeat the previous step one additional time for a total of 2 rinses.
    5. Add the peptide sample to the TopTip and elute to waste as above.
    6. Rinse the loaded TopTip with 600uL of Rinse Buffer.
    7. Repeat the previous step two additional times for a total of 3 rinses.
    8. Elute the peptides with 600uL of the Elution Buffer into a fresh 1.5mL tube.
    9. Repeat the previous step one additional time for a total of 2 elutions.
    10. Poke an approximately 1cm diameter hole in the lid of each sample tube and transfer the tubes to the -80C freezer.
    11. Turn on the lyophilizer and allow the vaccuum chamber to chill.
    12. Add the frozen samples to the lyophilizer and turn on the vaccuum. Leave for about 4 to 6-hours, or overnight.
    13. Once the fractions have reached dryness, add 20uL of the 1% formic acid, 1% DMSO solution. Do not try to pipette mix.
    14. Vortex the tubes for 10-seconds and then centrifuge for 2-minutes at 12,000g.
    15. Repeat the previous step one additional time.
    16. Samples can be frozen at this stage at -80C indefinitely.
5. Samples can now be analyzed by mass spectrometry using your method of choice.

<hr style="height:6pt; visibility:hidden;" />

## Notes

<span id="note1"></span>

**Note 1** - I generally aim to have a trypsin:protein, ug:ug ratio of around 1:100, depending on the volume. For a larger volume from a big gel piece, I would likely scale this down to a 1:25 ratio. But these are personal preferences and digestion should be efficient at the values you would typically use in your lab.

<span id="note2"></span>

**Note 2** - If you don't have a sonicating bath, you can just vortex the tubes periodically.

<span id="note3"></span>

**Note 3** - If you have many samples to process, you can also use a SlitPlate here. A protocol for SlitPlate processing can be found on [this website](https://github.com/chrishuges/wetLabProtocols/tree/master/relatedToProteomics).

<span id="note4"></span>

**Note 4** - When a TopTip is first used, there will generally be some beads stuck to the side of the upper TopTip walls. Try to rinse the beads on the upper TopTip wall to join the rest of the bead bed.
