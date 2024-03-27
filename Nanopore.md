## Library Prep and Sequencing for Nanopore

### Summary
This is a three-step procedure for library prep and sequencing. This procedure is adapted from the [ligation sequencing Kit V14](https://github.com/ken-inoue/lab_protocols/files/14776449/Ligation_Sequencing.pdf), [Srivathsan et. al (2021)](https://doi.org/10.1186/s12915-021-01141-x), and [ligation sequencing DNA V14 (SQK-LSK114)](https://github.com/ken-inoue/lab_protocols/files/14776483/genomic-dna-by-ligation-sqk-lsk114-GDE_9161_v114_revU_29Jun2022-minion.pdf) protocols. This procedure is volume adjusted for Flongle Flow Cells but may need modification for use with MinION Flow Cells or other Nanopore sequencing devices.

Step 1: [End Prep](https://github.com/ken-inoue/lab_protocols/blob/main/Nanopore.md#end-prep)

Step 2: [Adapter Ligation and Cleanup](https://github.com/ken-inoue/lab_protocols/blob/main/Nanopore.md#adapter-ligation-and-cleanup)

Step 3: [Priming and Loading the Flongle Flow Cell](https://github.com/ken-inoue/lab_protocols/blob/main/Nanopore.md#priming-and-loading-the-flongle-flow-cell)

## End Prep
### Equipment and Supplies
- Vortex
- Table-top centrifuge
- Gentle rotator mixer
- Magnetic rack
- Pipettes
- Pipette tips
- 1.5 mL Eppendorf tubes
- Qubit assay tubes
- Ice
- Qubit fluorometer

### Reagents and standards
- 100 ng DNA from [PCR product pooling and cleanup (Nanopore)](Nanopore_Product_Pooling.md)
- DNA Control Sample (DCS)
- SPRI beads
- Molecular-grade H2O
- 100% EtOH
- NEBNext Ultra II End Repair/dA-tailing Module
- Qubit dsDNA HS Assay Kit

### Procedure
#### Mix DNA solution
*This protocol calls for 100 ng of DNA adjusted to 22.5 µL in molecular-grade H2O.*
1. steps here
#### End-prep
1. Thaw DNA Control Sample (DCS) at room temperature, spin down, mix by pipetting, and place on ice.
2. Thaw NEBNext Ultra II End Repair/dA-tailing Module reagents on ice.
    - **Do NOT vortex the Ultra II End Prep Enzyme Mix**. Flick or invert the tube to ensure it is well mixed.
    - The Ultra II End Prep Buffer may have precipitate. Pipette the buffer up and down to break up the precipitate and then vortex for 30 seconds.
3. In a 0.2 μL PCR tube, mix the following

|Reagent	|Volume|
|:--------|:-----|
|DCS|0.5 µL|
|DNA|22.5 µL|
|Ultra II End Prep Reaction Buffer|3.5 µL|
|Ultra II End Prep Enzyme Mix|1.5 µL|
|Molecular-grade H2O|2 µL|
|**Total**|**30 µL**|

4. Thoroughly mix the reaction by gently pipetting up and down.
5. Incubate the reaction in a thermal cycler for 10 minutes (20°C for 5 minutes, 65°C for 5 minutes).
6. Resuspend SPRI beads by vortexing.
7. Transfer the DNA to a clean 1.5 mL Eppendorf tube.
8. Add 30 µL of resuspended SPRI beads to the reaction and mix by flicking the tube.
9. Incubate at room temperature on a gentle rotator mixer for 5 minutes.
10. Prepare 300 µL of fresh 80% EtOH in a clean 1.5 mL Eppendorf tube (60 µL molecular-grade H2O, 240 µL 100% EtOH).
11. Spin down sample and pellet on a magnetic rack until the supernatant is clear and colorless (~3-5 minutes).
12. Keep tube on magnetic rack, pipette off the supernatant, and disgard the supernatant.
13. Keep tube on magnetic rack, add 100 µL 80% EtOH and wash by gently pipetting up, taking care not to disturb the beads. Let sit for 1 minute, then pipette off EtOH and disgard.
14. Repeat step 13.
15. Remove the tube from rack, spin down, and place tube back on magnet. Pipette off any residual EtOH and allow pellet to dry for 30 seconds. **Do NOT overdry the pellet**.
16. Remove the tube from rack and resuspend the pellet in 31 µL of molecular-grade H2O. Resuspend the pellet by flicking and incubate at room temperature for 2 minutes.
17. Pellet the beads on magnetic rack until eluate is clear and coloreless (~1-2 minutes).
18. Pipette off the 31 µL eluate and transfer to a clean 1.5 mL Eppendorf tube. The pellet may be disgarded.
19. Quantify 1 µL of eluate using a Qubit fluorometer. *The sample should read between 3-4 ng/µL if 100 ng of cleaned PCR product were used in the DNA solution*
### Sample storage
Move immediately to the adapter ligation step. If this is not possible, the sample can be stored at 4°C overnight.

## Adapter Ligation and Cleanup
### Equipment and Supplies
- Vortex
- Table-top centrifuge
- Gentle rotator mixer
- Magnetic rack
- Pipettes
- Pipette tips
- 1.5 mL Eppendorf tubes
- Qubit assay tubes
- Ice
- Qubit fluorometer

### Reagents and Standards
- Eluate from end-prep step
- Ligation Adapter (LA)
- Ligation Buffer (LNB) *from the ligation sequencing kit*
- Long Fragment Buffer (LFB)
- Short Fragment Buffer (SFB)
- SPRI beads
- Elution Buffer (EB) *from the Oxford Nanopore sequencing kit*
- NEBNext Quick Ligation Module

### Procedure
#### Adapter ligation and cleanup

## Priming and loading the Flongle Flow Cell
### Equipment and Supplies
- Flongle Flow Cell
- MinION device with Flongle adapter
- Pipettes
- Pipette tips
- 1.5 mL Eppendorf tubes

### Reagents and Standards
- Eluate from adapter ligation and cleanup step
- Molecular-grade H2O
- Flow Cell Flush (FCF)
- Flow Cell Tether (FCT)
- Library Beads (LIB)
- Sequencing Buffer (SB)

### Procedure
#### Priming and loading the Flongle Flow Cell

#### Data Acquisition and Basecalling

***
### Data analysis and cleanup

### Cleanup

### Notes

