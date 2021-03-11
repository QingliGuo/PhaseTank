# PhaseTank

## Introduction

Phase siRNAs (phasiRNAs) are a class of small RNAs, which triggered by miRNA-targeted cleavage and followed by DCL4-mediated production of small RNAs phased in 21-nt increments.

Here, we introduce PhaseTank to systemically characterize phasiRNAs/tasiRNAs and their regulatory cascades 'miRNA/phasiRNA -> PHAS gene -> phasiRNAs -> target genes' in plants.

## Usage

PhaseTank is implemented using Perl 5.0, which can be called using one command line. Here are examples about using PhaseTank for four different goals.

+ To predict PHAS loci from the given organism and read libraries
 
```$ perl PhaseTank_v1.pl --genome ath_genome_TAIR10.fa --lib GSM1174496.fa,GSM277608.fa,GSM342999.fa,GSM709567.fa,MTSRNA1.fa,RMMT10.fa```

+ To predict phasiRNAs and search their miRNA-triggered cleavage

```$ perl PhaseTank_v1.pl --genome ath_genome_TAIR10.fa --lib GSM1174496.fa,GSM277608.fa,GSM342999.fa,GSM709567.fa,MTSRNA1.fa,RMMT10.fa --miR ath_miRNA.fa --degradome de_GSM278335.fa –trigger_miRNA```

+ To predict phasiRNAs and their targets

```$ perl PhaseTank_v1.pl --genome ath_genome_TAIR10.fa --lib GSM1174496.fa,GSM277608.fa,GSM342999.fa,GSM709567.fa,MTSRNA1.fa,RMMT10.fa --degradome de_GSM278335.fa --target ath_cDNA_TAIR10.fa --phasiRNA_target```

+ To predict phasiRNAs, search the miRNA-triggered cleavage and detect phasiRNAs targets

```$ perl PhaseTank_v1.pl --genome ath_genome_TAIR10.fa --lib GSM1174496.fa,GSM277608.fa,GSM342999.fa,GSM709567.fa,MTSRNA1.fa,RMMT10.fa --miR miRNA.fa --degradome de_GSM278335.fa --target ath_cDNA_TAIR10.fa --phasiRNA_target```

## Citation

**Guo Q**, Qu X, Jin W. PhaseTank: genome-wide computational identification of phasiRNAs and their regulatory cascades. Bioinformatics. 2015 Jan 15;31(2):284-6. doi: 10.1093/bioinformatics/btu628. Epub 2014 Sep 21. PMID: 25246430.

Click [here](http://phasetank.sourceforge.net/) to reach the original website.
