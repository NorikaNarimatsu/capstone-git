# capstone-git

## Project Brief

### Title: 
Reviewing Japan’s most significant competitive grant Grants-in-Aid for Scientific Research system, and evaluating the effect of grants on the scientific output.

### Main DataBase: 
KAKEN: https://kaken.nii.ac.jp/en/
 
### Commitee Meeting Presentation: 
https://docs.google.com/presentation/d/11vF7CntUp0up9PLgaykhg7BZwxxWdS1SVYq3OdfrjLY/edit#slide=id.g15e36913df0_0_106

## File Information: 

# 1_download_xml_files.ipynb: 
The file to download all xml files between 1964 and 2022 from KAKEN
# 2_parse_master.ipynb: 
This is the file to parse KAKEN master repository and upload extracted data to mariadb.
# 3_parse_grantaward.ipynb: 
This is the file to automatically store all projects between 2000 and 2022 to local MariaDB by using KAKEN API. 
# Categoryc_trend.ipynb: 
To plot the general trend of category C.
# RDD_analysis / RDD_cleaning .ipynb: 
The file to clean the data for RDD analysis and pring descriptive statistics (not very commented or organized yet)
# api_test.ipynb: 
This is the main submission for the midterm deliverable assignment. In this file, I conducted the following things: (1) downloading the KAKEN dataset via API, (2) converting the JSON file into Pandas Dataframe, (3) parsing JSON file and getting DOI information, (4) getting ISSN information based on DOI information by using crossref API, (5) getting Impact Factor based on ISSN by using ImpactFactor() (Attempted but failed)

# crossrefdoi_api_practice.ipynb: 
This is the python file in which I tried several things with the crossref API module. I used the DOI of Prof.Hadavand's paper, and it worked!
# KAKEN_api_practice.ipynb: 
This is the python file in which I practiced the KAKEN API definition.
# method1_kaken.json : 
This json file is manually downloaded from the KAKEN dataset. It only contains the information of 7 researchers. I compared this dataset and another dataset, which was downloaded via API. These two files are matched, and you can confirm it in api_test.ipynb file
# df_main_product.csv: 
I could only upload this dataset. This data combines basic researcher information and research output method by awardnumber. 
