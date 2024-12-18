# EMotEP: **E**arlham **Mot**if **E**xtrapolation **P**ipeline

EMotEP is a Snakemake based pipeline developed to lift-over regulatory motif annotations drawn from ChIP-seq data. The pipeline is designed to use data from well annotated model species, and lift-over to species which have annotated genomes but no regulatory motif annotations.

## Documentation

The full documentation for this pipeline is available on [readthedocs](https://emotep.readthedocs.io/)

## Description

The pipeline works by extracting putative, user defined, regulatory regions from all annotated genes in a genome. Based on user defined orthology information, the putative regulatory region of each gene is then scanned for sequences which match ChIP-seq peaks in the model species orthologue. Based on all sequence matches across the genome, the motif for each transcription factor is redefined based on the matching sequences retrieved from the non-model target species.

### Pipeline Digram

<img src="https://github.com/bibionid/EMotEP/blob/working_version/docs/dag.svg" width="600"/>

## Acknowledgments

[GTRD Database](https://gtrd.biouml.org/)


## Developers
- Will Nash
- Tarang Mehta
- Padhmanand Sudhakar
- Wilfried Haerty

## Contributors

- Federica DiPalma
- Tamas Korcsmaros
