![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)
# Healthcare Insurance Cost Analysis

## Project Overview

This project analyses a healthcare insurance dataset to explore how personal, lifestyle and geographic factors are related to medical insurance charges.

The aim of the project is to use Python data analysis and visualisation techniques to identify patterns in the dataset and understand which customer characteristics appear to be most strongly associated with higher insurance charges.

## Business Question

Which customer characteristics appear to be most strongly related to higher healthcare insurance charges?

## Real-World Application and Analytics Value

Healthcare insurance providers can use data analytics to better understand which customer characteristics are associated with higher insurance charges. This can support evidence-based decision-making by helping organisations identify key cost drivers, compare customer groups and plan future pricing or risk assessment strategies.

In this project, data analytics is used to explore how factors such as smoking status, age, BMI, sex, number of children and region relate to insurance charges. The findings can help show which variables may be most useful for further analysis or future predictive modelling.

AI could also be used as a future opportunity by building predictive models that estimate insurance charges for new customers based on their characteristics. This could help organisations make faster estimates, identify high-risk groups and support more informed decision-making. However, any AI solution would need to be tested carefully to avoid unfair or biased outcomes.

## Dataset

The dataset used in this project is `insurance.csv`, stored in the `data` folder.

The dataset contains customer information including:

* `age`: age of the insurance customer
* `sex`: gender of the customer
* `bmi`: body mass index
* `children`: number of children/dependants covered by insurance
* `smoker`: whether the customer is a smoker
* `region`: customer region
* `charges`: individual medical insurance charges

The original dataset contained 1,338 rows and 7 columns. After the ETL process, one duplicate row was removed, leaving 1,337 rows and 7 columns.

## Project Objectives

The objectives of this project are to:

* Load and inspect the healthcare insurance dataset
* Check for missing values, duplicates, data types and categorical consistency
* Clean the dataset and save a cleaned version
* Explore relationships between insurance charges and customer characteristics
* Create visualisations using Python libraries
* Identify the factors most strongly associated with higher insurance charges
* Summarise key findings, limitations and possible next steps

## Technologies Used

The project was completed using:

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Jupyter Notebook
* VS Code
* Git and GitHub

## Repository Structure

```text
Healthcare_Insurance/
│
├── data/
│   └── insurance.csv
│
├── jupyter_notebooks/
│   ├── 01_ETL.ipynb
│   └── 02_data_visualisation.ipynb
│
├── outputs/
│   └── cleaned_insurance.csv
│
├── README.md
└── requirements.txt
```

## ETL Process

The ETL notebook loads the raw dataset and checks the data for quality issues before analysis.

The ETL process included:

* Loading the raw `insurance.csv` dataset
* Inspecting the shape, column names, data types and summary statistics
* Checking for duplicate rows
* Removing one duplicate row
* Checking for missing values
* Checking that categorical values were consistent
* Saving the cleaned dataset as `outputs/cleaned_insurance.csv`

No additional transformations were required because the dataset had no missing values, clear column names, suitable data types and consistent categorical values.

## Data Analysis and Visualisation

The data visualisation notebook uses the cleaned dataset to explore the relationship between insurance charges and other variables.

The analysis includes:

* Summary statistics for insurance charges, age and BMI
* Count distributions for sex, smoker status, region and children
* Grouped analysis of average insurance charges by smoking status, sex, children and region
* Visualisations using Matplotlib, Pandas, Seaborn and Plotly

The visualisations include:

* Histogram of insurance charges
* Bar chart of average insurance charges by smoking status
* Boxplot of insurance charges by smoking status
* Scatter plot of age against insurance charges by smoking status
* Scatter plot of BMI against insurance charges by smoking status
* Scatter matrix of numerical variables by smoking status
* Boxplot of insurance charges by region
* Boxplot of insurance charges by sex and smoking status
* Bar chart of insurance charges by number of children and smoking status

## Key Findings

The main findings from the analysis are:

* Smoking status has the strongest relationship with insurance charges.
* Smokers have much higher average insurance charges than non-smokers.
* Insurance charges generally increase with age.
* BMI appears to have some relationship with insurance charges, especially among smokers.
* Region, sex and number of children show some variation in charges, but their relationships are weaker and less consistent than smoking status.
* The number of children does not show a clear pattern where charges increase steadily.

## Limitations

This analysis is based on one dataset, so the findings may not represent all healthcare insurance customers or all healthcare systems.

The dataset also does not include other factors that could affect medical costs, such as:

* Medical history
* Income
* Occupation
* Exercise habits
* Pre-existing conditions

The analysis shows relationships between variables and insurance charges, but it does not prove direct causation.

Some groups, such as customers with four or five children, have smaller sample sizes, so their averages should be interpreted carefully.

## Next Steps

Future analysis could include:

* Building a simple predictive model to estimate insurance charges
* Comparing different machine learning models
* Evaluating which variables are most useful for prediction
* Adding more customer information, such as medical history or lifestyle data
* Investigating whether smoking status interacts with age or BMI when predicting insurance charges

## How to Run the Project

To run this project:

1. Clone the repository:

```bash
git clone https://github.com/sahra02/Healthcare_Insurance.git
```

2. Open the project folder in VS Code.

3. Create and activate a virtual environment.

4. Install the required packages:

```bash
pip install -r requirements.txt
```

5. Open and run the notebooks in this order:

```text
jupyter_notebooks/01_ETL.ipynb
jupyter_notebooks/02_data_visualisation.ipynb
```

The ETL notebook creates the cleaned dataset, and the data visualisation notebook uses the cleaned dataset for analysis.

## Code Review and Quality Checks

The notebooks were reviewed and run from top to bottom to check that the code worked correctly and that the outputs matched the written explanations. Relative file paths were used so the project can be run from the repository structure.

The ETL notebook confirms that the raw dataset contains 1,338 rows and 7 columns, removes one duplicate row, and saves a cleaned dataset with 1,337 rows and 7 columns. The data visualisation notebook then loads the cleaned dataset and uses it for analysis.

Markdown explanations were included throughout the notebooks to explain the purpose of each step and the reasoning behind the cleaning and analysis decisions.

## Use of AI Tools

AI tools were used to support the development process, including project planning, debugging, markdown wording, explanation checking and notebook organisation.

AI support was used for tasks such as:

* Understanding Python and notebook errors
* Improving the structure of the notebooks
* Checking that written explanations matched the code outputs
* Reviewing the project for clarity and consistency

All code was reviewed, edited and tested before being included in the project. The final outputs and insights were checked manually to make sure they matched the dataset.

## Credits

* Dataset: Healthcare Insurance dataset from Kaggle
* Code Institute course materials were used to support learning around Python, data analysis, visualisation and project structure.