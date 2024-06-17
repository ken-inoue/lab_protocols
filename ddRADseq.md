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
- PstI-HF® ref NEB : R3140S
  - PstI adapter p1.1: ACACTCTTTCCCTACACGACGCTCTTCCGATCTnnnnnnTGCA
  - PstI adapter p1.2: nnnnnnAGATCGGAAGAGCGTCGTGTAGGGAAAGAGTGT
- MseI  ref Neb : R0525S
    - MseI adaptor 2.1: GTGACTGGAGTTCAGACGTGTGCTCTTCCGATCT
    - MseI adaptor 2.2: /5Phos/TAAGATCGGAAGAGCGAGAACAA
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
|Enzyme 1 Pst HF|20u/µL|8U|0.4 µL|41.6 µL|
|Enzyme 2 Msel|10u/µL|2 U|0.2 µL|20.8 µL|
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
#### PCR





















