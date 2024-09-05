# Mod-2-jupyter-note
# Employee Data Processing

This project contains a Jupyter Notebook for processing employee salary data, exporting it, and analyzing it using both Python and R.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Jupyter Notebook installed
- Python 3.7+ installed
- R installed
- Required Python libraries: pandas
- Required R libraries: readr, dplyr

## Setup

1. Clone this repository or download the files to your local machine.
2. Ensure you have a file named `salary_data.csv` in the same directory as the Jupyter Notebook. This file should contain columns for Name, Department, Salary, and Years of Experience.

## Using the Jupyter Notebook

1. Open the `employee_data_processing.ipynb` file in Jupyter Notebook.
2. Run each cell in order from top to bottom.

### Python Code

The Python section of the notebook does the following:

1. Imports the salary data from `salary_data.csv`.
2. Defines a function `get_employee_details(name)` to retrieve details for a specific employee.
3. Processes the data into a dictionary for easy access.
4. Implements error handling with `safe_get_employee_details(name)`.
5. Exports the employee details to a CSV file and zips it into an "Employee Profile" folder.

To use the Python functions interactively:

```python
# Get details for an employee
details = get_employee_details("John Doe")
print(details)

# Safely get details (with error handling)
safe_details = safe_get_employee_details("Jane Smith")
print(safe_details)

### R code of this project

The R section of the notebook:

Unzips the exported CSV file.
Reads the CSV data.
Displays the data and provides summary statistics.
The R code runs automatically when you execute the last cell of the notebook.

Customizing the Code
To change the input file name, modify the pd.read_csv('salary_data.csv') line in the Python code.
To change the output folder name, modify the output_folder = 'Employee Profile' line.
To add more analysis in R, add your R code to the last cell of the notebook.
Troubleshooting
If you encounter a "File not found" error, ensure that salary_data.csv is in the same directory as the notebook.
If R code doesn't run, make sure you have the R kernel installed in Jupyter and the required R libraries (readr, dplyr) installed.
Additional Notes
The exported CSV and zip files will be created in an "Employee Profile" folder in the same directory as the notebook.
Make sure you have write permissions in the directory where you're running the notebook.
For any additional help or questions, please open an issue in the project repository.


This README file provides comprehensive instructions on:

1. Prerequisites and setup
2. How to use the Jupyter Notebook
3. Explanation of the Python code and how to use it interactively
4. Explanation of the R code
5. How to customize the code
6. Troubleshooting common issues
7. Additional notes on file locations and permissions
