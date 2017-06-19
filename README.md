# Mutation_burden
Building a pipeline to assess effects of mutation burden
We will calculate clone-specific mutational burden and determine the potential benefit from immunotherapy treatment

Work Flow: 
1) Preprocessing: FASTQ files->BAM and VCF files
2) CNV calling: CNV variants 
3) Mutational burden calculation: SNV calculation per clone of cells (comparison among different tools)
4) Output: Appropriate for immunotherapy or not, which immunotherapy
