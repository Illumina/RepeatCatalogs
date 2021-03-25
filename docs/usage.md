# Analysis of STRs using STR catalogs

The most straightforward and common way to use the STR catalog is to estimate the sizes of STRs using [ExpansionHunter](https://github.com/Illumina/ExpansionHunter). ExpansionHunter is a tool to estimate STR sizes based on short reads data, and the json format of the catalog can be directly used by ExpansionHunter.

## Usage

For detailed usage about ExpansionHunter, you can refer to the [ExpansionHunter documentation](https://github.com/Illumina/ExpansionHunter/tree/master/docs). Briefly, you only need the BAM/CRAM file from the sample you need to analyze and the fasta file of the reference genome. Catalogs can be found in either [pathogenic STR](../pathogenic_STR/) or [polymorphic STR](../polymorphic_STR/) depending on the needs. 

After getting all the files ready, simply run

```bash
ExpansionHunter --reads <BAM/CRAM file with aligned reads> \
                --reference <FASTA file with reference genome> \
                --variant-catalog <JSON file specifying variants to genotype> \
                --output-prefix <Prefix for the output files>
```

## Running time

For pathogenic STRs, it can be analyzed using ExpansionHunter pretty fast in default seeking mode (typically a few minutes). For polymorphic STRs, it is preferred to use streaming mode in ExpansionHunter so it can be analyzed in <90 minutes. But it does require ~90G memory. If you don't have the memory capacity, you can also split the catalogs and run them in parallel.
