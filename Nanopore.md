## Library Prep and Sequencing for Nanopore

### Summary
This is a three-step procedure for library prep and sequencing. This procedure is adapted from the [ligation sequencing Kit V14](https://github.com/ken-inoue/lab_protocols/files/14776449/Ligation_Sequencing.pdf), [Srivathsan et. al (2021)](https://doi.org/10.1186/s12915-021-01141-x), and [ligation sequencing DNA V14 (SQK-LSK114)](https://github.com/ken-inoue/lab_protocols/files/14776483/genomic-dna-by-ligation-sqk-lsk114-GDE_9161_v114_revU_29Jun2022-minion.pdf) protocols. This procedure is volume adjusted for Flongle Flow Cells but may need modification for use with MinION Flow Cells or other Nanopore sequencing devices.

Step 1: End Prep

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

### Data Acquisition and Basecalling

### Data analysis and cleanup

### Cleanup

### Notes

