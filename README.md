# pandas-challenge
This project involves analyzing data related to schools and students using Python and the Pandas library. We will perform various calculations and generate summary statistics to gain insights into the educational system of PyCity.

Getting Started
To begin, you'll need to set up your Python environment and load the necessary data files. Follow the steps below to get started:

Dependencies and Setup: Make sure you have the required libraries installed. You can install them using pip if you don't have them already:
python
Copy code
import pandas as pd
Data Files: You need two data files: one containing information about schools and another containing data about students. Please provide the file paths to these data files in the code.
python
Copy code
school_data_to_load = "Resources/schools_complete.csv"
student_data_to_load = "Resources/students_complete.csv"
Read Data: Load the school and student data into Pandas DataFrames.
python
Copy code
school_data = pd.read_csv(school_data_to_load)
student_data = pd.read_csv(student_data_to_load)
Combine Data: Merge the school and student data into a single dataset for analysis.
python
Copy code
school_data_complete = pd.merge(student_data, school_data, how="left", on=["school_name", "school_name"])
District Summary
In this project, we will calculate various summary statistics for the district, including:

Total number of schools
Total number of students
Total budget
Average math score
Average reading score
Percentage of students with a passing math score (70 or greater)
Percentage of students with a passing reading score (70 or greater)
Percentage of students who passed both math and reading (% Overall Passing)
We will create a DataFrame to store these results and, if desired, format the displayed data for clarity.

