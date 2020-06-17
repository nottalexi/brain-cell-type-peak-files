# brain-cell-type-peak-files

H3K27ac/ # Peak files for H3K27ac ChIPseq generated using nuclei from human cortical resected brain tissue enriched for neuron (NeuN), microglia (PU1), oligodendrocyte (olig2) and astrocyte (LHX2) cell type populations.

H3K4me3/ # Peak files for H3K4me3 ChIPseq generated using nuclei from human cortical resected brain tissue enriched for neuron (NeuN), microglia (PU1), oligodendrocyte (olig2) and astrocyte (LHX2) cell type populations.

ATAC/ # Peak files for ATACseq generated using nuclei from human cortical resected brain tissue enriched for neuron (NeuN), microglia (PU1), oligodendrocyte (olig2) and astrocyte (LHX2) cell type populations.

https://pubmed.ncbi.nlm.nih.gov/31727856/
PMID: 31727856 PMCID: PMC7028213 DOI: 10.1126/science.aay0793

Brain Cell Type-Specific Enhancer-Promoter Interactome Maps and Disease - Risk Association

Abstract
Noncoding genetic variation is a major driver of phenotypic diversity, but functional interpretation is challenging. To better understand common genetic variation associated with brain diseases, we defined noncoding regulatory regions for major cell types of the human brain. Whereas psychiatric disorders were primarily associated with variants in transcriptional enhancers and promoters in neurons, sporadic Alzheimer's disease (AD) variants were largely confined to microglia enhancers. Interactome maps connecting disease-risk variants in cell-type-specific enhancers to promoters revealed an extended microglia gene network in AD. Deletion of a microglia-specific enhancer harboring AD-risk variants ablated BIN1 expression in microglia, but not in neurons or astrocytes. These findings revise and expand the list of genes likely to be influenced by noncoding variants in AD and suggest the probable cell types in which they function.

FASTQ-files for ATAC-seq and ChIP-seq were processed with the official ENCODE ATAC-seq (https://github.com/ENCODE-DCC/atac-seq-pipeline) and ChIP-seq (https://github.com/ENCODE-DCC/chip-seq-pipeline2) pipelines, respectively. Both pipelines were installed with a local anaconda environment. The Build_genome_data scripts were run to build the local hg19 reference genome and other dependencies. These pipelines execute a number of programs to process and align sequencing reads and to generate quality control statistics. In brief, FASTQ-files were trimmed with cutadapt (Version 1.9.1) and aligned with Bowtie2 to hg19. SAMtools (Version 1.2), MarkDuplicates (Picard Version 1.126), and bedtools (Version 2.26) were used to filter and clean data post alignment. MACS2 (Version 2.1.1) was used for peak calling. The ATAC-seq pipeline also runs IDR to detect peaks with high reproducibility. The optimal peak sets that came out of these pipelines were used for downstream analysis.
