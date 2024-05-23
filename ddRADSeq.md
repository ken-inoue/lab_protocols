## ddRADSeq

### Summary
This protocol describes a double digested restriction-site associated DNA (ddRADseq) procedure, that is a variation on the original RAD sequencing method (Davey & Blaxter 2011), which is used for de novo SNP discovery and genotyping. 

*This protocol differs from the original ddRADseq protocol (Peterson et al 2012), in which the samples are pooled just after the ligation to adaptors (i.e. before size selection and PCR).*
The present ddRAD protocol as been slightly adapted from Alan Brelsford's protocol published in the supplementary material of this paper: (https://www.nature.com/articles/hdy201583/)

[ddRADseq at a glance](https://github.com/ken-inoue/lab_protocols/assets/151090195/a970a2e2-8c46-43b6-b73e-9df929fda2df)


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
  - [P1-PstI_sequences.pdf](https://github.com/ken-inoue/lab_protocols/files/15421345/P1-PstI_sequences.pdf)
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
#### Preparation of double-stranded adapters
##### Barcoded P1 adapters
1. 
