# Matplotlib Challenge

This project analyzes how different drug treatments impact mice with cancerous tumors. The dataset includes data from various drug regimens studied over time, and the analysis involves using data visualization and statistical methods to investigate changes in tumor volume and relationships between variables like mouse weight and tumor volume.
The analysis includes data preparation, summary statistics, visualization (bar charts, pie charts, box plots), and linear regression analysis (Module 5 Challenge).

# Analysis Steps

1. Data Preparation
   - Merged Datasets: I merged the `mouse_metadata` and `study_results` datasets on the `Mouse ID` column to create a comprehensive DataFrame.
   - Cleaned Data: I identified and removed duplicate entries (if a mouse had the same time point recorded multiple times), ensuring only unique observations were used for analysis.

2. Summary Statistics
   Statistical Summary: I generated summary statistics for each drug regimen, which included:
     - Mean Tumor Volume
     - Median Tumor Volume
     - Variance of Tumor Volume
     - Standard Deviation of Tumor Volume
     - Standard Error of the Mean (SEM) of Tumor Volume

3. Bar Charts and Pie Charts
    - Bar Charts: I created two bar charts to show the total number of data points for each drug regimen.
       - One chart was generated using Pandas DataFrame `.plot()`, and the other using Matplotlib's pyplot functions.
    - Pie Charts: I created pie charts to show the gender distribution of the mice (Male vs. Female).
        - One pie chart was created using Pandas DataFrame `.plot()`, and another using Matplotlib's pyplot

4. Quartiles, Outliers, and Box Plot
    - Final Tumor Volume I calculated the final tumor volume for each mouse across four treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin.
    - Quartiles and IQR I calculated the interquartile range (IQR) and determined any potential outliers for these regimens.
    - Box Plot Using Matplotlib, I generated a box plot to show the distribution of final tumor volumes for these four regimens. Outliers were highlighted using a different color.

5. Line Plot and Scatter Plot
   - Line Plot I selected a mouse treated with Capomulin and generated a line plot showing tumor volume over time.
   - Scatter Plot I generated a scatter plot to visualize the relationship between mouse weight and average tumor volume for all mice treated with Capomulin.

6. Correlation and Regression Analysis
   - Correlation: I calculated the correlation coefficient between mouse weight and average tumor volume for the Capomulin regimen.
   - Linear Regression I performed a linear regression analysis and plotted the regression line on top of the scatter plot to highlight the relationship between mouse weight and tumor volume.

# Data Sources
- Mouse_metadata.csv: Contains details like mouse ID, drug regimen, sex, age, and weight.
- Study_results.csv: Includes tumor volume and metastatic site data across time points.

# How to Run
   1. Clone the repository:
       1. Open your terminal (Git Bash, Command Prompt, or any Git client).
       2. Use the cd command to navigate to the directory where you want to clone the repository.
       3. Run the following command to clone the repository: git clone link_provided
  2. Ensure Pandas, Matplotlib, SciPy, and NumPy is installed on your machine.
     - Install Pandas using pip if it's not already installed (pip install pandas).
     - Install Matplotlib using pip if it's not already installed (pip install matplotlib).
     - Install SciPy using pip if it's not already installed (pip install scipy).
     - Install NumPy using pip if it's not already installed (pip install numpy).
  3. Open the cloned file in the Visual Studio Code:
       1. Go to file > Open Folder and navigate to the folder where you cloned the repository.
       2. Select the folder to open in VS code.
  4. Run the Jupyter Notebook
     1. Open the notebook file (pymaceuticals_starter.ipynb) in VS code or Jupyter.
     2. Run the cells to perform the Analysis.

# Data Analysis Highlights
- Summary statistics: Statistical properties like mean, median, variance, and SEM of the tumor volumes across drug regimens.
- Outliers: Detected using interquartile range (IQR) method and visualized in box plots.
- Correlation: The link between mouse weight and tumor volume was examined using scatter plots and linear regression.

# Conclusion
The research contributes to a better understanding of the efficiency of various treatment regimens on tumor growth, as well as the potential correlations between animal features (such as weight) and tumor volume.
