# Folder structure and file format

## Folder structure

Each catalog has its own folder and there are multiple folders within it.

* `hg38/` catalog in json format in hg38
* `hg19/` catalog in json format in hg19
* `truthset/` truthset developed based on PacBio CCS reads and replicates of illumina reads  

## File format

* Catalogs are stored in json format as specified in [ExpansionHunter](https://github.com/Illumina/ExpansionHunter/blob/master/docs/04_VariantCatalogFiles.md).
* Truthset for each sample are in csv format with two columns: `VariantId` and `Genotype`. 
