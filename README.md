# TCGA_Survival

The Kaplan Meier estimate is an important methodology in disease research. It is used to estimate the probability that a patient will undergo a defined clinical event. In these two examples, the events are Overall Survival (for lung cancer) and Disease Free Survival (for prostate cancer). The lung and prostate cancer patients are grouped by the number of copies of the genes CCT3 and PTEN that they express; measured as copy number alteration (CNA).

To run these scripts you need to download the following files for your cancer of choice from https://www.cbioportal.org/ and place in your working directory:

data_clinical_patient.txt > contains the survival information for patients
data_clinical_sample.txt  > you want to work with patient rather than sample level information, however the CNA data works with sample level identifiers                               and this file is needed to convert between the two
data_cna.txt              > measurements of CNA for each gene in each sample

Currently, the scripts do not use a configuration file, therefore you will need to change all instances of the example genes to your favourite gene. This can be done easily with the find and replace all option in RStudio.

## PTEN loss in Prostate Cancer

The tumour supressor gene PTEN is one of the most commonly lost genes in prostate cancer. Here the "DFS" script determines if loss of PTEN copy number is able to estimate if a patient with prostate cancer is likely to progress with their disease. This progression is measured by DFS as the event.

The example uses TCGA-PRAD (PanCancer Atlas: Prostate Cancer data from c-bioportal)

![PTEN_Prostate](https://user-images.githubusercontent.com/18528125/173326883-d38594b8-9ef1-4f4a-9aa3-4712eb550af6.png)

## CCT3 loss in Lung Squamous Cell Carcinoma

The tumour supressor gene PTEN is one of the most commonly lost genes in prostate cancer. Here the "DFS" script determines if loss of PTEN copy number is able to estimate if a patient with prostate cancer is likely to progress with their disease. This progression is measured by DFS as the event.

The example uses TCGA-LUSC (PanCancer Atlas: Lung Squamous Cell Carcinoma data from c-bioportal)
