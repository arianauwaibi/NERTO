# Installing and Using CoverM in Nautilus 

## Installing CoverM
>*CoverM can only be used in Linux*

`conda update conda`

[![Anaconda-Server Badge](https://anaconda.org/bioconda/coverm/badges/installer/conda.svg)](https://conda.anaconda.org/bioconda)

`conda install -c bioconda coverm`

To comfirm CoverM was properly installed
```
coverm --help
```

## Using CoverM

CoverM contig usage: 

Proper syntax

1. Main Command (coverm)
2. Sub Command (contig)
3. file name or path needed for subcommand
4. Any other subcommands needed
5. Reference

#### Input the Pair Ended Reads

**Forward FASTA/Q file**

  `coverm -1 <the path>`

    >The home part of the path does not have be included. Only include the folder the files are in as the path name. `/home/jovyan/` not needed. Command `pwd` can be used in the linux terminal to access the file path. 

**Reverse FASTA/Q file**

  `coverm -2 <the path>`

**Company Example**
  $ coverm contig --coupled read1.fastq.gz read2.fastq.gz --reference assembly.fna

**This code did not give me an error**
coverm contig -1 Sample_134807_R1_trim.fastq.gz -2 Sample_134807_R2_trim.fastq.gz --reference reference_strains/strain_BS13-02.fna.gz
