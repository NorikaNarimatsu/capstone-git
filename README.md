# capstone-git

## Project Brief

### Title: 
Reviewing Japan’s most significant competitive grant Grants-in-Aid for Scientific Research system, and evaluating the effect of grants on the scientific output.

### Main DataBase: 
KAKEN: https://kaken.nii.ac.jp/en/
 
### Commitee Meeting Presentation: 
https://docs.google.com/presentation/d/11vF7CntUp0up9PLgaykhg7BZwxxWdS1SVYq3OdfrjLY/edit#slide=id.g15e36913df0_0_106

## File Information: 
1. **api_test.ipynb**:
This is the main submission for midterm deliverable assignment. 
In this file, I conducted the following things:
(1) downloading the KAKEN dataset via API, (2) converting Json file into Pandas Dataframe, 
(3) parsing json file and getting DOI information, (4) getting ISSN information based on DOI informationby using crossrefapi,
(5) getting Impact Factor based on ISSN by using ImpactFactor() (Attempted but failed)

🚨When you are running this code, you need appid to access KAKEN dataset via API 🚨
You can refgister it from here. https://support.nii.ac.jp/en/cinii/api/developer

2. **crossrefdoi_api_practice.ipynb**
This is the python file, in which I tried several things with crossref api module. I use the doi of Prof.Hadavand's paper and it worked!

3. **KAKEN_api_practice.ipynb**
This is the python file, in which I practiced KAKEN api definition.

4. **method1_kaken.json**
This json file is manually downloaded from KAKEN dataset. It only contains the information of 7 researchers. 
I compared this dataset and another dataset, which was downloaded via API. These two files are matched and you can confirm it in **api_test.ipynb** file
