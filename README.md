# STR Catalogs

Short tandem repeats (STRs) are genomic sequences comprised of repetitions of a short motif (typically 2-6bp). Many STRs are implicated in a variety of genetic disorders, such as Huntington's disease, amyotrophic lateral sclerosis (ALS), and fragile X syndrome. Thanks to recent improvements in Next-Generation Sequencing (NGS) technologies and computational methods (e.g., Expansion Hunter), it is now possible to identify large expansions of STRs using Whole Genome Sequencing (WGS).

Accurate repeat genotyping requires a high-quality STR catalog that specifies reference coordinates and structure of each locus. Here, we generated well-curated  STR catalog that can facilitate analysis of STRs genome-wide. 

## Documentation

### Analyze STRs using Expansion Hunter

The way to use the catalog is to genotype STRs in the catalog in WGS data using [Expansion Hunter](https://github.com/Illumina/ExpansionHunter). We provided a quick [introduction](docs/usage.md) to do that.

### Catalogs

The contains genome-wide STRs that are polymorphic across populations and 30+ known pathogenic STRs.

#### Overview

The genome-wide polymorphic STR catalog is a comprehensive STR catalog focused on functional STRs generated using population sequencing data. It is the catalog to use if you would like to analyze STRs genome wide. For more details about how genome-wide polymorphic STR catalog differ from other catalogs and how it was generated. You can find more details [here](docs/str_generation.md).

#### Population distribution

To facilitate the use of the catalog, we genotyped STRs across different samples in 1000 Genomes Project using Expansion Hunter 5.0.0. The histograms of genotypes are [here](hg38/genotype/1000genomes). We also summarized polymorphism by population in [documentation](docs/str_diversity_1kg.md).

#### Folder structure and file format

* `hg38/` catalog in json format in hg38
* `hg19/` catalog in json format in hg19

#### File format

* Catalogs are stored in json format as specified in [Expansion Hunter](https://github.com/Illumina/ExpansionHunter/blob/master/docs/04_VariantCatalogFiles.md).

## Contributors

* Yunjiang Qiu
* Viraj Deshpande
* Pavel Avdeyev
* Egor Dolzhenko
* Michael A. Eberle

## Contacts 

If you have any questions or suggestions, you can either create an issue or reach me by [email](mailto:yqiu@illumina.com). 

## License

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
