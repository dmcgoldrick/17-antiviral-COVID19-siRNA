# Targeting SARS-CoV-2 with siRNA
An RNAi pipeline is applied to the genome of the positive sense RNA, SARS-like corona virus, severe acute respiratory syndrome coronavirus 2 (SARS-CoV-2; Wuhan-HU-1 NC_045512). This is the cause of COVID-19. I found 17 best candidate siRNA sequences potentially useful for nebulization therapy (download Targets.seq to get these siRNA sequences).

# Methods
1) Generated all 21mers for the human genome transcriptome gencodev33 and the COVID-19 coronavirus (WH1; https://www.ncbi.nlm.nih.gov/nuccore/NC_045512) 
2) Found all 21mers that were in the WH1 genome and not the human transcriptome
3) filtered the remaining 29,854 21mers into those that did not contain 5,4,3, or 2 stretches of bases (n=27951,22303,9351,123 resp.)
  These kmers should not be easy to inhibit with homo-polymer sequences at 5',3' or internal sites 
4) Proceeded with the n=123 21mers to back compare against the entire NT database (all of life) for 

  4.1) circular top hits back to a coronavirus and 
  
  4.2) with a complete 21 bp alignment (see Wuhan_specific_21mers_nodimers.xlsx)
  
5) Of the 17 aligned candidates left, put the sequences through a thermodynamic nearest neighbor analysis for off -target binding
  
6) Inspected the distribution of target sites on the annotated Wuhan-Hu-1 genome for the targeting sites (see WH1.png). These 21mers hit 9 distinct locations spread across the viral genome

7) Displaced the siRNA sequence allowing binding comparisons for neighboring kmers (ignoring G,U, and T) recorded lowest free energy of off-targets and the sequence to assess the genes that might be off-target hits in humans  - see dataset (siRNA_df.xlsx)

7.1) ALL potential off-target sites in human transcripts have a predicted free energy change of greater than ~ 11 kcal/mol disfavoring their binding (see Keq ratios in siRNA_df.xlsx). So viral targets are favored more than 10 fold. Unlike other agents for RNAi which globally attack mRNA and have approval from the FDA for ebola and SARS-coV-2, these siRNA agents are unlikely to affect host human mRNA in the lungs and other organs to such a degree as the ebola medication.
 
8) Release of the off-target gene stats 
 
9) Report final selection for siRNA chemistry - Targets.seq

10) Check the conservation of the inital targets against 3928 publicly available complete genome isolates across the globe and by other researchers than Wuhan1/Chinese researchers. All hit SARS2 many hit SARS1, three strains are ancestral max matches wrt the Covid-19 strains: MG772933.1, MG772933.1 MN996532.1
These strains might serve as a consensus for the ancestral origin and analysis of selection/recombination across the SARS2 genome.

11) report all sequences in 5'-3' orientation now that the multialignment confirms the genome.

So these siRNA oligos are available for clinical research testing against cases that are not responding to vaccines or other therapy. The sequence plus the antisense RNA can be ordered (sources below e.g. Megascript  RNAi kit - $472/20 reactions ) and annealed together in a suitable sterile physiological buffer to generate siRNA in a deliverable nebulizable vapor form and taken into the lungs.

# NEW 2020-07-02 Single Line Multiple Alignment of 3928 SARS coV2 isolates
see SARS_COV2_mafft_singleLine.out.gz
This file traces the changes in the SARS virus and is the initial multiple alignment using mafft

# Sequence Sources:
sequences can be ordered here:
https://www.thermofisher.com/order/custom-genomic-products/tools/sirna/

or here:
https://horizondiscovery.com/en/products/tools/Custom-siRNA

or ...
https://www.sigmaaldrich.com/life-science/custom-oligos/sirna-oligos.html

or ...
choose your own

# Cost Effective Lab Production Reference
https://www.thermofisher.com/order/catalog/product/AM1626#/AM1626

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC152823/

# Simple Clinical Delivery Methods 
https://www.jstage.jst.go.jp/article/cpb/64/1/64_c15-00615/_pdf/-char/en

https://www.future-science.com/doi/full/10.4155/tde-2019-0009

https://www.adwdiabetes.com/product/7537/omron-compair-lightweight-compressor-nebulizer?utm_source=google&utm_medium=cpc&utm_campaign=shopping&gclid=EAIaIQobChMIpNv7wrCY6AIV1Rx9Ch30fwAXEAQYAiABEgKAqvD_BwE

https://www.amazon.com/gp/product/B0832VKS79/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1

# RNAi References
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC387140/pdf/pnas00328-0108.pdf
https://www.frontiersin.org/articles/10.3389/fendo.2018.00402/full

# miR-223 reference (promising miRNA that affects ARDS and ALI)
https://stm.sciencemag.org/content/9/408/eaah5360?utm_source=VancePak%20%28updated%206/30/2017%29&utm_campaign=2fa0418255-EMAIL_CAMPAIGN_2017_09_15&utm_medium=email&utm_term=0_56c46682ac-2fa0418255-126546449

# Recent Powerpoint presentation

https://docs.google.com/presentation/d/1QJPAHh0LMmp01nwcUsoS785jvM5FPzEQw8eEfYTQSFI/edit?usp=sharing

For comments please open issues :-)
best,
Daniel J McGoldrick
