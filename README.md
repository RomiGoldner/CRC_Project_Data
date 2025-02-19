# Colon Cancer Project Data (Descriptor)

This project involves the analysis of immune repertoire data obtained from the blood samples of 205 newly diagnosed colorectal cancer (CRC) patients before any treatment. The dataset comprises T-cell receptor (TCR) sequences for both alpha (TRA) and beta (TRB) chains, generated by repertoire sequencing (Rep-Seq). A key focus of this work is the detailed profiling of the hypervariable CDR3 region, which plays a critical role in antigen recognition and the specificity of the immune response. In addition, patients were classified according to the TNM staging system, and this clinical metadata has been integrated with the TCR data.

![image](https://github.com/RomiGoldner/CRC_Project_Data/blob/2ba32b2025a866b8a412bda19bf820a6185e1fb0/Figure_1_pipeline.png)

## Data Collection and Processing

1. **Blood Collection:**
   - Blood samples were obtained from pre-treatment colorectal cancer patients.

2. **Repertoire Sequencing (Rep-Seq):**
   - Repertoire sequencing was performed on the collected blood samples to obtain TRA and TRB sequences.
     
3. **Data Processing with MiXCR:**
   - Raw sequencing data were processed using the MiXCR pipeline.

4. **Concatenation of TRA and TRB Files:**
   - Processed TRA and TRB files were concatenated to facilitate further analysis.
  
5. **Metadata Integration**
   - TNM staging information was added to the repertoire data to provide additional clinical context.
     
## Data Analysis

**initial_immunarch_analysis.Rmd:**
  - The `immunarch` package was used to perform an initial analysis of the TCR repertoire data. This analysis generated key statistics such as clone count, average clone count per sample, clonotype count, and average clonotype count per sample for both alpha and beta chains.

- **Downsampling_Script.Rmd:**
  - This script subsamples the data to retain only high-quality samples with sufficient clone counts for further analysis.
 
- **CRC_immunarch_analysis.Rmd**
   - This script compares unique clonotypes, clonality, and diversity across samples. The comparisons are based on the TNM stage labels, providing insights into immune repertoire differences among clinical stages.
     
## Installation
1. **Clone the repository:**
   ```sh
   git clone https://github.com/RomiGoldner/CRC_Project_Data.git
2. Requiremtnets:
   - R version XXXX
   - immunarch package version XXXX

## Usage
   - Reproduce the analysis by following the steps outlined in each analysis script provided in the repository.

## Data Availability
XXXXXXXXX
