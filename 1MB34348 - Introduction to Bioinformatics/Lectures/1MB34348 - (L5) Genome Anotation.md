
___
> Author: <span class="name">Sam Hurenkamp</span>
> Tags: #Evergreen/Seedling #lecture #bioinformatics 
> Last modified: `$= dv.current().file.mtime`

<div class="f-info">
	<div class="course-code">
		<span class="fheader"> Course Code </span> <br/>
		<span class="fbody"> 1MB34348 </span>
	</div>
	<div class="discipline">
		<span class="fheader"> Discipline </span> <br />
		<span class="fbody"> Bioinformatics </span>
	</div>
	<div class="date">
		<span class="fheader"> Created</span> <br />
		<span class="fbody last-modified"> 2023-09-2019 </span>
	</div>
</div>
___

### Definition
___
- **Also called DNA annotation**
- It is the next step after sequencing the genome/DNA.
- Aims to determine what part of a genome is a coding sequence and which is non-coding. Start and stop codons are also identified. Function is identified.

# Major parts of gene annotation
___
- [[Structural genome annotation]] 
	- Step 1: Identify portions of the genome that do not code for genes
	- Step 2: Gene prediction/Gene finding
- [[Functional genome annotation]]
	- Step 3. Infer biological information/function to these elements.

#### What to look for?
___
- Protein-coding ([[Exons]]/[[Intron]])
- [[UTR]]
- Promoters, regulatory elements

![[Pasted image 20230919102303.png|center-align]]


- Repeats(Generally masked, you want to get rid of them as they “screw up things")
	- Low-complexity regions (homopolymers
	- Tandem repeats
	- Transposable elements (LINEs, SINEs)

#### Tandem repeats
____
Repeat: A segment of DNA that occurs more than once in the genome (~50% human genome is comprised of repeats)
- Repeat-rich genomes will have negative impact on genome assembly
- The repeated element is collapsed into a single contigs
- Nuisance for reliability and genome assembly
___
**The law of repeats**: It is impossible to resolve repeats of length $S$ unless you have $reads>S$
___

Repeat-rich genomes will also have a negative impact on genome annotation if left unmasked (A,T,G,C -> N’s or a,t,g,c)

<u>For example:</u>
- Generates millions of spurious BLAST hits
- [[Open-Reading Frame (ORF)]]s in transposons can be wrongly annotated as additional
exons

###### Two approaches to identify repeats:
___
- Similarity search vs repeat libraries (e.g. RepeatMasker)
- <i>de novo</i> identification (identification of repeated sequences)

## Gene Annotation
___
![[Pasted image 20230919102901.png|center-align]]

### Take home message
___
When looking for genes, you need to know about the organism and what to expect in the organism

e.g., Eukaryotes vs. Prokaryotes (See below):
![[Pasted image 20230919103308.png|center-align]]

___
To-do: write notes on: [[Reading Frame]]
___


- [[Expressed sequence tag (EST)]]

## Workflow
___
1. Sequence cDNA with short-reads
2. Gene prediction with mRNA evidence (?)
3. Combine 2. with Protein evidence
4. Combine annotation resulting from synthesize all available evidence and map it back to the genome.

## Annotation: the different approaches
___
- Similarity-based methods
- <i>Ab initio</i> prediction
- Hybrid approaches

### Similarity-based approach
___
<u>Strength</u>
-  Produce biologically relevant predictions
- Produce evidence useful for
ab initio tools, pipelines
<u>Weaknesses</u>
- Lowly expressed transcripts are hard to catch
- Transcriptome assembly errors


### Hidden-marker models
___
![[Pasted image 20230919104525.png | center-align]]


### Transition probabilities
___
![[Pasted image 20230919104651.png | center-align]]


![[Pasted image 20230919105455.png | center-align]]

> Emission probabilities: The probability of observing/deducing something about the state from the observed trait.

[[Viterbi algorithm]] solves in linear time
A very important key to the success of HMM!


![HMM](https://www.youtube.com/watch?v=J_y5hx_ySCg)




### The most simple HMM gene predictor
___
HMM works well for gene prediction because genes have a sequential structure.

Given a stretch of DNA, where are the coding and non-coding regions?
<u>Observables</u>: DNA sequence (nucleotides – 1 at a time)
<u>Hidden states</u>: coding and non-coding regions ⇽ This is what we want to infer






