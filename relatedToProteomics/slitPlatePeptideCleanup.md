# Peptide clean-up using C18 SlitPlates <!-- omit in toc -->

This protocol was last updated - May 19, 2020 by Chris Hughes.

This protocol describes clean-up of peptide samples using C18 SlitPlates prior to downstream processing, such as mass spectrometry analysis. The described protocol uses 96-well SlitPlates, but can be scaled for 384-well plates.

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [Reagents and materials](#reagents-and-materials)
- [Solution recipes](#solution-recipes)
- [Protocol](#protocol)
- [Notes](#notes)

<hr style="height:6pt; visibility:hidden;" />

## Reagents and materials

- C18 SlitPlates (CAT#S2C18, Glygen Corp.)
- Acetonitrile, HPLC grade (CAT#51101, Thermo Scientific)
- Water, HPLC grade (CAT#51140, Thermo Scientific)
- Trifluoroacetic acid, HPLC grade (CAT#85183, Thermo Scientific)
- Formic acid, HPLC grade (CAT#85178, Thermo Scientific)
- 1.5mL snap-lock tubes (CAT#05-402-25, Thermo Scientific)
- Benchtop centrifuge with plate-holder rotor (multiple vendors)

## Solution recipes

- Buffer A - 0.1% trifluoroacetic acid (TFA) in acetonitrile
- Buffer B - 0.1% TFA in water
- Rinse buffer - 0.1% formic acid in water
- Elution buffer - 0.1% formic acid in 60% acetonitrile

## Protocol

Prior to processing, ensure that your sample contains less than 5% (v/v) of acetonitrile or other similar solvents, otherwise your sample will not bind efficiently. The sample volume needs to be below 200uL to load on the SlitPlate. Only uncover wells on the SlitPlate that you intend to use.

1. Using a pipette, add 180uL of Buffer A to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
2. Repeat the previous step one additional time for a total of 2 rinses.
3. Add 180uL of Buffer B to the SlitPlate wells and centrifuge at 250g for 3-minutes (see [**Note 1**](#note1)). Empty the collection plate to the waste.
4. Repeat the previous step one additional time for a total of 2 rinses.
5. Add the peptide samples to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
6. Add 180uL of Rinse buffer to the SlitPlate wells and centrifuge at 250g for 3-minutes. Empty the collection plate to the waste.
7. Repeat the previous step two additional times for a total of 3 rinses. After the final rinse, make sure to empty all liquid from the collection plate.
8. Add 180uL of Elution buffer to the SlitPlate wells and centrifuge at 250g for 3-minutes (see [**Note 2**](#note2)).
9. Transfer the elution to fresh 1.5mL tubes.
10. Concentrate the sample by evaporation (see [**Note 3**](#note3)).

<hr style="height:6pt; visibility:hidden;" />

## Notes

<span id="note1"></span>

**Note 1** - Pay attention to the wells after the spin as some may flow slower than others. If this is the case, add time to the spin rather than increasing the speed of the spin.

<span id="note2"></span>

**Note 2** - You can also elute directly into a 96-well plate to be put in a nanoLC autosampler. In this case, you will need to use a smaller elution volume (around 100uL) to avoid overflowing of the collection wells.

<span id="note3"></span>

**Note 3** - There are multiple methods you can use here, such as a SpeedVac centrifuge or a lyophilizer. If using a lyophilizer, poke a small hole in the cap of the 1.5mL tube containing the peptide sample and freeze it at -80C prior to concentration.
