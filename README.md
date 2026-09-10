# OLIVER_PA3
## Intended Learning Outcomes
1. load a CSV dataset into a Pandas DataFrame;
2. select rows and columns using positional and label-based indexing;
3. filter records using conditions on a DataFrame column; and
4. extract a well-defined subset of data without changing the source data.
## A. POSITIONAL AND LABEL-BASED SLICING
We are required to output from the file `cars.csv` and only show a specific row and column.

* `import pandas as pd` - Gives us access to the Pandas Library.
* `pd.read_csv('cars.csv')` - Lets us read and access a `.csv` file uploaded into our Jupyter Notebook.
* `cars.iloc[6:11]` - Selects the rows starting from row 6 until row 10.
* `cars_6_to_10.loc[:, ['Model', 'mpg','cyl','hp', ]]` - Only selects and outputs the mentioned columns.
## B. MODEL LOOK UP
We are required to display only a single specific row and utilize boolean indexing to display a specific column.

* `cars.loc[cars['Model']=='Toyota Corolla']` - Searches for the specific input assigned in that column and displays the whole row.
* `cars.loc[cars['Model']=='Pontiac Firebird',['Model','mpg','cyl','wt']]` - Searches for the specific input assigned in that column and also only displays the specified columns for its rows.
## C. MULTI-MODEL SUBSETTING
In this problem we need to only call for the specified rows and only display some specific columns; also displaying its shape.

* `cars.loc[cars['Model'].isin(['Datsun 710','Lotus Europa','Ferrari Dino'])]` - Selects the rows with specific values.
* `,['Model','mpg','cyl','hp','gear']` - Retains the only mentioned columns.
* `selected_cars.shape` - Displays the number of rows and columns.

To view the main python program for Programming Assignment 2, click this OLIVER_PA3.ipynb and download. Open in Jupyter Notebook, then run all cells.
