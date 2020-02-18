# 17 specific siRNA hitting 9 loci of COVID-19
An RNAi pipeline is applied to the genome of SARS like corona virus COVID-19 (Wuhan-HU-1; NC_045512) yielding 17 candidate siRNA sequences potentially useful for nebulization therapy.

# Methods
1) Generated all 21mers for the human genome transcriptome gencodev33 and the COVID-19 coronavirus (WH1; https://www.ncbi.nlm.nih.gov/nuccore/NC_045512) 
2) Found all 21mers that were in the WH1 genome and not the human transcriptome
3) filtered the remaining 29,854 21mers into those that did not contain 5,4,3, or 2 stretches of bases (n=27951,22303,9351,123 resp.)
  These kmers should not be easy to inhibit with homo-polymer sequences at 5',3' or internal sites 
4) Proceeded with the n=123 21mers to back compare against the entire NT database (all of life) for 

  4.1) circular top hits back to a coronavirus and 
  
  4.2) with a complete 21 bp alignment (see Wuhan_specific_21mers_nodimers.xlsx)
  
5) Of the 17 nucleotide aligned candidates left, put the sequences through a thermodynamic nearest neighbor analysis for off target binding
  
6) Inspected the distribution of target sites on the annotated Wuhan-Hu-1 genome for the targeting sites (see WH1.png). These 21mers hit 9 distinct locations across the COVID-19 genome

7) Displaced the siRNA sequence allowing comparisons for all kmers ignoring G,U, and T bp recorded lowest free energy of off target and sequence to assess the genes that might be off-targets  - see dataset (siRNA_df.tsv)

8) Investigated the genes of all off target energies for the displaced siRNA sequence - see dataset (siRNA_genes_df.tsv). Every gene hit by a signifi8cant binding energy is evaluated for protein coding genes expressed in the lungs, and blood for potential unintended off-target effects. 
 
9) Release of the off-target gene stats 
 
10) Report Final selection for siRNA chemistry - Targets.seq

So these siRNA oligos are available for clinical research testing against cases that are not responding to vaccines or other therapy. The sequence plus the antisense RNA can be ordered (sources below) and annealed together in a suitable sterile physiological buffer to generate siRNA in a deliverable vapor form and taken into the lungs.

see Simple Clinical Delivery Methods below

# Sequence Sources:
sequences can be ordered here:
https://www.thermofisher.com/order/custom-genomic-products/tools/sirna/
or here:
https://horizondiscovery.com/en/products/tools/Custom-siRNA
or ...

# Simple Clinical Delivery Methods 
and see:
https://www.jstage.jst.go.jp/article/cpb/64/1/64_c15-00615/_pdf/-char/en
https://www.amazon.com/gp/product/B0832VKS79/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1

# RNA References
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC387140/pdf/pnas00328-0108.pdf
