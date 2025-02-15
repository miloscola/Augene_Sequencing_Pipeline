![Augene_Beauty_logo](https://github.com/user-attachments/assets/84520cca-6e4a-40f1-8aff-8767a34bc5fb)

## Function:


1. Scraping and downloading microbiome profile data from scientific papers
2. Performing batch correction and data processing
3. Generating microbiome profiles from raw reads
4. Generating a diagnosis from the microbiome profile with machine learning (TODO)

## Krona Graph Showing Microbiome Profile by Taxanomic Level:
![image](https://github.com/user-attachments/assets/b49d1bbc-5312-4a6b-9a10-1e185e901a45)




## Usage:

**Data Scraping:**

Activate the Qiime2 environment and run SKINOME_training_data/data_downloader. This script will download sequencing data from skin microbiome papers listed in DataFrame_2_Pruned. DataFrame_2_Pruned was generated with code modified from the [Skinome Project](https://academic.oup.com/database/article/doi/10.1093/database/baac033/6586378). Papers were filtered to only contain microbiomes classified as healthy, atopic dermatitis, psoriasis, parapsoriasis, or acne. Papers were only included if they used swabs to collect samples and Illumina sequencing for standardization. 

**Microbiome Profile Calculation:**

Activate the Qiime2 environment and run SKINOME_training_data/QIIME2_pipeline. Ensure you have an appropriate classifier in the SKINOME_training_data/classifier folder. For more information on training a classifier, see [this guide](https://docs.qiime2.org/2024.10/tutorials/feature-classifier/). 

**Generate Diagnosis: (TODO)**

Data may lack necessary resolution for proper classification. 

**The data_processing and data_vis folders contain old code**
