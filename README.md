# Analysis of Domestic Violence Cases

## Introduction
This notebook analyzes a dataset containing information about domestic violence cases. The objective is to uncover patterns related to geographical location, gender, age group, and time, providing key insights and conclusions.

## Data Loading and Cleaning

### Data Source
The dataset was initially loaded from a CSV file, encompassing several attributes essential for the analysis.

### Data Inspection
- **Mixed Data Types**: Observed in the 'CODIGO DANE' column.
- **Missing Values**: Found in 'ARMAS MEDIOS', 'GENERO', and 'GRUPO ETARIO'.
- **Duplicate Rows**: Present within the dataset.

### Cleaning Steps
The following steps were taken to clean the data:

1. Dropped duplicate rows to ensure unique records.
2. Replaced '-' and 'NO REPORTA' with NaN in 'GENERO', 'ARMAS MEDIOS', and 'GRUPO ETARIO'.
3. Removed rows containing NaN values in 'GENERO', 'ARMAS MEDIOS', and 'GRUPO ETARIO'.
4. Converted 'GENERO', 'ARMAS MEDIOS', and 'GRUPO ETARIO' values to uppercase for standardization.
5. Transformed the 'FECHA HECHO' column into datetime objects, accommodating both standard date formats and Excel serial dates.
6. Dropped the original 'FECHA HECHO' column while retaining clean date data.
7. Extracted 'Year', 'Month', and 'Day' into separate columns for detailed temporal analysis.

## Exploratory Data Analysis

The cleaned dataset facilitated the following exploratory data analyses:

- **Cases by Department**: Displayed through a bar plot, illustrating the total number of cases per department.
- **Cases by Gender**: Demonstrated using a bar plot to reveal the gender distribution of cases.
- **Cases by Age Group**: Visualized with a pie chart to show the proportion of cases across different age groups (Adults, Adolescents, Minors).
- **Cases Over Time**: A line plot showcasing the temporal trend in domestic violence occurrences.

## Conclusion

The analysis unveiled distinct patterns in domestic violence cases based on location, gender, age, and timeframes. Potential areas for further exploration include:

- Detailed examination of specific departments or municipalities.
- Investigation into types of weapons/means involved.
- Exploration of correlations with socioeconomic factors.

## Future Work
This project may benefit from extended datasets and incorporate additional variables for more comprehensive analysis and decision-making support.

---

Feel free to contribute or fork this repository to expand upon the current analysis or introduce new datasets and techniques. For questions or collaboration, please reach out!
