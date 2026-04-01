# Myriad-HPC
This repository collects bioinformatics pipelines I have used and studied, with practical notes and reproducible commands.
This workflow is based on the ULP-WGS pipeline:
https://github.com/TearsWillFall/ULPwgs
It was used during my PhD internship at UCL (Prof. G. Attard lab) for cfDNA analysis.
**Branch Structure**

Pipelines included:

This repository is organized into modular branches representing different analytical components:

- `main` → full integrated pipeline
- `abemus` → preprocessing and permissive variant calling
- `clonet` → CNV analysis and tumor content estimation
- `strelka` → stringent variant calling

Each branch can be used independently or as part of the complete workflow.

**Goals:**
Document real-world usage
Provide reproducible command-line examples
Build a solid reference for future projects

**Environment:**
Most analyses were run on Linux (HPC environment).

**Notes:**
These are practical notes based on hands-on usage, not official documentation.
