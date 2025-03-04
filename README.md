<big> **The presented RandomForrest.Rmd script is used to develop a predictive model for the Quantitative Structure-Activity Relationship (QSAR) of a set of advanced nanomaterials. The data used in the analysis is located in input_file.csv. The code is regularly updated to add further steps of analysis.** <big/>

<big> **Website presenting code and results: https://michalinalaura.github.io/MachineLearning/.** <big/>

The data were collected based on scientific publications. 
The independent variables include the dose (µg/mouse), duration of exposure (in days) to the nanomaterial, as well as the aspect ratio (the ratio of length to diameter) and BET_SSA (specific surface area measured using the Brunauer-Emmett-Teller method). The dependent variable is DNA damage in bronchoalveolar lavage (BAL) fluid, expressed as the percentage of DNA strand breaks (TDNA%). DOI: 10.3390/nano13061059; 10.1021/acsnano.9b08818; 10.1016/j.taap.2019.114830; 10.1093/mutage/gew046; 10.1177/0960327118774910; 10.1080/17435390.2022.2106906; 10.1002/em.21888; 10.1080/17435390.2019.1654004; 10.1016/j.etap.2019.103266; 10.1016/j.etap.2019.103303.

**In addition to the predictive model, the code includes a multivariate data analysis essential for understanding the data structure.**

The code is written in a highly versatile manner, facilitating its use with other datasets while maintaining the appropriate structure of the input file.  
The R code requires an input data matrix in .CSV file format, which should be placed in the same directory as the R script file. The decimal separator should be a comma. The matrix should be arranged as follows:
* the first column should contain the names of the compounds,
* the following columns should contain the descriptor values (independent variables),
* the last column should represent the experimental toxicity (dependent variable).

<big>**Example:**<big/>

|Name|  Descriptor(1) | Descriptor(2) | Descriptor(3) | ... | Descriptor(x) |  Responce |
|----|----------------|---------------|---------------|-----|---------------|---------- |
| AB |      12,0      |      0,23     |       1       | ... |      1,0      |    3,5    |       
| CD |      45,5      |      0,30     |       2       | ... |      1,2      |    4,5    |
| EF |      46,3      |      0,67     |       1       | ... |      1,0      |    4,7    |
| GH |      34,9      |      0,24     |       1       | ... |      1,3      |    3,2    |
| IJ |      56,7      |      0,31     |       2       | ... |      1,5      |    5,5    |
|... |      ...       |      ...      |      ...      | ... |      ...      |    ...    |
| YZ |      45,5      |      0,80     |       1       | ... |      1,4      |    3,7    |

