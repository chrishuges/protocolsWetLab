# Preparation of immunoprecipitation samples for MS analysis <!-- omit in toc -->

This protocol was last updated - May 26, 2020 by Chris Hughes.

This document describes how to perform preparation of immunoprecipitated protein samples for analysis by mass spectrometry. The assumed starting point for this protocol is an eluted sample. As we will be using SP3 as the first processing step, elution can be performed in virtually any condition. Below, I give a formulation of a typical elution buffer that I use in my immunoprecipitation (IP) experiments.

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
- 20% SDS (Thermo Scientific, CAT#BP1311)
- Dithiothreitol (Bio-Rad, CAT#1610611)
- Chloroacetamide (Sigma, CAT#C0267)
- NP-40 (Sigma, CAT#NP40)
- Deoxycholate (DOC) (Sigma, CAT#D6750)
- cOmplete protease inhibitor tablets, EDTA free (Sigma, CAT#11836170001)
- Ethanol, absolute (whatever vendor sells this to your lab)
- SP3 beads (Thermo Scientific, CAT#65152105050250, CAT#45152105050250) (see [**Note 1**](#note1))
- Trypsin/rLysC mix (Promega, CAT#V5073)
- 1.5mL or 2.0mL Safe-Lock tubes (Fisher Scientific, CAT#05-402-25 or CAT#05-402-7)
- Thermomixer capable of holding 1.5mL or 2.0mL tubes (Eppendorf)
- Benchtop centrifuge (capable of holding 1.5mL or 2mL microfuge tubes)
- Magnetic rack for 1.5mL or 2.0mL tubes (Promega, CAT#Z5342)
- Sonicating water bath (optional)

<span id="solution-recipes"></span>

## Solution recipes

- 0.2M of dithiothreitol (DTT) - 15mg in 500uL of 1M HEPES, pH 7.3, prepare fresh and keep on ice
- 0.4M of chloroacetamide (CAA) - 18mg in 500uL of 1M HEPES, pH 7.3, prepare fresh and keep on ice
- 10% (v/v) NP-40 - 1mL in 9mL of water
- 10% (w/v) DOC - 1g in 10mL of water
- 10X cOmplete protease inhibitor stock - 1 tablet in 1mL of water
- IP elution solution (need 200uL per sample, recipe for 1mL)
  - 100mM HEPES pH 7.3 (100uL of 1M stock)
  - 0.5% (v/v) NP-40 (50uL of 10% stock)
  - 0.5% (v/v) DOC (50uL of 10% stock)
  - 1% (v/v) SDS (50uL of 20% stock)
  - 0.5X cOmplete protease inhibitor (50uL of 10X stock)
  - 10mM DTT (50uL of 0.2M stock)
  - water to 1mL (750uL of clean water)
- Clean water (Thermo Scientific, CAT#10977023)
- 100mM HEPES, pH 7.3 (100uL of 1M stock combined with 900uL of water)
- 80% (v/v) ethanol (prepare fresh)

<span id="protocol"></span>

## Protocol

1. Pre-heat the ThermoMixer to +85C.
2. Prepare your sample by reconstituting your IP beads in 100uL of IP elution solution and incubate in the heated ThermoMixer for 5-minutes with shaking at 1,000rpm.
3. Recover 95uL of the supernatant to a fresh 2mL tube and repeat the previous step one additional time for a total of two elutions. Combine the supernatants.
4. Prepare the SP3 beads stock (see [**Note 2**](#note2)):
   1. Vortex the bead stock to re-suspend the material.
   2. Take 500uL of each of the bead stocks and combine in a fresh 2mL tube.
   3. Place on a magnetic rack and wait for beads to settle. Discard the supernatant.
   4. Reconstitute the beads in 1mL of water with pipetting and place back on the magnetic rack. After the beads settle, discard the supernatant.
   5. Repeat the above rinse one additional time for a total of 2 rinses.
   6. Reconstitute the beads in 500uL of water. The bead stock can be stored at +4C indefinitely.
5. Add 10uL of SP3 beads to the sample and pipette mix.
6. Add 200uL of ethanol to the sample and gently shake the tube with your hand to mix the phases. Do not vortex.
7. Place in a shaking incubator at room temperature for 5-minutes.
8. Centrifuge the tube at 50g for 30-seconds to bring any liquid down from the top of the tube.
9. Place the tube on a magnetic rack and wait for the beads to settle. Discard the supernatant.
10. Remove the tube from the rack and reconstitute the beads in 800uL of 80% ethanol. Gently rinse the beads by pipetting.
11. Place the tube on a magnetic rack and wait for the beads to settle. Discard the supernatant.
12. Repeat **Steps 8 - 10** two additional times for a total of 3 rinses.
13. Place the tube back on the magnetic rack an wait for the beads to settle.
14. Discard the supernatant taking care to remove any residual ethanol remaining. It is not necessary to air dry the tubes.
15. At this point, you can elute your proteins, or digest. For elution:
    1. Reconstitute the beads in your elution solution of choice (see [**Note 3**](#note3)).
    2. Incubate, heat, or sonicate the mixture to factilate elution.
    3. Place the tube on a magnetic rack and wait for the beads to settle.
    4. Recover the eluted proteins to a fresh 2mL tube.
16. For digestion:
    1. Prepare a digestion solution by combining 1ug of trypsin in 100uL of 100mM HEPES, pH 7.3 (see [**Note 4**](#note4)).
    2. Add 100uL of the digestion solution to the sample and pipette mix (see [**Note 5**](#note5)).
    3. Incubate at +37C in a shaking incubator or ThermoMixer overnight (around 14-hours).
    4. After digestion, gently shake the tube to reconstitute the beads.
    5. Centrifuge the tube at 20,000g for 2-minutes.
    6. Place on the magnetic rack and wait for the beads to settle.
    7. Transfer the supernatant to a fresh 1.5mL tube.
    8. The peptide sample can be stored at -80C indefinitely.
17. The samples can now be processed for MS analysis (see [**Note 6**](#note6)).

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

<span id="note6"></span>

**Note 6** - You have quite a few options at this stage. I personally like to TMT label my replicate IP samples along with my controls, desalt with TopTips, and analyze by MS (protocols for all of these individual steps can be found on this GitHub page). Alternatively, you can directly desalt the digested peptides with TopTips and analyze by MS as single injection replicates. You could also substitute a volatile digestion solution instead of HEPES, such as ammonium bicarbonate, and proceed directly to MS analysis without the TopTip desalting step.
