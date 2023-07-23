# Resources for GWAS (statistical genetics)

This repository contains resources needed for analyzing [GWAS](https://www.ebi.ac.uk/training/online/courses/gwas-catalogue-exploring-snp-trait-associations/what-is-gwas-catalog/what-are-genome-wide-association-studies-gwas/) data.


The content of this repository:

* Online learning material
* Interesting articles
* Publicly available genetic data (raw or summarized)
* Tools to perform statistical analyses on genetic data



### Online learning material

* Access course material [here](https://drive.google.com/file/d/1srSMRG-M-7_23ZaXVJ-oLmm_T1sSSGxP/view) by [Abdel Abdellaoui](https://twitter.com/dr_appie).

* [**Lectures** at the Broad Institute](https://www.youtube.com/playlist?list=PLlMMtlgw6qNjROoMNTBQjAcdx53kV50cS), for example the one by [Hilary Finucane](https://www.youtube.com/watch?v=mivyklWDtBI).

* The Broad Institute has some [recordings](https://sites.google.com/broadinstitute.com/onlinejournalclub/other-genetic-presentations?authuser=0) from the **"Medical Population Genetics Program"**

* [This](https://sites.google.com/broadinstitute.com/onlinejournalclub) online **journalclub** from the Broad Institute is not active anymore, but has some nice recordings.


### Articles in Statistical Genetics

##### Integration of omics data

- [Integration of summary data from GWAS and eQTL studies predicts complex trait gene targets](https://www.nature.com/articles/ng.3538); Zhihong Zhu, Futao Zhang, Han Hu, Andrew Bakshi, Matthew R Robinson, Joseph E Powell, Grant W Montgomery, Michael E Goddard, Naomi R Wray, Peter M Visscher & Jian Yang. 2016.

- [Integrating Gene Expression with Summary Association Statistics to Identify Genes Associated with 30 Complex Traits](https://www.cell.com/ajhg/fulltext/S0002-9297(17)30032-0); Nicholas Mancuso, Huwenbo Shi, Pagé Goddard, Gleb Kichaev, Alexander Gusev, Bogdan Pasaniuc. 2017. 

- [trans-eQTL blogpost by Greg Gibson (2021)](http://genomestake.blogspot.com/2021/09/ninety-third-take-trans-eqtl-finally.html).

##### Mendelian randomisation

- [Mendelian randomization with invalid instruments: effect estimation and bias detection through Egger regression](https://doi.org/10.1093/ije/dyv080); Jack Bowden, George Davey Smith, Stephen Burgess. 2015. *MR-Egger Regression and how it deals with pleiotropy and invalid IV.*

- [Mendelian randomization: genetic anchors for causal inference in epidemiological studies](https://doi.org/10.1093/hmg/ddu328); George Davey Smith, Gibran Hemani. 2014. *Overview of MR and its extensions.*

- [Mendelian Randomization Analysis With Multiple Genetic Variants Using Summarized Data](https://doi.org/10.1002/gepi.21758); Stephen Burgess, Adam Butterworth, Simon G. Thompson. 2013. *MR using summarised data, introduces the various MR methods like IVW, likelihood-based and talks about weak instruments and winners curse. Interesting things to know at the start.*

- [Recent Developments in Mendelian Randomization Studies](https://doi.org/10.1007/s40471-017-0128-6); Jie Zheng, Denis Baird, Maria-Carolina Borges, Jack Bowden, Gibran Hemani, Philip Haycock, David M. Evans, George Davey Smith. 2017. *A very well rounded review on MR, more detailed than the first listed article, recent (late 2017) and discusses applications, limitations, and different extensions of MR.*


### Data access

##### Individual level data

- [**HapMap Project**](https://www.sanger.ac.uk/resources/downloads/human/hapmap3.html) phase III includes sequencing data from 1'397 individuals, 11 ancestry groups → his database is [not maintained](https://www.ncbi.nlm.nih.gov/variation/news/NCBI_retiring_HapMap/) anymore. <!-- phase one 270 individuals -->
- [**1000 Genomes Project**](http://www.internationalgenome.org/): phase III contains sequencing data from 2'504 individuals, from 26 populations, for 84.4 million variants markers → publicly available data.
- [**UK10K**](http://www.uk10k.org/): sequencing data from 4000 individuals of European/British ancestry → restricted access. 
- [**UK Biobank**](http://www.ukbiobank.ac.uk/): genotype and genotype imputed data for 500K individuals → restricted access.
- [**African Genome Variation Project**](https://www.nature.com/articles/nature13997) Dense genotypes from 1'481 individuals + WGS from 320 individuals across sub-Saharan Africa → restricted access.
- [**OpenSNP**](https://opensnp.org/): Uploaded genotype and phenotype data from direct-to-consumer genetic tests → publicly available data.
- [**gnomAD**](https://gnomad.broadinstitute.org/): Summary statistics (allele frequency) available through exome and genome sequencing of 71,702 individuals (various disease-specific and population genetic studies, large-scale sequencing projects).

Currently, 1000 Genomes Project and UK10K data are often used as **reference panels** for imputation (except if an online imputation service is used, e.g. the [Sanger Imputation Service](https://imputation.sanger.ac.uk/)). 

##### Summary association statistics

- [**GENEBASS**](https://genebass.org/gene/ENSG00000119737?burdenSet=pLoF&phewasOpts=1&resultLayout=full):Exome-based association statistics, based on  3,817 phenotypes with gene-based and single-variant testing across 281,852 individuals with exome sequence data from the UK Biobank. 
- [**Open Targets Genetics**](https://genetics.opentargets.org)
- [**GWAS Atlas**](http://atlas.ctglab.nl): Comprehensive GWAS catalogue with possibility to compare multiple GWASs (browser).
<!--http://megastroke.org/download.html-->
- [**GWAS Catalog**](https://www.genome.gov/gwastudies/) provides a curated list of all GWAS results, incl [download](https://www.ebi.ac.uk/gwas/downloads/summary-statistics).
- [**gwas.mrcieu.ac.uk**](https://gwas.mrcieu.ac.uk/datasets/): Open GWAS initiative
- [**Pan UK Biobank results**](https://pan.ukbb.broadinstitute.org): Multi-ancestry analysis of 7,221 phenotypes, across 6 continental ancestry groups. 
- [**UK Biobank results**](http://www.nealelab.is/uk-biobank): GWAS summary statistics from genotype imputed UK Biobank data, including 337'000 individuals and 2'419 phenotypes. Based on this, [**UKB phewas**](http://pheweb.sph.umich.edu:5000/) takes a variant id as input and returns the association results for the most relevant phenotypes (browser + download).
- [**Gene Atlas** (UK Biobank GWAS results)](http://geneatlas.roslin.ed.ac.uk/): Associations of 452K UK Biobank White British individuals (browser + download full summary statistics).
- [**Global Biobank Engine**](https://biobankengine.stanford.edu/): Aggregated summary statistics from over 750,000 individuals across three population cohorts: UK Biobank, Million Veterans Program and Biobank Japan (browser).
- [**MR-base**](http://www.mrbase.org/): a web application that displays the result of a systematically performed MR analyses on a number of traits, using > 1000 GWAS summary statistic results. [**MR-base PheWas**](http://phewas.mrbase.org) takes a variant id as input, and returns the traits with relevant MR results as output. 
[**LD-Hub**](http://ldsc.broadinstitute.org/ldhub/): a web application to look up pre-run LD score regression results (browser + download full summary statistics).
- [**eQTL**](https://genenetwork.nl/bloodeqtlbrowser/): Cis- and trans-eQTLs results in whole blood samples, limited to FDR=0.5 (download).
- [**GTEx**](http://www.gtexportal.org/): eQTL summary statistics from over 40 tissues (browser + download full summary statistics).
- [**EBI eQTL catalogue**](https://www.ebi.ac.uk/eqtl/Datasets/) lists a variety of eQTL studies using standardized analyis (download full summary statistics).
- Table 1 in [Pasaniuc & Price (2017)](https://www.nature.com/articles/nrg.2016.142) lists publicly available summary statistics.

##### Download
Places to find full genome summary statistics:
- [**GWAS Catalog**](https://www.genome.gov/gwastudies/) 
- [GWAS Summary Statistics by ctg.cncr.nl](https://ctg.cncr.nl/software/summary_statistics)
- dbGap




