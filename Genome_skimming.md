## Genome skimming

### Summary
Genome skimming is used to generate long-read, low coverage sequencing data for an individual sample, or a few barcoded samples. The protocol for genome skimming is virtually identical to that described in [Nanopore library prep and sequencing](Nanopore.md). Because genome skimming is PCR free, pooling and cleanup steps can be skipped (unless using multiple barcoded samples, then pooling is required before library prep). Before starting library prep, the sample (or pooled samples) must be quantified using Qubit HS fluorometry. The starting concentration for library prep for this protocol is recommended to be 400 ng/µL. All other steps of library prep and sequencing are the same.

When you load the flow cell and prep it for processing with MinKNOW, make sure to select the "PCR-free" option. You may also want to select for reads with a lower number of base pairs depending on the read length you are targeting (eg. 50bp minimum versus the standard 200bp).

### Analysis
Potential programs and helpful tips for analysis are listed below along with their functions.
#### QC
- [PycoQC](https://github.com/a-slide/pycoQC)
    - Used to check quality of raw and cleaned Nanopore data
    - Requires a summary.txt file, but can also generate a summary from fast5 files
    - Supports data generated from Minion, basecalling by MinKNOW, Albacore, or Guppy
    - Written in Python
#### Cleanup
- [Porechop](https://github.com/rrwick/Porechop)
    - Finds and removes adapters from Nanopore sequencing data
    - Con: Database of recognized adaptors is somewhat limited as new adaptors are being manufactured for Nanopore sequencing protocols
    - Can choose to split sequences with a middle adaptor or leave them intact
    - Runs on Linux or macOS
- [NanoFilt](https://github.com/wdecoster/nanofilt)
    - Filters and trims based on read quality and length
    - Can specify a number of nucleotides to trim from the beginning and end of each read
    - Can filter based on a specified Q score
    - Can filter based on a specified minimum and maximum read length
    - Written for Python, runs on Linux
#### Assembly
- [Minimap2 (with Geneious)](https://github.com/lh3/minimap2?tab=readme-ov-file)
    - Tip for Nanopore reads: use ava-ont mode and (-r 10,000) to help with long-read overlap
    - This program does not work well with large amounts of short-read overlap
    - Option for de novo assembly or assembly using a reference sequence
    - For cross species alignment:
      - asm5 = divergence <1%
      - asm10 = divergence ~2-3%
      - asm15 = divergence ≤ 20% *mapping divergence up to 15% has not been carefully evaluated*
- [Flye](https://github.com/mikolmogorov/Flye)
    - Uses de novo assembly to generate a consensus sequence
#### Polishing

#### Annotation
- [GeSeq](https://chlorobox.mpimp-golm.mpg.de/geseq.html)
    - Developed for plant chloroplasts, but can be used for mitochondrial genomes
    - Option to map to multiple reference genomes
    - Generates a graphic of the annotated genomes with gaps to denote missing sequences
    - Optimized for use with with Nanopore data
- [MITOS](http://mitos.bioinf.uni-leipzig.de/)
    - Used by multiple researchers for Nanopore data
    - No graphic of annotated genome
- [MitoZ](https://github.com/linzhi2013/MitoZ)
    - Used by multiple researchers for Nanopore data
    - No graphic of annoted genome
