## PCR Cleanup (ExoSAP)

### Summary
This is a procedure for polymerase chain reaction (PCR). This protocol was designed specifically for the ExoSAP step of sample prep for Sanger sequencing, and removes excess primers and unincorporated nucleotides from the Sanger sequencing PCR reaction. Each study will require fine tuning of this protocol as PCR protocols may not transfer well from one study to another. This protocol provides a starting point but may need modifications (see PCR optimization procedure and troubleshooting).

### Equipment and Supplies
- Vortex
- Pipettes
- Pipette tips
- Microcentrifuge tubes
- Table-top centrifuge
- Thermal cycler

### Reagents and Standards
- PCR products from [PCR (general and Sanger sequencing)](PCR.md)
- Exonuclease I (Exo I)
- Shrimp Alkaline Phosphatase (rSAP)
- Buffer (Exonuclease I reaction buffer or rCutSmart buffer)

### Sample Preparation and Storage
All reagents should be kept frozen until you are ready to use. Products from the Sanger sequencing PCR reaction may be allowed to thaw and sit out during preparation.

### Procedure
To minimize pipette error and chances of contamination, you will first make a master mix solution depending on how many samples you are running plus 4 (to account for pipetting error). This master mix solution is then put into each tube so that you are not putting in each reagent into each tube separately.

### PCR for ExoSAP cleanup
1. Thaw all reagents and keep them on ice. Briefly vortex but do not spin.
2. Make the following PCR reaction mix solution on ice.

The following is an example of a reagent master mix for 96 samples*. These volumes are deposited into each well of a 96-sample plate containing PCR products from the Sanger sequencing PCR reaction.
|Reagents	|Amount| Final concentration|
|:--------|:-----|:-------------------|
|Exo I | 25 µL | | 
|rSAP | 50 µL | |
|Buffer | 100 µL | |

_*Total volume adds +4 reaction volume to account for pipetting error_

The following table displays the final volume of all reagents in each well of the 96-sample plate
|Reagents	|Amount	|Final concentration in each well
|:--------|:-----|:-------------------|
|Exo I | 0.25 µL |	|
|rSAP | 0.5 µL | |
|Buffer | 1 µL | |
|PCR product | 10 µL | |

3. Aliquot 1.75 µL of the master mix into each well of the plate containing PCR product, placing the mix on the wall of each well. 
4. Mix the reagents well by spinning in plate centrifuge.
5. Cover the plate and place it into the thermal cycler and run Exosap program.  Basic thermal cycle: Incubate at 37˚C for 15 min followed by inactivation of ExoSAP reagents at 80˚C for 15 min.

### Clean Up

### Data Analysis and Calculations

### Notes
- Samples can be frozen after this step
- See [Cycle sequencing](Cycle_sequencing.md) procedure for next steps to process products for Sanger sequencing
