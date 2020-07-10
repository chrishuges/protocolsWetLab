# Preparing a BSA standard for MS <!-- omit in toc -->

This document describes a protocol for preparing a bovine serum albumin (BSA) protein digest for use as a standard to measure chromatography and mass spectrometer performance. This protocol was designed to optimize ease of use and could theoretically be applied to the preparation of other protein standards, if desired.

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [Reagents and materials](#reagents-and-materials)
- [Solution recipes](#solution-recipes)
- [Protocol](#protocol)
- [Notes](#notes)

<hr style="height:6pt; visibility:hidden;" />

<span id="reagents-and-materials"></span>

## Reagents and materials

- 1.5mL or 2.0mL Safe-Lock tubes (Fisher Scientific, CAT#05-402-25 or CAT#05-402-7)
- Bovine serum albumin, fraction V (Sigma, CAT#A2153)
- 1M HEPES pH 7.3 (Thermo Scientific, CAT#BP299)
- Guanidine hydrochloride (Sigma, CAT#G3272)
- Dithiothreitol (Bio-Rad, CAT#1610611)
- Chloroacetamide (Sigma, CAT#C0267)
- Trypsin/rLysC mix (Promega, CAT#V5073)
- Thermomixer capable of holding 1.5mL or 2.0mL tubes
- Lyophilizer or SpeedVac centrifuge (multiple vendors)
- C18 TopTips (CAT#TT3C18, Glygen Corp.)
- Acetonitrile, HPLC grade (CAT#51101, Thermo Scientific)
- Water, HPLC grade (CAT#51140, Thermo Scientific)
- Trifluoroacetic acid, HPLC grade (CAT#85183, Thermo Scientific)
- Formic acid, HPLC grade (CAT#85178, Thermo Scientific)
- Benchtop centrifuge (capable of holding 1.5mL or 2mL microfuge tubes)

<span id="solution-recipes"></span>

## Solution recipes

- 0.2M of dithiothreitol (DTT) - 15mg in 500uL of 1M HEPES, pH 7.3, prepare fresh and keep on ice
- 0.4M of chloroacetamide (CAA) - 18mg in 500uL of 1M HEPES, pH 7.3, prepare fresh and keep on ice
- Solubilization solution (need 1mL)
  - 4M guanidine hydrochloride (382mg)
  - 100mM HEPES pH 7.3 (100uL of 1M stock)
  - 10mM DTT (50uL of 0.2M stock)
  - water to 1mL (650uL should be enough here with volume adjustment due to the guanidine)
- 10% (v/v) trifluoroacetic acid (TFA) - 100uL in 900uL of water
- Buffer A - 0.1% trifluoroacetic acid (TFA) in acetonitrile
- Buffer B - 0.1% TFA in water
- Rinse Buffer - 0.1% formic acid in water
- Elution Buffer - 0.1% formic acid in 60% acetonitrile

<span id="protocol"></span>

## Protocol

1. Weigh out 20mg of BSA in a 2mL tube.
2. Add 1mL of Solubilization solution and mix to dissolve the BSA (see [**Note 1**](#note1)).
3. Heat the mixture at +65C for 15-minutes with shaking at 1,000rpm in a Thermomixer.
4. Let the tube cool to room temperature and add 100uL of CAA (from 0.4M stock). Incubate at room temperature (+21C) for 30-minutes in the dark.
5. Add 50uL of DTT (from 0.2M stock) to quench, and incubate at room temperature for 10-minutes.
6. At this point, the protein sample can be aliquoted (~2mg of BSA in 100uL) to 1.5mL tubes and frozen at -80C for later preparation as needed.
7. To proceed with digestion:
   1. Thaw an aliquot and split it into two individual 2mL tubes (50uL each).
   2. Prepare 20ug of trypsin by reconstituting a vial in 1000uL of 0.1M HEPES, pH 7.3 (see [**Note 2**](#note2)).
   3. Add 450uL of trypsin (10ug) (there may be some precipitation at this point...it is ok).
   4. Digest at +37C overnight with mixing at 1000rpm in a Thermomixer.
   5. The next day, acidify by addition of 10% TFA to an approximate final concentration of 1%.
   6. Centrifuge the digest at 20,000g for 5-minutes and recover the supernatant to a fresh 2mL tube. The digest can be frozen at -80C at this stage indefinitely.
8. To clean-up the digestion for downstream analysis:
   1. Using a pipette, add 600uL of Buffer A to a 1mL TopTip and elute the added liquid to the waste at a flow rate of 1 drop per second (see [**Note 3**](#note3)).
   2. Repeat the previous step one additional time for a total of 2 rinses.
   3. Add 600uL of Buffer B to the TopTip and elute to waste as above.
   4. Repeat the previous step one additional time for a total of 2 rinses.
   5. Add the sample to the TopTip and elute to waste as above.
   6. Rinse the loaded TopTip with 600uL of Rinse Buffer.
   7. Repeat the previous step two additional times for a total of 3 rinses.
   8. Elute the peptides with 600uL of the Elution Buffer into a fresh 2mL tube.
   9. Repeat the previous step one additional time for a total of 2 elutions.
   10. Poke an approximately 1cm diameter hole in the lid of the elution tube and transfer it to the -80C freezer.
9. Turn on the lyophilizer and allow the vaccuum chamber to chill.
10. Add the frozen samples to the lyophilizer and turn on the vaccuum. Leave overnight, or for about 12-hours.
11. Remove the sample tube from the lyophilizer (there should be only white material remaining), and reconstitute in 1000uL of water (see [**Note 4**](#note4)). This stock can be frozen at -80C indefinitely.

<hr style="height:6pt; visibility:hidden;" />

<span id="notes"></span>

## Notes

<span id="note1"></span>

**Note 1** - Optionally, you can add the mixture to a Lysing Matrix Y tube and disrupt on the FastPrep using a standard protocol (6M/s, 30 second cycles, 2 cycles). This can help homogenize the solution.

 <span id="note2"></span>

**Note 2** - You could substitute whatever buffer you want here (e.g. ammonium bicarbonate).

<span id="note3"></span>

**Note 3** - When a TopTip is first used, there will generally be some beads stuck to the side of the upper TopTip walls. Try to rinse the beads on the upper TopTip wall to join the rest of the bead bed.

<span id="note4"></span>

**Note 4** - For HPLC analysis, I take 100uL of this stock, dilute to 200uL total, and inject 50uL. For MS analysis, I take 10uL of this stock, dilute it to 200uL, and inject 2uL.
