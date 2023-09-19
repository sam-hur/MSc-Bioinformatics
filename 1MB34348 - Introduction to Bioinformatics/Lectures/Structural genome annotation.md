---
tags:
  - Evergreen/Seedling
  - definition
  - bioinformatics
---

## Definition
___
Find out where region of interest are in the genome and what they look like. 

**It is used for the identification of genomic elements, as well as what portions of the genome do/do not code for genes** (coding region vs. non-coding regions).

This helps narrow down the genome to a smaller region of interest (e.g., through gene mapping) and discover the exact sites of the gene where [[exon]]s are located and are ultimately coded into proteins.

Furthermore, this helps in gene prediction/gene finding (to discover which part of the gene is a coding/non-coding region).

- Coding regions are [[exon]]s
- Non-coding regions are [[intron]]s and intergenic regions


Consists of:
1. [[Open-Reading Frame (ORF)]]
2. Gene Structure
3. Location of regulatory regions/motifs
4. identifying coding/non-coding regions


Precursor to [[Functional genome annotation]]

###### Genomic Elements
___
The identification of genomic elements may include genes, regulatory elements, repetitive (repeated) sequences, and more.

##### Identification for non-coding regions
___
Identify start and stop codon, generally `AUG` (Methionine). Generally, the start region is 20 bp (base-pairs) in length. Stop codon region is present at the end of the gene and is rich in thymine. Normally approx 20-30bp in length.

##### Gene finding - Stepwise approach
___
- expensive process
- done with the help of gene knockout experiments
- gene of interest is knocked out from the animal test subject.
	- Test subject is the used in an observational study to view changes in phenotype.

2. BLAST, FASTA:
	- Find out regions of similarity between the given number of sequences.
	- If a region has very high similarity to mRNA or protein production, then it means that the region observed is a protein-coding gene.

3. Find out [[the pribnow box]] and transcription factor binding sites (for prokaryotes only)
4. Find out the [[Open-Reading Frame (ORF)]].
5. Find out the [[CpG islands]] (in Eukaryotes).
6. Find out the binding sites for a [[Polyadenylate tails]] (poly(A)tail). This represents the end of a gene/[[exon]].
7. 