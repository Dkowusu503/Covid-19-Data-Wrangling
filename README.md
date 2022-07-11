# Covid-19-Data-Wrangling
Covid-19 Data wrangling with python pandas in jupyter notebook.

Data cleaning process is as follows:
1. Changing the datatype of the date column from object to datetime.

2. Deleting all rows containing empty values in the continent column.
* This is because those rows were found to contain continent names in country column.
* Deleting those rows then ensures country column only contain country names and not sum of values for continents.

3. Empty values in total cases, new cases, total deaths, new deaths, total vaccinations and new vaccinations columns were replaced with zero.
* Most of the empty values were found to be at the begining of the pandemic for each country when data was not present or collected.
* Replacing NaN with zero makes it easy for analysis. For instance columns containing NaN values cannot be changed from float datatype to integer datatype.

4. Datatype in total cases, new cases, total deaths, new deaths, total vaccinations and new vaccinations column were changed from float to integer datatype.
* Reason for this is because counts of humans are whole and not fractional.

5. Finally, whitespace in all the columns are trimmed for easy data visualizations and analysis.

