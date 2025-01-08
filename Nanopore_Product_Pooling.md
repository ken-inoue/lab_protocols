## PCR Product Pooling and Cleanup for Nanopore

### Summary
This is a procedure for PCR product pooling and cleanup for Nanopore adapted from [Srivathsan et al. (2021)](https://doi.org/10.1186/s12915-021-01141-x). This procedure is volume adjusted for Flongle Flow Cells but may need modification for use with MinION Flow Cells or other Nanopore sequencing devices.

***For first time Nanopore users, we recommend that you review the [Nanopore online learning](Nanopore_learning.md) document before starting Nanopore lab protocols.***

### Equipment and Supplies
- Vortex
- Table-top centrifuge
- Magnetic rack
- Pipettes
- Pipette tips
- 1.5 mL Eppendorf tubes
- 8-strip tubes
- Qubit Fluorometer

### Reagents and Standards
- PCR products from [PCR (Nanopore)](Nanopore_PCR.md) protocol
- Molecular-grade H20
- 100 % EtOH
- SPRI beads

### Sample preparation and storage
PCR products should be kept frozen until use. Products can be taken out and thawed to room temperature before being pooled. SPRI beads should be kept refrigerated at 4°C, and can be brought to room temperature and vortexed well before use. All other reagents can be stored at room temperature.

### Procedure
#### Pooling of PCR products
1. Using a multichannel pipette, pipette 6 μL of PCR product from each well of the plate(s) into a single 8-strip tube.
2. Pool the PCR products in the 8-strip tube into a single 1.5 mL tube.
3. Take a 500 μL subsample of pooled producted from the tube and add it to a clean 1.5 mL tube.
#### Cleanup of pooled products
5. Add a .7x ratio (for COI) of SPRI beads to the tube containing the subsample of pooled products. For 500 μL, add 350 μL SPRI beads.
6. Incubate the tube at room temperature for 10 minutes to allow DNA to bind to the beads.
7. Pellet SPRI beads on a magnetic rack for 2 minutes until supernatant is clear and colorless.
8. Leaving the tube on the magnetic rack, pipette off the supernatant without disturbing the beads. Place the supernatant in a clean 1.5 mL tube and set aside.
9. Make 2 mL of fresh 70% EtOH in 2 1.5 mL tubes by adding 300 μL molecular-grade H20 and 700 μL of 100% EtOH to each tube. Mix by briefly vortexing or inverting the tube.
10. Add 1 mL 70% EtOH to the beads, pipetting gently up and down to wash the beads without disturbing them. Incubate the tube on the magnetic rack for 2 minutes.
11. Pipette off the ethanol, taking care to not disturb the beads.
12. Repeat steps 9 and 10 to wash the beads a second time.
13. Dry the bead pellet on the magnetic rack for up to 5 minutes. Do not overdry the pellet.
14. Take the tube off of the magnetic rack, add 40 μL of molecular-grade water to elute the DNA and flick the tube to resuspend the pellet.
15. Incubate the tube at room temperature for 10 minutes.
16. Pellet beads on the magnetic rack for 5 minutes until the eluate is clear and colorless.
17. Transfer eluate into a clean 1.5 mL tube.

### Data analysis and calculation
18. Quantify 1 μL of eluate using a [Qubit](Qubit.md) fluorometer. If original concentration is too high, quanify a 1:5 or 1:10 dilution of eluate.
19. [Gel test](gel_electrophoresis.md) cleanup success by running conserved supernatant and eluate side-by-side. If cleanup was successful, the eluate should show no presence of primer dimers and should be brighter than the supernatant. If primer dimers are still present in cleaned product, an additional cleanup may be necessary. [Photo example](https://github.com/ken-inoue/lab_protocols/assets/151090195/a5ca5d4f-1c47-4dab-9169-440d7e57c553)

### Cleanup
Remaining pooled products from Step 2 may be frozen for future use or disgarded.
Remaining supernatant from Step 8 not used in gel test may be disgarded.

### Notes
Move on to [Nanopore library prep and sequencing](Nanopore.md).
