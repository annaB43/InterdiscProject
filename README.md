
# Gender Dynamics at Work: Analyzing Trends and Patterns in the US Labor Market


This project aims to analyze gender dynamics in
the US labor market using data spanning 2000 to 2023. In particular, exploratory data analysis and statistical testing are used to examine the trends in gender representation and income disparities across various occupational fields and how they have evolved over time. Furthermore, social network analysis techniques are used to explore occupational mobility for men and women and its connection to income. This analysis provides deeper understanding of gender dynamics in the labor market and offers valuable insights for policy interventions aimed at promoting gender equality in the workforce.

## Project Structure
- `asec_analysis.ipynb`: Jupyter notebook with the data cleaning, preprocessing, EDA and hypothesis testing code.
- `occupational_mobility_analysis.ipynb`: Jupyter notebook with the occupational mobility analysis code using the preprocessed data.
- `IntermediaryResults/`: Directory for storing the intermediary results (the hypothesis test results and social network analysis results).
- `requirements.txt`: List of Python packages required to run the code.
- `README.md`: Project overview and instructions.

## Data Retrieval

Utilize the [IPUMS Online Data Extract System](https://cps.ipums.org/cps/index.shtml):
1. Identify the desired variables to be included in your dataset - *YEAR, SERIAL, MONTH, CPSID, ASECFLAG, HFLAG, ASECWTH, PERNUM, CPSIDV, CPSIDP, ASECWT, ASECWTCVD, AGE, SEX, RACE, MARST, EMPSTAT, OCC2010, EDUC, ASECOVERP, OCC10LY, INCWAGE*
2. Select 24 samples spanning the years 2000-2023.
3. Set the data format to `.csv` and the structure to Rectangular (cross-sectional).
4. After processing, the extract will become available for use.
5. Make a directory `data`, download the dataset and save it in the `data` directory.
6. Additionally, use the accompanying codebook files, which feature the codes and labels of the variables. Convert these files to `.csv` format to facilitate easier access and manipulation during the subsequent stages of analysis. Store them in the `data` directory.
7. The data file is renamed `df_asec.csv` and the labels are named `educ-labels.csv`, `race-labels.csv`, `marst-labels.csv`, `empstat-labels.csv`, `occ2010_labels.csv` for the *EDUC, RACE, MARST, EMPSTAT, OCC2010* variable labels, respectively. These label files have two columns - *Code* and *Label*. You can use these names for consistency. 

## Package Installation

To install the required packages, run the following command:

```bash
pip install -r requirements.txt
```

## Reproducing the Python Analysis

Run the Jupyter notebooks `asec_analysis.ipynb` and `occupational_mobility_analysis.ipynb` in this order to reproduce the analysis.

## Reproducing the Social Network Analysis

Use the generated files and networks in `IntermediaryResults/newtork/` directory in [Gephi](https://gephi.org/) to reproduce the analysis.