# EV proteome analysis with mass spectrometry <!-- omit in toc -->

This document describes an end-to-end protocol for analysis of the proteome of EV samples prepared via ultracentrifugation.

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [1. Protein digestion](#1-protein-digestion)
  - [1.1 Reagents and materials](#11-reagents-and-materials)
  - [1.2 Solution recipes](#12-solution-recipes)
  - [1.3 Protocol](#13-protocol)
- [2. Peptide cleanup](#2-peptide-cleanup)
  - [2.1 Reagents and materials](#21-reagents-and-materials)
  - [2.2 Solution recipes](#22-solution-recipes)
  - [2.3 Protocol](#23-protocol)
- [Notes](#notes)

<hr style="height:6pt; visibility:hidden;" />

<span id="1-protein-digestion"></span>

## 1. Protein digestion

This protocol is based on a direct trypsin approach and assumes a starting point of a pellet following ultracentrifugation.

<span id="11-reagents-and-materials"></span>

### 1.1 Reagents and materials

- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- Rapid Trypsin kit (Promega, CAT#VA1061)
- Benzonase nuclease, 25U/uL (Sigma, CAT#70664-3)
- Clean water (Thermo Scientific, CAT#10977023)
- Trifluoroacetic acid (TFA), HPLC grade (CAT#85183, Thermo Scientific)
- Thermomixer with 2mL tube block (Eppendorf)

<span id="12-solution-recipes"></span>

### 1.2 Solution recipes

- Digestion buffer (need 200uL per sample, recipe is for 1 sample)(see [**Note 1**](#note1))
  - 50uL of clean water
  - 150uL of Rapid Digestion Buffer (part of the Rapid trypsin kit, pre-warm to +37C)
  - 1uL of trypsin (0.5ug/uL stock concentration in kit provided reconstitution buffer)
- Acidification solution (10% TFA, v/v)

<span id="13-protocol"></span>

### 1.3 Protocol

1. Preheat Thermomixer to +70C with the 2mL block, set to 1-hour with 1,000rpm mixing.
2. To the prepared EV pellet, add 200uL of Digestion buffer and pipette mix to reconstitute. Transfer to fresh 2mL tube.
3. Place 2mL tubes in the pre-heated Thermomixer and digest for 1-hour with mixing.
4. After incubation, add 20uL of Acidification solution and vortex briefly.
5. Samples are now ready for clean-up prior to MS analysis and can be stored at -20C or -80C indefinitely.

<hr style="height:6pt; visibility:hidden;" />

<span id="2-peptide-cleanup"></span>

## 2. Peptide cleanup

This protocol is based on the use of 96-well SlitPlates, but you can use any standard C18 peptide cleanup procedure you are familiar with.

<span id="21-reagents-and-materials"></span>

### 2.1 Reagents and materials

- C18 SlitPlates (CAT#S2C18, Glygen Corp.)
- Acetonitrile, HPLC grade (CAT#51101, Thermo Scientific)
- Water, HPLC grade (CAT#51140, Thermo Scientific)
- Trifluoroacetic acid, HPLC grade (CAT#85183, Thermo Scientific)
- Formic acid, HPLC grade (CAT#85178, Thermo Scientific)
- 1.5mL snap-lock tubes (CAT#05-402-25, Thermo Scientific)
- Benchtop centrifuge with plate-holder rotor (multiple vendors)

<span id="22-solution-recipes"></span>

### 2.2 Solution recipes

- Buffer A - 0.1% trifluoroacetic acid (TFA) in acetonitrile
- Buffer B - 0.1% TFA in water
- Rinse buffer - 0.1% formic acid in water
- Elution buffer - 0.1% formic acid in 60% acetonitrile

<span id="23-protocol"></span>

### 2.3 Protocol

Prior to processing, ensure that your sample contains less than 5% (v/v) of acetonitrile or other similar solvents, otherwise your sample will not bind efficiently. The sample volume needs to be below 200uL to load on the SlitPlate. Only uncover wells on the SlitPlate that you intend to use.

1. Using a pipette, add 160uL of Buffer A to the SlitPlate wells and centrifuge at 250g for 2-minutes. Empty the collection plate to the waste.
2. Optional: repeat the previous step one additional time for a total of 2 rinses.
3. Add 160uL of Buffer B to the SlitPlate wells and centrifuge at 250g for 2-minutes (see [**Note 2**](#note2)). Empty the collection plate to the waste.
4. Optional: repeat the previous step one additional time for a total of 2 rinses.
5. Add the peptide samples to the SlitPlate wells and centrifuge at 250g for 5-minutes. Empty the collection plate to the waste.
6. Add 160uL of Rinse buffer to the SlitPlate wells and centrifuge at 250g for 2-minutes. Empty the collection plate to the waste.
7. Optional: repeat the previous step two additional times for a total of 3 rinses. After the final rinse, make sure to empty all liquid from the collection plate.
8. Add 160uL of Elution buffer to the SlitPlate wells and centrifuge at 250g for 5-minutes (see [**Note 3**](#note3)).
9. Transfer the elution to fresh 1.5mL tubes.
10. Concentrate the sample by evaporation (see [**Note 4**](#note4)).

<hr style="height:6pt; visibility:hidden;" />

<span id="notes"></span>

## Notes

<span id="note1"></span>

**Note 1** - If you think you need more volume for the pellet, scale accordingly. With this kit, trypsin will come as a lyophilized material. Reconstitute at a concentration of 0.5ug/uL in the provided reconstitution solution and aliquot to 2.5ug fractions to be stored at -80C.

<span id="note2"></span>

**Note 2** - Pay attention to the wells after the spin as some may flow slower than others. If this is the case, add time to the spin rather than increasing the speed of the spin.

<span id="note3"></span>

**Note 3** - You can also elute directly into a 96-well plate to be put in a nanoLC autosampler. In this case, you will need to use a smaller elution volume (around 100uL) to avoid overflowing of the collection wells.

<span id="note4"></span>

**Note 4** - There are multiple methods you can use here, such as a SpeedVac centrifuge or a lyophilizer. If using a lyophilizer, poke a small hole in the cap of the 1.5mL tube containing the peptide sample and freeze it at -80C prior to concentration.
