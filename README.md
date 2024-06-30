# 👨Customer Acquisition Analysis

## Introduction
This project aims to perform exploratory data analysis and hypothesis testing to understand the various factors contributing to customer acquisition. By analyzing the data, we aim to uncover insights that can help improve marketing strategies and customer engagement.

## Objectives
- Perform exploratory data analysis (EDA) to gain insights into customer behavior and preferences.
- Test hypotheses related to customer acquisition factors.
- Use visualizations to support the analysis and findings.

## Dataset Description
The dataset contains variables related to:
- **People**: Birth year, education, income, etc.
- **Product**: Amount spent on wine, fruits, gold, etc.
- **Place**: Sales channels such as websites, stores, etc.
- **Promotion**: Information on promotions and campaign results.

## Methodology
### Data Preparation
1. **Import Libraries and Load Dataset**:
   - Import necessary Python libraries such as pandas, seaborn, matplotlib, feature-engine and sklearn.
   - Load the dataset into a pandas DataFrame.

2. **Data Wrangling and Feature Engineering**:
   - Handle missing values and perform data cleaning.
   - Encode categorical values and create new features if necessary.

### Hypothesis Testing
1. **Normality Check**:
   - Use the Anderson-Darling test to check for normality.
   - Apply variance stabilizing transformation using PowerTransformer (Yeo-Johnson) to achieve normality.

2. **Hypotheses**:
   - Older people are not as tech-savvy and probably prefer shopping in-store.
   - Customers with kids probably have less time to visit a store and would prefer to shop online.
   - Other distribution channels may cannibalize sales at the store.
   - The US fares significantly better than the rest of the world in terms of total purchases.

3. **Non-Parametric Tests**:
   - Since the dataset was not normalized, use non-parametric tests such as Mann-Whitney U and Kruskal-Wallis for hypothesis testing.

### Exploratory Data Analysis (EDA)
1. **Visualizations**:
   - Use seaborn and matplotlib to create various plots to analyze:
     - Products' performance in terms of revenue.
     - Pattern between age of customers and last campaign acceptance rate.
     - Country with the greatest number of customers who accepted the last campaign.
     - Pattern in the number of children at home and total spend.
     - Education background of customers who complained in the last 2 years.

## Folder Structure
- `data/`: Contains the dataset files.
- `notebooks/`: Jupyter notebooks for data analysis, hypothesis testing, and visualization.
- `src/`: Python scripts for data processing and analysis.
- `api/`: Api code (if any).
- `models/`: Trained models and saved results.
- `docs/`: Output files including visualizations and test results.

## Installation and Usage
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/MariahFerns/HypothesisTesting-CustomerAcquisition.git
   cd HypothesisTesting-CustomerAcquisition

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt

3. Run Jupyter Notebooks:
   Navigate to the notebooks/ folder and open the notebooks to explore data analysis and model development.

4. Run Scripts:
   Use the scripts in the scripts/ folder to preprocess data, perform hypothesis testing, and create visualizations.

## Results and Findings
**EDA Insights:**
- Identified top-performing and least-performing products in terms of revenue.
- Found patterns between customer age and campaign acceptance rates.
- Determined which country had the most customers accepting the last campaign.
- Analyzed the relationship between the number of children at home and total spending.
- Examined the education background of customers who complained in the last 2 years.

**Hypothesis Testing Results:**
- Older people showed a preference for in-store shopping.
- Customers with kids preferred online shopping.
- Other distribution channels had an impact on store sales.
- The US performed significantly better in terms of total purchases compared to the rest of the world.


## Conclusion
This project provided valuable insights into customer acquisition factors through thorough data analysis and hypothesis testing. The findings can help improve marketing strategies and customer engagement.
