## Genome skimming

### Summary
Genome skimming is used to generate long-read, low coverage sequencing data for an individual sample, or a few barcoded samples. The protocol for genome skimming is virtually identical to that described in [Nanopore library prep and sequencing](Nanopore.md). Because genome skimming is PCR free, pooling and cleanup steps can be skipped (unless using multiple barcoded samples, then pooling is required before library prep). Before starting library prep, the sample (or pooled samples) must be quantified using Qubit HS fluorometry. The starting concentration for library prep for this protocol is recommended to be 400 ng/µL. All other steps of library prep and sequencing are the same.

When you load the flow cell and prep it for processing with MinKNOW, make sure to select the "PCR-free" option. You may also want to select for reads with a lower number of base pairs depending on the read length you are targeting (eg. 50bp minimum versus the standard 200bp).

### Analysis
Potential programs and helpful tips for analysis are listed below along with their functions.

