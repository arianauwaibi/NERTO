# Installing and Using CoverM in Nautilus 

## Installing CoverM
>*CoverM can only be used in Linux*

`conda update conda`

[![Anaconda-Server Badge](https://anaconda.org/bioconda/coverm/badges/installer/conda.svg)](https://conda.anaconda.org/bioconda)

`conda install -c bioconda coverm`

To comfirm CoverM was properly installed
`coverm --help`

## Using CoverM

CoverM contig usage: 

Proper syntax

1. Main Command (coverm)
2. Sub Command (contig)
3. 

Input the Pair Ended Reads

**Forward FASTA/Q file**
`coverm -1 <the path>`

Sample 134807 Read 1 Path: 
/home/jovyan/Sample_134807_R1_trim.fastq.gz

`coverm -1 /home/jovyan/Sample_134807_R1_trim.fastq.gz`

**Reverse FASTA/Q file**
`coverm -2 <the path>`
/home/jovyan/Sample_134807_R2_trim.fastq.gz


**Company Example**
$ coverm contig --coupled read1.fastq.gz read2.fastq.gz --reference assembly.fna


coverm contig -1 Sample_134807_R2_trim.fastq.gz --reference 
