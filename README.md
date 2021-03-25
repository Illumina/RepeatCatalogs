# STR Catalogs

Short tandem repeats (STRs) are genomic sequences comprised of repetitions of a short motif (typically 2-6bp). Many STRs are implicated in a variety of genetic disorders, such as Huntington's disease, amyotrophic lateral sclerosis (ALS), and fragile X syndrome. Thanks to recent improvements in Next-Generation Sequencing (NGS) technologies and computational methods (e.g., ExpansionHunter), it is now possible to identify large expansions of STRs using Whole Genome Sequencing (WGS).

Accurate repeat genotyping requires a high-quality STR catalog that specifies reference coordinates and structure of each locus. Here, we generated multiple STR catalogs that can facilitate analysis of STRs. 

## Documentation

### Analyze STRs using ExpansionHunter

The way to use the catalog is to genotype STRs in the catalog in WGS data using [ExpansionHunter](https://github.com/Illumina/ExpansionHunter). We provided a quick [introduction](docs/usage.md) to do that.

### Catalogs

We generated multiple STR catalogs that contain mutually exclusive set of STRs using difference approaches to serve different purposes. 

* [pathogenic STR](pathogenic_STR/) contains 40+ known pathogenic STRs. 
* [polymorphic STR](polymorphic_STR/) contains genome-wide STRs that are polymorphic across populations. 

### Truthset

We generated truthsets of STR catalogs in NA12878 using PacBio CCS reads. Details of the method can be found [here](docs/truthset.md).

## Folder structure and file format

Each catalog has its own folder and there are multiple folders within it. Details can be found [here](docs/files.md). 

## Contributors

* Yunjiang Qiu
* Viraj Deshpande
* Pavel Avdeyev
* Egor Dolzhenko
* Michael A. Eberle

## Contacts 

If you have any questions or suggestions, you can either create an issue or reach me by [email](yqiu@illumina.com). 

## License

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg