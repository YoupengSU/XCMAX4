1. Function: XCMAX4.
    This function is used to test the association between an X chromosomal marker and a binary trait.

2. Arguments of the function
   data: The data should contain the information of phenotype, genotype, sex, and possible additional covariates . Each row represents the data of a specific individual.
   The first column records the phenotype information, with 1 representing the case and 0 representing the control.
   The second column provides the genotype information, with 0, 1 and 2 representing the number of risk alleles.
   The third column contains the sex information, with 0 being male and 1 being female.
   The remaining columns records the information of possible additional covariates.


3. Example dataset: han.csv 
    This dataset is obtained from a two-stage GWAS, which is studying if the SNP rs3827440 is associated with the Graves' disease.
    The data contain four columns. The first column is the phenotype, the second column is the genotype, the third column is the sex information, and the last column represents the stage, with 0 being 
    stage Ⅰ and 1 being stage Ⅱ.

3. Example code

## Read the han data
     data <- read.csv("han.csv")

## run the functon: XCMAX4
    source ("XCAMX4.R")
     XCMAX4(data)
