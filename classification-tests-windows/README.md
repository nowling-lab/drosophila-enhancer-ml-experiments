# Sequence Model Experiments
This folder contains a Snakemake pipeline and associated scripts for:

1. Extracting peak sequences
2. Sampling control sequences
3. Performing chromosome-level cross-fold validation on sequence models

for _Drosophila melanogaster_ ATAC, DNase, FAIRE, H3K27ac ChIP, H3K43me1 ChIP, H3K4me3 ChIP, STARR, and STARR-Seq data.

## Running

You should have the following Python libraries installed:

* Pandas
* Scikit learn
* Matplotlib
* Seaborn
* Numpy
* Scipy
* Snakemake

Download version r6.45 of the _Drosophila melanogaster_ genome (all chromosomes) and add to the `input` folder with the name `genome.fa`.

To run the pipeline:

```bash
$ snakemake --cores 24 run_experiments
```

where cores can be 24 or less.
