# Cleanup of protein mixtures using SP3 <!-- omit in toc -->

This protocol was last updated - May 11, 2020 by Chris Hughes.

This document describes how to perform SP3 on a prepared protein mixture that contains contaminants you would like to remove (e.g. detergents). The described protocol includes information of directly eluting proteins, or digestion with trypsin as the final elution step from the beads. This protocol is described based on the use of 100ug of input lysate, but the protocol can be scaled for any amount of input material. Refer to the Nature Protocols paper on SP3 for considerations related to scaling volumes or bead amounts when you use different amounts of input material (PMID: 30464214).

<hr style="height:6pt; visibility:hidden;" />

## Quick links <!-- omit in toc -->

- [Reagents and materials](#reagents-and-materials)
- [Solution recipes](#solution-recipes)
- [Protocol](#protocol)
- [Notes](#notes)

<hr style="height:6pt; visibility:hidden;" />

<span id="reagents-and-materials"></span>

## Reagents and materials

- 1M HEPES pH 7.3 (Thermo Scientific, CAT#BP299)
- Ethanol, absolute (whatever vendor sells this to your lab)
- SP3 beads (Thermo Scientific, CAT#65152105050250, CAT#45152105050250) (see [**Note 1**](#note1))
- Trypsin/rLysC mix (Promega, CAT#V5073)
- 1.5mL or 2.0mL Safe-Lock tubes (Fisher Scientific, CAT#05-402-25 or CAT#05-402-7)
- Thermomixer capable of holding 1.5mL or 2.0mL tubes
- Benchtop centrifuge (capable of holding 1.5mL or 2mL microfuge tubes)
- Magnetic rack for 1.5mL or 2.0mL tubes (I like this rack: Promega, CAT#Z5342)
- Sonicating water bath (optional)

<span id="solution-recipes"></span>

## Solution recipes

- 100mM HEPES, pH 7.3 (100uL of 1M stock combined with 900uL of water)
- 80% (v/v) ethanol (prepare fresh)

<span id="protocol"></span>

## Protocol

For all stages of this protocol, discussion of various aspects related to performance or compatibility can be found in PMID: 30464214.

1. Prepare your sample by bringing 100ug of protein from the lysate to a total volume of 190uL using 100mM HEPES pH 7.3.
2. Prepare the SP3 beads stock (see [**Note 2**](#note2)):
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
13. At this point, you can elute your proteins, or digest. For elution:
    1. Reconstitute the beads in your elution solution of choice (see [**Note 3**](#note3)).
    2. Incubate, heat, or sonicate the mixture to factilate elution.
    3. Place the tube on a magnetic rack and wait for the beads to settle.
    4. Recover the eluted proteins to a fresh 2mL tube.
14. For digestion:
    1. Prepare a digestion solution by combining 2ug of trypsin in 100uL of 100mM HEPES, pH 7.3 (see [**Note 4**](#note4)).
    2. Add 100uL of the digestion solution to the sample and pipette mix (see [**Note 5**](#note5)).
    3. Incubate at +37C in a shaking incubator or ThermoMixer overnight (around 14-hours).
    4. After digestion, gently shake the tube to reconstitute the beads.
    5. Centrifuge the tube at 20,000g for 2-minutes.
    6. Place on the magnetic rack and wait for the beads to settle.
    7. Transfer the supernatant to a fresh 1.5mL tube.
    8. The peptide sample can be stored at -80C indefinitely.

<hr style="height:6pt; visibility:hidden;" />

<span id="notes"></span>

## Notes

<span id="note1"></span>

**Note 1** - Other beads can be substituted here, such as BangsLabs Magnefy beads (CAT#MFY0001), or other carboxylate modified particles. Other companies, such as MagReSyn also offer HILIC beads which are also compatible.

<span id="note2"></span>

**Note 2** - The bead stock from the vendor is 50mg/mL. We recommend using the beads at a 10:1 (ug of beads : ug of protein) ratio. This is far in excess of what is necessary, but will improve rinsing and elution efficiency by reducing the amount of 'clumping' that happens during binding.

<span id="note3"></span>

**Note 3** - Elution of proteins directly from the beads can be inefficient just due to how efficient the binding is itself. So, the more aggressive you can be here, the more successful you will be. For example, you will see more efficient elution if you are able to using detergent containing solutions, heating, and sonication.

<span id="note4"></span>

**Note 4** - I generally aim to have a trypsin:protein, ug:ug ratio of around 1:100, depending on the volume. For a larger volume I would likely scale this down to a 1:25 ratio. But these are personal preferences and digestion should be efficient at the values you would typically use in your lab.

<span id="note5"></span>

**Note 5** - The beads may need to be sonicated for 30-seconds in a water bath to help disaggregate them. If you noticed a large amount of clumping of the beads during the binding phase, this can be beneficial for ensuring an efficienct digestion.
