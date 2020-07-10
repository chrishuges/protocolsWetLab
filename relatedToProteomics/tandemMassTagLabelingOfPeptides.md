# Tandem mass tag labeling of peptides <!-- omit in toc -->

This document describes how to chemically label peptides with tandem mass tags (TMT). TMT is a barcoding technique that allows for samples to be multiplexed during mass spectrometry analysis. This protocol is based on the use of the 5mg TMT kits in 11-plex format, but is applicable to any TMT kit without modification.

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [Reagents and materials](#reagents-and-materials)
- [Solution recipes](#solution-recipes)
- [Protocol](#protocol)
- [Notes](#notes)

<hr style="height:6pt; visibility:hidden;" />

<span id="reagents-and-materials"></span>

## Reagents and materials

- TMT 11-plex kit, 5mg per label (Thermo Scientific, CAT#A34808)
- Acetonitrile, HPLC grade (Thermo Scientific, CAT#51101)
- Glycine (Thermo Scientific, CAT#15527013)
- RNA clean water (Thermo Fisher, CAT#10977023)
- 1.5mL or 2.0mL Safe-Lock tubes (Thermo Scientific, CAT#05-402-25 or CAT#05-402-7)
- Benchtop centrifuge (capable of holding 1.5mL or 2mL microfuge tubes)

<span id="solution-recipes"></span>

## Solution recipes

- 1M glycine (750mg in 10mL of water)

<span id="protocol"></span>

## Protocol

The assumed starting point for this protocol is a mixture of peptides in aqueous solution. The pH should be around 8, and the solution should be free of other primary amines (e.g. no Tris buffer, no ammonium bicarbonate). The assumed volume of the peptide solution is around 100uL, based on previous processing by SP3. If you are using larger volumes, you may want to scale up the amount of TMT label you are using. I generally aim to end up with a final TMT:peptide (ug:ug) ratio of 4:1.

1. Prepare the TMT label stocks:
   1. Spin the TMT label tubes at 12,000g for 2-minutes.
   2. Add 500uL of acetonitrile to each label and vortex to dissolve the powder (final concentration of label is 10ug/uL)(see [**Note 1**](#note1)).
2. To a protein digest prepared from 100ug of protein previously processed with SP3, add 20uL of TMT label (2:1 ratio) and pipette mix followed by a brief vortex (see [**Note 2**](#note2)).
3. Incubate the tubes at room temperature (+21C) for 30-minutes.
4. After incubation, add an addition 20uL of TMT label to the tubes and vortex briefly.
5. Incubate the tubes at room temperature for 30-minutes.
6. Add 20uL of 1M glycine to the tubes and vortex.
7. The samples are now labeled and my be stored at -80C indefinitely (see [**Note 3**](#note3)).

<span id="notes"></span>

## Notes

<span id="note1"></span>

**Note 1** - For short or long term storage of the reconstituted TMT labels, you should close the lid and wrap it in parafilm to that no air will enter the tube. The tubes should then be stored at -80C. Tubes stored in this format can be freeze-thawed numerous times without a decrease in label performance. The labels can also be aliquoted and stored in the same manner if desired.

<span id="note2"></span>

**Note 2** - Pay attention to your labeling layout to avoid interference between channels. For example, for a 9 sample experiment where you have 3 conditions, each in triplicate, lay your samples out in the format:

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

<span id="note3"></span>

**Note 3** - If you plan to proceed to downstream analysis by HPLC fractionation or mass spectrometry, it is important to concentrate your samples to reduce the overall levels of added solvent. This can be done using a SpeedVac or lyophilizer, for example. TMT labeled samples can be combined and concentrated as a single mixture, or as separate tubes and combined during reconstitution.
