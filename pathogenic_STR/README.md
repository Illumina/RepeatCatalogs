# Pathogenic STR

## Overview

We have curated a set of STRs that cause diseases, which contains 40+ known pathogenic STRs from literatures. We regularly update the catalog to incorporate novel pathogenic STRs.

If you are interested in analyzing known pathogenic STRs, this is the catalog to use. Most of STRs in the catalog are integrated into Dragen and TruSight Software Suite. But you can also analyze them using custom bam/cram files with Expansion Hunter.

## Truthset

Truthset for NA12878 was generated using PacBio CCS data. Overview of the method is described [here](../docs/truthset.md).

In particular, we performed several filters for pathogenic STR.

1. 22 STRs can be called using PacBio CCS data which are single-unit and contain no ambiguous bases.
2. We further require minimum allele supported by >30% CCS reads and all alleles supported by >80% CCS reads and all 22 STRs met the criteria.
3. In summary, we have 22 STRs in the truthset.  

## Population distribution

To facilitate the use of the catalog, we genotyped pathogenic STRs across different samples in 1000 Genomes Project using Expansion Hunter 4.0.2. The genotypes are [here](hg38/genotype/1000genomes). We also compared genotypes with known pathogenic threshold and summarized results in [documentation](hg38/genotype/1000genomes/docs/pathogenic_STR_1kg.md).
