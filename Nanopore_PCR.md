## PCR

### Summary
This is a procedure for polymerase chain reaction (PCR). This protocol was designed specifically for Nanopore sequencing. Each study will require fine tuning of this protocol as PCR protocols may not transfer well from one study to another. This protocol provides a starting point but may need modifications (see PCR optimization procedure and troubleshooting).

***For first time Nanopore users, we recommend that you review the [Nanopore online learning](Nanopore_learning.md) document before starting Nanopore lab protocols.***

### Equipment & Supplies
- Vortex
- Pipettes
- Pipette tips
- Microcentrifuge tubes
- PCR tubes
- Table-top spinner
- Thermal cycler

### Reagents & Standards
- Template DNA (~10 ng/µL)
- Taq Master Mix (GoTaq Master Mix, Promega)
- Forward & reverse primers
- Molecular-grade H2O

### Sample Preparation & Storage
All reagents should be kept frozen until you are ready to use. Repeated freezing and thawing will kill Taq and primers. The other materials may be thawed and allowed to set out during preparation. Place primers on ice once thawed if possible. There are 96 reverse primers. The easiest way to prepare them is by mixing dilutions in a 96-well plate (primers should have a concentration of 10 µM). 

### Procedure
To minimize pipette error and chances of contamination, you will first make a master mix solution depending on how many samples you are running plus 2 (one for a negative control and one to account for pipetting error). This master mix solution is then put into each tube so that you are not putting in each reagent into each tube separately.

#### PCR for Sanger Sequencing
1.	Thaw all reagents and keep them on ice. Briefly vortex and spin to collect the material at the bottom of the tubes.
2.	Mix the following PCR reaction master mix solution on ice in a 1.5 mL Eppendorf tube. Vortex well.

The following is an example for 96 (+2 for error) samples.
For 15-µL reaction volume:
|Reagents	|Amount|
|:--------|:-----|
|GoTaq Master Mix|735 µL|
|Forward primer (10 µM)|98 µL|
|Molecular grade H2O|392 µL|

3. Using a pipette, aliquot 12.5 µL of master mix into each well of a 96-well plate.
4. Using a multichannel pipette, add 1 µL of reverse primer from a prepared plate of 96 diluted reverse primers into each well of the sample plate. Spin down to mix the master mix with the added reverse primers.
5. Add 1.5 µL of DNA into each well of the sample plate, leaving one well without DNA to serve as a negative control. Briefly spin to mix. A single reaction should contain the following volumes

|Reagents	|Amount|
|:--------|:-----|
|GoTaq Master Mix|7.5 µL|
|Forward primer (10 µM)|1 µL|
|Molecular grade H2O|4 µL|
|Reverse primer (10 µM)|1 µL|
|DNA |1.5 µL|
|**Total**|**15 µL**|

6. Place the plate into the thermal cycler and run program. (Program will vary with project and gene being amplified).

### Clean up

### Data analysis and calculations
PCR products can be checked by agarose gel electrophoresis.

### Notes
See [PCR product pooling and cleanup (Nanopore)](Nanopore_Product_Pooling.md) and [Nanopore library prep and sequencing](Nanopore.md) for next steps in the Nanopore sequencing process.

