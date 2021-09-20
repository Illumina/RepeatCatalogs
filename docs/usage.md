# Analysis of STRs using STR catalogs

The most straightforward and common way to use the STR catalog is to estimate the sizes of STRs using [Expansion Hunter](https://github.com/Illumina/ExpansionHunter). Expansion Hunter is a tool to estimate STR sizes based on short reads data, and the json format of the catalog can be directly used by ExpansionHunter.

## Usage

For detailed usage about Expansion Hunter, you can refer to the [Expansion Hunter documentation](https://github.com/Illumina/ExpansionHunter/tree/master/docs). Briefly, you only need the BAM/CRAM file from the sample you need to analyze and the fasta file of the reference genome. Catalogs can be found in either [hg19](../hg19/) or [hg38](../hg38/) depending on the reference. 

After getting all the files ready, simply run

```bash
ExpansionHunter --reads <BAM/CRAM file with aligned reads> \
                --reference <FASTA file with reference genome> \
                --variant-catalog <JSON file specifying variants to genotype> \
                --output-prefix <Prefix for the output files>
```

## Running time

For the genome-wide catalog, it is preferred to use streaming mode in Expansion Hunter v5.0.0 in multi-thread mode so it can be analyzed quickly.
