
## Capstone Thesis Repository

## Research question:
*What is the impact of flexible funding system implementation in KAKENHI on scientific outputs?*

## Data Sources:
The grant information for KAKENHI is available through a public database, KAKEN, provided by the National Institutes of Informatics. This database provides information on research projects supported by the KAKENHI program since 1965, such as grant amount, project members, grant category, scientific field, and resulting publications. I obtained the whole dataset as of 29 Nov 2022 and reconstructed it for this study. The final dataset includes approximately 970,000 grants.

The citation information attributed to KAKENHI projects was obtained through the Web of Science. Web of Science database provides citation reports for academic papers, including the citation impact of individual articles, authors, and journals. I obtained the citation reports for resulting publications for my analysis as of 1 Feb 2023. The final dataset includes approximately 10,000 citation reports.


## Repository Structure:

**Main Directory**
| folder | Content |
| ------------- | ------------- |
| Code | Contains the code to download the data from KAKEN and the code for RDD and DiD |
| Data | Contains all data used for RDD and DiD |
| External Sources | Contains all requirements (necessary for PyWebIO sharing) |

**Code/analysis_code/**
| File | Content |
| ------------- | ------------- |
| DiD.ipynb| Code to conduct Difference-in-Diffrences Design|
| RDD.ipynb | Code to conduct Regression Discontinuity Design|
| datacleaning.ipynb | Code to compile the raw data and create the cleaned dataframe for analysis)|

**Code/database_code/**
| File | Content |
| ------------- | ------------- |
| 1_download_xml_files.ipynb| Code to downloading all research projects XML files from KAKEN|
| 2_parse_master.ipynb | Code to store KAKEN Master Documents to local MariaDB |
| 3_parse_grantaward.ipynb | Code to store all projects between 2000 and 2022 to local MariaDB|

**External Sources**
| File | Content |
| ------------- | ------------- |
| KAKEN_definition(API,JSON,XML) | PDF files that contains the definition of master data |
| grants_masterxml_kaken |  XML files of the master data for KAKEN |

## Working Environment
1. You need to register to use CiNii Web API to get the data from KAKEN database. 
See https://support.nii.ac.jp/ja/cinii/api/developer for details. After the registration is completed, you will be notified of the appid by email. 
 
2. Need to install MariaDB locally and keep running while coding. 

## How to Run the RDD and DID analysis 
Before running, RDD or DiD analysis, you first have to parse KAKEN data and save it to a local MariaDB database. 


Step1. clone the repository
```
git clone [https://github.com/NorikaNarimatsu/capstone-git]
```

Step2. Run the code in database_code in the order

Step3. Parse KAKEN master Data and KAKEN Grant Data to MariaDB

Step4. Run the datacleaning file in analysis_code 

Step5. Run the RDD or DiD file.


## Dependencies

- Python 3.6 or higher
- Jupyter Notebook
- pymysql
- requests
- lxml
- pandas

## License

Copyright (c) 2022  Narimatsu, N.
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Cite
Narimatsu, N.(2022). Effects of flexible funding system implementation in scientific grant: a case study of Japanese competitive research grant, KAKENHI.
