# TCGA Survival Analysis Script

The TCGA Survival script utilizes the Kaplan-Meier estimate, a crucial methodology in disease research, to estimate the probability of patients undergoing defined clinical events. Specifically, it focuses on Overall Survival for lung cancer and Disease-Free Survival for prostate cancer.

## Gene-Specific Analysis

The script categorizes cancer patients based on the copy number alteration (CNA) of your gene of interest.The expression levels of these genes, measured through CNA, serve as key factors in patient grouping.

In the example below the genes CCT3 and PTEN are analysed in the context of Lung and Prostate cancers respectively.

## Requirements

Before running the script, ensure you download the necessary data files for your chosen cancer type from [cBioPortal](https://www.cbioportal.org/) and place them in your working directory:

- **data_clinical_patient.txt:** Contains survival information for patients.
- **data_clinical_sample.txt:** Provides patient-level information, crucial for CNA data processing.

## How to Use

1. Download the required data files mentioned above.
2. Set your working directory.
3. Run the function within the script to perform survival analysis on the specified cancer type, considering gene-specific copy number alterations of your gene of interest.

## PTEN loss in Prostate Cancer

The tumour supressor gene PTEN is one of the most commonly lost genes in prostate cancer. Here the "DFS" script determines if loss of PTEN copy number is able to estimate if a patient with prostate cancer is likely to progress with their disease. This progression is measured by DFS as the event.

The example uses TCGA-PRAD (PanCancer Atlas: Prostate Cancer data from c-bioportal)

![PTEN PC](https://user-images.githubusercontent.com/18528125/173332063-d6286cc4-9c33-4bf9-8e85-5e4e40c49435.png)
