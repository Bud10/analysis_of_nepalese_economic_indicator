Analysis of Macro-Economic Indicators (2000-2021)

This repository contains an analysis of macro-economic indicators from the years 2000 to 2021. 
The analysis explores various economic factors and their trends over time, using different datasets. 
The project includes a Jupyter notebook for visualizing and analyzing the data and a couple of CSV files containing summarized economic data.

📂 File Structure

    macro-economic-analysis/
    │
    ├── Analysis_of_macro_economic_indicators(2000-2021).ipynb    # Jupyter notebook for macro-economic analysis
    ├── summary-of-macro-economic-indicators.csv                   # Summary dataset of macro-economic indicators (2000-2018)
    ├── summary-of-macro-economic-indicators_2012-2021table06.csv   # Dataset for macro-economic indicators (2012-2021)
    └── README.md                                                  # Project description

Datasets:

    summary-of-macro-economic-indicators.csv
    This dataset contains summarized macro-economic indicators for the entire period of 2000-2021. It includes various economic variables like GDP, inflation rates, unemployment rates, and more.

    summary-of-macro-economic-indicators_2012-2021table06.csv
    This dataset contains a more detailed summary of macro-economic indicators from 2012 to 2021, which can be used for more specific trend analysis during this period.

📊 Project Overview

The goal of this project is to analyze and visualize key macro-economic indicators over the past two decades (2000-2021). The analysis includes:

    GDP growth rates
    Inflation rates
    Unemployment rates
    Other relevant economic indicators

This analysis can provide insights into how various macroeconomic factors have influenced each other over the years and can help to make future predictions or understand past economic trends.

🧑‍💻 Prerequisites

To run the analysis and explore the data, you will need to install the following Python libraries:

    pandas (for data manipulation)
    matplotlib (for plotting and visualizations)
    seaborn (for enhanced visualizations)
    numpy (for numerical operations)
    jupyter (to run Jupyter notebooks)

You can install the dependencies using pip:

pip install pandas matplotlib seaborn numpy jupyter

🚀 How to Use
1. Open the Jupyter Notebook

    The analysis is done within the Jupyter notebook, Analysis_of_macro_economic_indicators(2000-2021).ipynb.
    To open the notebook, you can either:
        Open it directly on GitHub and view the code/visuals there.
        Clone the repository to your local machine and run it using Jupyter Notebook.

2. Load the Datasets

    The required datasets are provided in CSV format:
        summary-of-macro-economic-indicators.csv
        summary-of-macro-economic-indicators_2012-2021table06.csv
    In the notebook, you'll find code to load the datasets into pandas DataFrames for further analysis.

import pandas as pd

# Load the datasets
df_2000_2018 = pd.read_csv('summary-of-macro-economic-indicators.csv')
df_2012_2021 = pd.read_csv('summary-of-macro-economic-indicators_2012-2021table06.csv')

3. Run the Analysis

    The notebook performs various analyses, including:
        Cleaning and preprocessing the data
        Exploring trends of macro-economic indicators over time
        Generating visualizations to understand the relationships between the economic variables

    You can run each cell in the Jupyter notebook to see the data analysis and visualization in real-time.

4. Visualize the Data

    The notebook generates various plots using matplotlib and seaborn to visualize trends and patterns in the data. Examples of visualizations include:
        Line charts showing the change in GDP over time
        Bar graphs comparing inflation rates for different years
        Correlation heatmaps between different economic indicators

Example of a simple plot in the notebook:

import matplotlib.pyplot as plt

# Example: Plot GDP over time
df_2000_2021['Year'] = pd.to_datetime(df_2000_2021['Year'], format='%Y')
plt.plot(df_2000_2021['Year'], df_2000_2021['GDP'])
plt.xlabel('Year')
plt.ylabel('GDP (in billion USD)')
plt.title('GDP Over Time (2000-2021)')
plt.show()

📈 Results and Insights

The notebook will provide you with various insights such as:

    Trends of macro-economic indicators (like GDP, inflation, etc.)
    Economic growth and downturns during specific periods (e.g., the 2008 financial crisis)
    Relationships between different economic factors, such as GDP growth and inflation

Example Insights:

    GDP Growth: The GDP of many countries has shown steady growth, with significant dips during economic recessions.
    Inflation: Inflation rates fluctuated significantly between 2000 and 2021, with notable peaks during times of global financial instability.

💡 How to Contribute

Feel free to fork the repository and contribute by:

    Adding new analyses or insights
    Improving the visualizations
    Adding additional datasets for macro-economic indicators
    Enhancing the code with more efficient methods or advanced techniques

To contribute:

    Fork the repository.
    Create a new branch for your feature or bugfix.
    Submit a pull request with a detailed description of your changes.

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.
