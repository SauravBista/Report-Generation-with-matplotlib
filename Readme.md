Programming Languages Post Analysis

This project involves analyzing programming languages' popularity over time based on StackExchange posts. The dataset provides monthly counts of posts for various programming languages, which allows for trends and comparisons between languages.
Getting Started
Prerequisites

    Python 3.x
    Pandas
    Matplotlib

You can install the required packages using pip:

bash

pip install pandas matplotlib

Data

The dataset used in this project is a CSV file named query.csv. It contains three columns:

    DATE: The date of the post (in YYYY-MM-DD format).
    TAG: The programming language tag.
    POSTS: The number of posts for the corresponding tag in the given month.

You can obtain this dataset by running an SQL query on StackExchange as described in the original file.
File Structure

    Programming_Languages_(start).ipynb: Jupyter Notebook containing the analysis and visualization code.
    query.csv: The dataset file.

Analysis
Data Loading

The dataset is loaded into a Pandas DataFrame from the query.csv file. The data is examined by displaying the first and last 5 rows, and the dimensions of the DataFrame are printed.
Data Exploration

    The total number of posts per programming language is calculated.
    The number of months of data available per language is counted, and the language with the fewest months of data is identified.

Data Cleaning

    The 'DATE' column is converted to a datetime format, and a new column for year-month periods is created.
    The DataFrame is reshaped to have dates as the index and programming languages as columns, with post counts as values.

Data Visualization

    A rolling mean is calculated over a 5-month window to smooth out the time series data.
    A line plot is generated to visualize trends in the number of posts for each programming language over time.

Usage

    Place the query.csv file in the same directory as the Jupyter Notebook.
    Open the Programming_Languages_(start).ipynb file in Jupyter Notebook.
    Run the cells to perform the data analysis and visualization.

Example

The notebook demonstrates how to:

    Load and explore the dataset.
    Clean and reshape the data.
    Visualize trends in programming language popularity over time.

License

This project is licensed under the MIT License. See the LICENSE file for details.