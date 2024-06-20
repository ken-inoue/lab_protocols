## ddRADseq

### Summary
This protocol describes a double digested restriction-site associated DNA (ddRADseq) procedure, that is a variation on the original RAD sequencing method (Davey & Blaxter 2011), which is used for de novo SNP discovery and genotyping. 

*This protocol differs from the original ddRADseq protocol (Peterson et al 2012), in which the samples are pooled just after the ligation to adaptors (i.e. before size selection and PCR).*
The present ddRAD protocol as been slightly adapted from Alan Brelsford's protocol published in the supplementary material of this paper: (https://www.nature.com/articles/hdy201583/)

[ddRADseq at a glance](https://github.com/ken-inoue/lab_protocols/assets/151090195/a970a2e2-8c46-43b6-b73e-9df929fda2df)

#### Procedure shortcuts:
[Preparation of double-stranded adapters](https://github.com/ken-inoue/lab_protocols/blob/main/ddRADseq.md#preparation-of-double-stranded-adapters)

[Double digestion](https://github.com/ken-inoue/lab_protocols/blob/main/ddRADseq.md#double-digestion)

[Adaptor ligation](https://github.com/ken-inoue/lab_protocols/blob/main/ddRADseq.md#adaptor-ligation)

[Bead purification](https://github.com/ken-inoue/lab_protocols/blob/main/ddRADseq.md#bead-purification)

[PCR](https://github.com/ken-inoue/lab_protocols/blob/main/ddRADseq.md#pcr-first-cycle)

[Size selection](https://github.com/ken-inoue/lab_protocols/blob/main/ddRADseq.md#size-selection-with-pippin-prep)

### Equipment and supplies
- PCR plates
- PCR tube strips
- Eppendorf tubes
- Pipettes
- Pipette tips
- Agilent DNA High sensitivity DNA kit (5067-4626)
- Qubit microtubes
- Table-top centrifuge
- Vortex
- Microwave
- Thermocycler
- Gel Electrophoresis Systems
- Magnetic tube rack
- Pippin prep (Sage Science)
- Qubit fluorimeter
- qPCR equipment
- Bioanalyzer

### Reagents and Standards (need about ~100 ng of DNA)
- 100 %  ethanol (molecular biology grade)
- Gel electrophoresis materials/reagents
- DNAse-Rnase free ultrapure water
- EcoRI-HF®
  - EcoRI adapter p1.1: ACACTCTTTCCCTACACGACGCTCTTCCGATCTnnnnnnTGCA
  - EcoRi adapter p1.2: nnnnnnAGATCGGAAGAGCGTCGTGTAGGGAAAGAGTGT
- MspI  ref
    - MspI adaptor 2.1: GTGACTGGAGTTCAGACGTGTGCTCTTCCGATCT
    - MspI adaptor 2.2: /5Phos/TAAGATCGGAAGAGCGAGAACAA
    - (AT rich genomes) MspI adaptor 2.1 : GTGACTGGAGTTCAGACGTGTGCTCTTCCGATCT
    - (At rich genomes) MspI adaptor 2.2:  /5Phos/CGAGATCGGAAGAGCGAGAACAA
- ILLPCR1 primer: aaTGATACGGCGACCACCGAGATCTACACTCTTTCCCTACACGACG
- T4 DNA Ligase  ref NEB : M0202L
- ATP 10mM ref NEB : P0756
- Annealing buffer stock (10X): 100 mM Tris HCl, pH 8, 500 mM NaCl, 10 mM EDTA
- dNTP set 4x0,25mlx100mM ref Neb : N0446S
- Q5® Hot Start High-Fidelity DNA Polymerase  ref NEB : M0493L
- Ampure XP beads or NGS clean up and size selection (Macherey Nagel REF  744970.50)
- Elution solution/buffer for magnetic beads (Tris 10mM)
- Freshly diluted 70/80% ethanol 
- Pippin Prep reagents and cassettes (1,5 % DF Marker K,  ref SageScience CDF1510) -> might not use
- NEBNext Library Quant kit for illumina  ref Neb : E7630 -> only for dilution buffer if we want to quantify concentration at the end (only quantifies fragments that will be amplified during Illumina)
- Qubit 1X dsDNA BR (Thermo, Q33266)

### Sample Preparation & Storage
All reagents should be kept frozen or refrigerated according to manufacturer recommendations until you are ready to use. Repeated freezing and thawing will kill primers. Place primers on ice once thawed if possible.

### Procedure
#### Make annealing buffer
1. Make the annealing buffer according to the recipe below:

|Reagents|Amount|
|:--------|:-----|
|Tris-HCl pH 8|100 mM|
|NaCl|500 mM|
|EDTA Na2|10 mM|
#### Preparation of double-stranded adapters
##### Barcoded P1 adaptors
2. In a 96-well plate, combine complimentary oligos [P1-PstI_sequences.pdf](https://github.com/ken-inoue/lab_protocols/files/15421345/P1-PstI_sequences.pdf) together with annealing buffer and nuclease-free water according to the table shown below. Leave space between wells to avoid cross contamination.
- Example plate map
  - <img width="493" alt="Plate map example" src="https://github.com/ken-inoue/lab_protocols/assets/151090195/99b871a3-9e30-4c69-9f66-a1f3015af46a">
In each well:
|Reagents|Concentration|Volume|
|:--------|:-----|:-----|
|Adaptor P1-1|10µM|5 µL|
|Adaptor P1-2|10µM|5 µL|
|Annealing buffer|10X|5 µL|
|Nuclease-free H2O|na|35 µL|
3. Seal the plate and incubate in a thermal cycler at 95°C for 5 minutes, then cool at a rate of 0.1°C/s to 20°C. Store at 4°C or -20°C for long term storage.
##### P2 adaptors
4. In an Eppendorf tube, combine the following and mix by pipetting:

|Reagents|Concentration|Volume|
|:--------|:-----|:-----|
|P2-1|100µM|80 µL|
|P2-2|100µM|80 µL|
|Annealing buffer|10X|80 µL|
|Nuclease-free H2O|na|560 µL|
5. Aliquot 100 µL of the solution into each well of an 8-PCR tube strip
6. Seal the tube strip and incubate in a thermal cycler at 95°C for 5 minutes, then cool at a rate of 0.1°C/s to 20°C. Store at 4°C or -20°C for long term storage.
#### Preparation of genomic DNA *(reqiures 50-100 ng of DNA per sample)*
7. Add genomic DNA and 30 µL nuclease-free water in a 96-well plate. Samples should not contain RNA. An RNAase treatment can be added to extraction to achieve RNA-free samples. Randomize samples across the plate, leaving a few wells open as negative controls.
#### Double digestion
8. Thaw, vortex and spin down all reagents except for enzymes. Place all reagents on ice while thawing.
9. In an Eppendorf tube, prepare the following master mix:

|Reagents|Concentration|Final quantity|N=1|N=104 (1 plate)|
|:--------|:-----|:-----|:-----|:-----|
|Genomic DNA|NA|50-200 ng|30 µL|NA|
|Cutsmart buffer|10X|1X|3.5 µL|364 µL|
|Enzyme 1 EcoRI HF|20u/µL|8U|0.4 µL|41.6 µL|
|Enzyme 2 Mspl|10u/µL|2 U|0.2 µL|20.8 µL|
|Nuclease-free H2O|NA|NA|0.9 µL|93.6 µL|
|Total volume|||35 µL||

10. Vortex and spin down the master mix. Aliquot 65 µL of master mix into each well of an 8-PCR tube strip.
11. Use a multichannel pipette to add 5 µL of master mix into each well of the 96-well plate containing the 30 µL of diluted genomic DNA. Seal the plate and spin down.
12. Incubate the plate in a thermal cycler at 37°C for 10 hours, then at 65°C for 20 minutes (to inactivate enzymes), then at 4°C overnight.
#### Check digestion
13. Check the efficiency of the digestion on a gel using 5 µL of digested DNA. High molecular weight DNA should no longer be visible. [Example](https://github.com/ken-inoue/lab_protocols/assets/151090195/33d7c782-2b79-4d5d-9ef0-8a6746fb9a5f)
#### Adaptor ligation
14.  Thaw, vortex and spin down all reagents except for enzymes. Place all reagents on ice while thawing.
15.  Set up the adaptor ligation mix and ligation reaction as follows:
###### Ligation Mix
|Reagents|Concentration (stock)|Concentration (final)|N=1|N=104 (1 plate)|
|:--------|:-----|:-----|:-----|:-----|
|ds nonbarcoded adaptor P2|10µM|NA|1.8 µL|187.2 µL|
|Cutsmart buffer|10X|1X|1 µL|104 µL|
|ATP|10mM|1mM|4 µL|416 µL|
|T4 DNA ligase|400u/µL|NA|0.4 µL|41.6 µL|
|Nuclease-free H2O|NA|NA|0.9 µL|93.6 µL|
|Total volume|||7.2 µL||
###### Ligation Master Mix
|Reagents|N=1|
|:--------|:-----|
|Digest DNA|30 µL|
|ds barcoded adaptor P1 1µM|2.8 µL|
|Ligation mix|7.2 µL|

16. Vortex and spin down the master mix. Aliquot 93.5 µL of master mix into each well of an 8-PCR tube strip.
17. In the DNA digestion plate (30 µL per well) add 2.8 µL of Adapt P1 from the adaptor plate (see Step 1) with a multichannel pipette.
18. Use a multichannel pipette to add 7.2 µL of ligation master mix into each well of the DNA digestion plate. Seal the plate and spin down.
19. Incubate the plate in a thermal cycler at 16°C for 6 hours, then at 4°C overnight. *If you are not planning to perform the bead purification the day after, store at -20°C.*
#### Bead purification
##### Prep
20. Remove magnetic beads from fridge and allow them to sit out and come to room temperature.
22. Prepare 50 mL fresh 70% EtOH (35 µL 100% EtOH, 15 µL nuclease-free H2O).
24. Vortex magnetic beads well to resuspend in solution. Fill each well of a 8-PCR tube strip with bead solution.
25. Using a multichannel pipette, add 60 µL of bead solution to the first 4 columns of a 96-well PCR plate.
26. Spin down the 96-well plate containing the digested-ligated DNA products.
27. Fill each well of a 8-PCR tube strip with Tris-HCl pH8 10mM.
28. Using a multichannel pipette, add 5 µL of Tris-HCl to each well of the 96-well plate containing digested-ligated DNA products.
##### Purification
28. Using a multichannel pipette, transfer 40 µL of DNA products from the first 4 columns of the digested-ligated 96-well plate into the first 4 columns of the purification plate. Mix by gently pipetting up and down. Incubate for 5 minutes at room temperature
29. Place the purification plate on the magnetic plate rack and incubate for 5 minutes until supernatant is clear and colorless and beads are pelleted on the walls of each well.
30. Leaving the plate on the magnetic rack, remove and disgard the supernatant using a pipette, taking care not to disturb the bead pellet.
31. Leaving the plate on the magnetic rack, add 200 µL of 70% EtOH to each well in the first 4 columns of the purification rack. Take care not to disturb the bead pellet. Incubate for 1 minute, then remove and disgard the EtOH using a pipette.
32. Repeat step 31.
33. Leaving the plate on the magnetic rack, let the bead pellets dry for a maximum of 5 minutes, taking care not to overdry the pellets to the point of cracking.
34. Remove the plate from the magnetic rack. Using a multichannel pipette, add 40 µL of Tris pH8 10mM to each well. Pipette up and down gently to re-suspend the pellet in solution. Incubate the purification plate at room temperature for 5 minutes.
35. Place the plate back on the magnetic rack and incubate for 5 minutes until eluate is clear and colorless and beads are pelleted on the walls of each well.
36. Transfer 35 µL of eluate containing purified DNA to a new 96-well plate. Disgard the purification plate.
37. Seal and store the plate at 4°C and proceed with the purification of columns 5-8 and 9-12 as described above. Once finished, seal and store the plate at 4°C for short term storage or -20°C for long term storage until PCR amplification.
#### PCR (first cycle)
38. Prepare the following master mixes in 5 mL and 1.5 mL Eppendorf tubes, respectively, as shown below:

###### 5 mL tube
|Reagents|Concentration (stock)|N=1|N=104 (1 plate)|
|:--------|:-----|:-----|:----|
|NEB Q5 buffer|5X|8 µL|832 µL|
|dNTP mix|25mM|0.3 µL|31.2 µL|
|NEB Q5 hotstart hifi DNA polymerase|2u/µL|0.4 µL|41.6 µL|
|NEB high GC enhancer|5X|8.0 µL|832 µL|
|Nuclease-free H2O||3.3 µL|343.2 µL|
|**Total volume**||20 µL|2080 µL|

###### 1.5 mL tubes (4 tubes total for a 96-well plate, 1 index per tube)
|Reagents|Concentration (stock)|N=1|N=28 (3 columns)|
|:--------|:-----|:-----|:----|
|illPCR primer mix (illPCR1 and illPCR2)|5X|1.4 µL|39.2 µL|
|Nuclease-free H2O||8.6 µL|240.8 µL|
|**Total volume**||10 µL|280 µL|

39. Vortex all 5 tubes of master mixes and spin down.
40. Aliquot 130 µL of the first master mix (in 5 mL tube) into each well of 2 8-PCR tube strips. Using a multichannel pipette, dispense 20 µL of the first master mix into each well of a new 96-well plate.
41. Aliquot 93 µL of the 4 primer PCR mixes (1.5 mL tubes) into each well of a 12-PCR tube strip (3 wells of 93 µL per index primer mix). [Example image](https://github.com/ken-inoue/lab_protocols/assets/151090195/9d344063-1fdf-4491-adb6-bfdb9b72d191)
42. Using a 12 multichannel pipette, dispense 10 µL of the PCR mixes by rows into each well of the 96-well plate containing the first master mix.
43. Spin down the adaptor-ligated purified DNA plate.
44. Using a multichannel pipette, transfer 10 µL of DNA into its corresponding well on the PCR plate and mix by pipetting.
45. Aliquot the 40 µL total volume in the PCR plate by transfering 30 µL from each well into 3 new PCR plates (10 µL of PCR mix per plate). Seal all 4 PCR plates and spin down.
46. Plate all 4 plates in thermal cyclers and start PCR simultaneously using the following program: 98°C for 30s, 15x [98°C for 20s, 60°C for 60s, 72°C for 40s], 72°C for 10 min, 12°C hold.

*PCR will be performed in parallel in 4 different thermal cyclers in order to reduce PCR bias. Products are pooled back into a single plate after PCR using a multichannel pipette.*
#### PCR (second cycle)
*Primers in excess*

47. Prepare the following master mix for each index primer in a 1.5 mL Eppendorf tube (4 total):

|Reagents|Concentration (stock)|N=1|N=28 (3 columns)|
|:--------|:-----|:-----|:----|
|NEB Q5 buffer|5X|0.2 µL|24 µL|
|dNTP mix|25mM|0.08 µL|9.6 µL|
|illPCR primer mix (illPCR1 and illPCR2)|5X|0.4 µL|48 µL|
|Nuclease-free H2O||0.32 µL|38.4 µL|
|**Total volume**||4 µL|120 µL|

## Issue here with volume of 4? double check

48. Vortex all 4 primer mixes and spin down. Aliquot 40 µL of the primer PCR mixes into each well of a 12-PCR tube strip (3 wells of 40 µL per index primer mix as shown in the example image from the first PCR).
49. Using a 12 multichannel pipette, dispense 4 µL of the PCR mixes by rows into each well of the 96-well plate containing the pooled products from the first PCR cycle. Seal the plate and spin down.
50. In a thermal cycler, run the following program: 98°C for 3 min, 60°C for 2 min, 72°C for 12 min, 12°C hold.
51. Store at 4°C for short term storage or -20°C for long term storage.
#### Check PCR success
52. Check the efficiency of PCR on a gel using 5 µL of PCR product. All smears should have a similar intensity after equalizing PCR. 
#### Sample pooling
53. All barcoded and index individuals can now be pooled into a single tube. Pool 5 µL of all individual samples into a single, 1.5 mL Eppendorf tube.

*If smear intensity on gel is not uniform, you can estimate the concentration of DNA fragments per sample and pool based on intensity (i.e., create separate pools for "low", "intermediate" and "high" intensity samples).*

54. Use Qubit to estimate the DNA concentration of the pooled samples. If the DNA concentration is lower than 20 nM, perform a 1:1 bead clean-up following the steps in the "Bead purification" section on a partial volume of the pool to improve the final concentration of DNA. Elution should be done in at least 50 µL, but adapt volume to the desired final concentration.
#### Size-selection with Pippin-Prep
55. Perform size selection on fragments between 300-800 bp using a 1.5% DF marker K agarose gel cassette. Follow manufacturer instructions [here](https://github.com/user-attachments/files/15877171/Quick-Guide-CDF1510-marker-K3.pdf).
#### Quality control
56. Use a Bioanalyzer (Agilent) in a High Sensitivity DNA chip to control the quality of the library. Dilute your pool 1:2 or more and load 1 µL of the pool before and after size selection, following manufacturer instructions [here](https://github.com/user-attachments/files/15877223/HighSensitivity_DNA_KG.pdf.pdf). [Example Bioanalyzer profile](https://github.com/ken-inoue/lab_protocols/assets/151090195/56fbe4a0-87c6-4629-8e7b-89eead0b8db4)
#### Concentration estimation
57. Perform an estimation of dsDNA using the Qubit BR assay kit or through qPCR quantification with the NEBNext Library Quant Kit for Illumina using p5 and p7 illumina primers. The qPCR estimation is more informative because it only registers fragments starting with p5 and ending with p7 sequences, effectively estimating only the DNA that will be amplified onto the flowcell of Illumina sequencers. [User manuel](https://github.com/user-attachments/files/15877270/manualE7630.pdf)
###### Dilution suggestions for qPCR kit
In a 8-tube PCR strip:
Prepare intermediate dilutions (1:10 and 1:100) of the library  with the dilution buffer supplied in the qPCR kit.

Then prepare the 4 library dilutions to be used in triplicate for qPCR analysis :

1:1000 : 10µl of 1/100 +  90µl buffer 1X

1:2000 : 50µl of 1/1000 +  50µl buffer 1X

1:4000 : 50µl of 1/2000 +  50µl buffer 1X

1:8000 : 50µl of 1/4000 +  50µl buffer 1X

You should get more than 10 nM, that is the library concentration usually required by the sequencing platform facilities. 
The library is now ready for sequencing in single read or paired-end 150 bases in an Illumina sequencer, with one index read. Use the average size of the library size range as estimated from the Bioanalyzer profile to convert DNA concentration from nM  to ng/µl.

























