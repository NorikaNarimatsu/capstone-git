
# Capstone Thesis Repository

## Effects of flexible funding system implementation in scientific grant: a case study of Japanese competitive research grant, KAKENHI.
*Minerva University Capstone Project*

## Research question:
*How can we effectively communicate the extent and depth of global inequality using data visualizations and summary statistics?*

## Data Sources:
Although we acknowledge that reducing global inequality requires high-level transformative changes with appropriate political and economic policies, there are several things we can do at the individual level. Thus, we aim to explore the effects of global inequality across different levels of analysis (international, regional, and national) globally for four topics: health, income, environment, and education. Although it is by no means a complete list of topics where global inequality is present, we believe it is a solid start to start educating the general audience.


## Repository Structure:

**Main Directory**
| folder | Content |
| ------------- | ------------- |
| quiz_game.py | Contains the actual PyWebIO application |
| requirements.txt | Contains all requirements (necessary for PyWebIO sharing) |

**data/Final/**
| File | Content |
| ------------- | ------------- |
| Datasets.zip| World Bank Development Indicators raw dataset |
| indicators.csv | Data containing the indicators for the app|
| countries.csv | Data containing values for countries only (exclusing economic status and regions)|
| df_countries.csv | Data containing the list of countries |

**Code**
| File | Content |
| ------------- | ------------- |
| DS4SG_Data_Importing.ipynb| Notebook used to change and filter the data and exctract a final dataset|
| questions.py | Python file used to include the questions & the order of the questions |
| visualizations.py | Python file containing visualizations for the questions |
| Tests.ipynb | Notebook used to create the question in infinite mode |
| Visualization Tests.ipynb | Notebook used to test the visualizations |
| extracting_data.ipynb | Notebook used to filter for a specific topic |
| pyweb_example.py | An example with a score board |

## How to Run the Application Locally
```
# clone the repository
git clone https://github.com/berdikhanova/DS4SG-Global-Inequality.git

# Go to the directory of the repository
cd DS4SG-Global-Inequality

# Install required packages
pip install -r requirements.txt

# Run app
python quiz_game.py
```

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
