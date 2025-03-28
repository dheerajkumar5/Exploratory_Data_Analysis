# Exploratory_Data_Analysis
**EDA_Using_Pandas**

_**Overview**_

This repository contains exploratory data analysis (EDA) performed on multiple datasets. The following analyses were conducted:

_**Datasets Used**_

**Titanic Dataset**: Focused on univariate preprocessing and bivariate analysis to study survival trends.
Visualized relationships between passenger demographics, ticket class, and survival rates.

**US Flights Dataset**: Demonstrated clustering techniques and time-based analyses using cluster maps and line plots.
Highlighted seasonal patterns and trends in flight data.

**Iris Dataset**: Used for multivariate analysis with pair plots to explore relationships between petal and sepal features across species.

_**Data Preprocessing**_

Key steps taken before analysis:

Read dataset into a pandas DataFrame for processing and analysis.

Initial Exploration: Used .head(), .sample(), .shape, .columns, .info, and .describe() to understand the structure, dimensions, and summary statistics of the data.

Missing Values: Checked for missing values using .isnull().sum() and handled appropriately during analysis.

Duplicate Data: Identified and removed duplicate rows using .duplicated().

_**Univariate Analysis
Categorical Data
**_
Count Plot: Used sns.countplot() to visualize the frequency of categorical variables.

Value Counts: Explored the distribution of categorical data using df['column_name'].value_counts().

Pie Chart: Created pie charts using df['column_name'].value_counts() to represent categorical data as proportions.

_**Numerical Data**__

Histograms: Visualized the distribution of numerical columns using sns.histplot().

Distribution Plot: Used sns.distplot() with:

Only histogram (hist=True, kde=False) for raw distribution.

Only kernel density estimate (KDE) (kde=True, hist=False) for smoothed density visualization.

Box Plot: Displayed numerical data distributions and detected outliers using sns.boxplot().

_**Bivariate Analysis**__

_**Numeric-Numeric Relationships**_

Scatter Plot: Compared numerical variables using sns.scatterplot(). Enhanced visualization by adding hue, size, and palette to encode additional dimensions.

_**Categorical-Numerical Relationships**__

Distribution Plot: Used sns.distplot() with hue and palette to separate distributions based on a categorical variable.

Bar Plot: Visualized averages of numerical data by categories with sns.barplot(). Incorporated hue and palette for deeper insights.

Box Plot: Analyzed the spread of numerical data by categories using sns.boxplot() with options for hue differentiation.

_**Categorical-Categorical Relationships**_

Crosstab and Heatmap: Created distributions of categorical data using pd.crosstab() and visualized them as heatmaps with sns.heatmap().

Cluster Map: Applied hierarchical clustering to the crosstab data with sns.clustermap() to group similar categories.

Groupby and Bar Plot: Aggregated categorical data using pd.groupby() and represented results via bar plots.

_**Time-Based Analysis**__

Line Plot: Visualized changes in numerical variables over time using sns.lineplot(). Useful for detecting trends and seasonality.

_**Multivariate Analysis**__

Pair Plot: Used sns.pairplot() to explore relationships among all numerical features. Color-coded data points using hue for differentiation by categories (e.g., survival status in Titanic, species in Iris).

Heatmap and Cluster Map: Created heatmaps and cluster maps using aggregated or grouped data (pd.pivot_table(), pd.crosstab()) to identify patterns and correlations across multiple variables.

