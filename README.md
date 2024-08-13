# Module 5 Challenge - Data Visualization
Using Pandas, MatPlotLib, and ScyPy PyStats to analyze pharmaceutical data about clinical mouse trials.

---

## Background 
You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.
---
## Requirements

### Prepare the Data
  - [x] The datasets are merged into a single DataFrame.
  - [x] The number of mice are shown from the merged DataFrame.
  - [x] Each duplicate mice is found based on the Mouse ID and Timepoint.
  - [x] A clean DataFrame is created with the dropped duplicate mice.
  - [x] The num=ber of mice are shown from the clean DataFrame.

### Generate Summary Statistics
  - [x] The mean of the tumor volume for each regimen is calculated using groupby.
  - [x] The median of the tumor volume for each regimen is calculated using groupby.
  - [x] The variance of the tumor volume for each regimen is calculated using groupby.
  - [x] The standard deviation of the tumor volume for each regimen is calculated using groupby.
  - [x] The SEM of the tumor volume for each regimen is calculated using groupby.
  - [x] A new DataFrame is created using the summary statistics.

### Create Bar Charts and Pie Charts**
  - [x] A bar plot showing the total number of timepoints for all mice tested for each drug regimen using Pandas is generated.
  - [x] A bar plot showing the total number of timepoints for all mice tested for each drug regimen using pyplot is generated.
  - [x] A pie chart showing the distribution of unique female versus male mice using Pandas is generated.
  - [x] A pie chart showing the distribution of unique female versus male mice using pyplot is generated.

### Calculate Quartiles, Find Outliers, and Create a Box Plot**
  - [x] A DataFrame that has the last timepoint for each mouse ID is created using groupby.
  - [x] The index of the DataFrame is reset.
  - [x] Retrieve the maximum timepoint for each mouse.
  - [x] The four treatment groups, Capomulin, Ramicane, Infubinol, and Ceftamin, are put in a list.
  - [x] An empty list is created to fill with tumor volume data.
  - [x] A for loop is used to display the interquartile range (IQR) and the outliers for each treatment group.
  - [x] A box plot is generated that shows the distribution of the final tumor volume for all the mice in each treatment group.

### Create a Line Plot and a Scatter Plot**
  - [x] A line plot is generated that shows the tumor volume vs. time point for one mouse treated with Capomulin.
  - [x] A scatter plot is generated that shows average tumor volume vs. mouse weight for the Capomulin regimen.

### Calculate Correlation and Regression**
  - [x] The correlation coefficient and linear regression model are calculated for mouse weight and average tumor volume for the Capomulin regimen.



# References
---
- This was used for the flierprops I noticed in the GitHub below. I used the syntax to change the customization of the outlier fliers in the boxplot piece 
  - [Flierprops MatPlotLib](https://matplotlib.org/3.1.1/gallery/statistics/boxplot.html)
- I used this GitHub Repo to compare results as well as processes to analyze the data. I tried to find alternate/better practices for some of the calculations. I mainly used this as a starting point or to go back and help debug my own code when it woulnd't work. | 
  - [Benanza Github Repo](https://github.com/benanza/Pymaceuticals)
- Richard Wallace - I used code derived from Richard's work to identify the duplicate Mouse ID and Timepoint values and remove them from the DataFrame. I got stuck on this for a while and could not for the life of me find documentation that gave me what I needed. Need to work on that. 
  - [Richard Wallace's GitHub Repo](https://github.com/Cenbull70/Module-5-Challenge)