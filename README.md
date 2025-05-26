# TASK-1-Data-Cleaning-and-Preprocessing
Objective:
To clean and preprocess the Medical Appointment No Shows dataset by identifying and handling:

1. Missing values
2. Duplicate records
3. Invalid data (e.g.negative ages)
4. Inconsistent formats in text and date columns
5. Poorly structured column names
6. The final goal is to prepare a clean dataset suitable for analysis and modeling.

Tools Used:

Google Colab

Steps Performed:
1. Dataset Loading
Imported the dataset using pandas.read_csv() and displayed the first few rows for structure understanding.
2. Exploratory Checks
Used .info() and .describe() to analyze data types, column-wise null counts, and identify anomalies.
3. Missing Values
Checked using .isnull().sum() — no missing values were found in this dataset.
4. Duplicate Removal
Used .duplicated().sum() and .drop_duplicates() to eliminate duplicate rows.
5. Invalid Data Handling
Removed records with negative ages (e.g., Age < 0).
6. Date Formatting
Converted ScheduledDay and AppointmentDay columns to datetime using pd.to_datetime().
7. Text Standardization
Made categorical text columns like Gender and No-show consistent using .str.upper().str.strip().
8. Column Renaming
Renamed all column headers to lowercase with underscores using string methods for clarity and ease of use.
9. Final Verification
Rechecked data using .isnull(), .duplicated() and dtypes to confirm cleanliness and consistency.

Output Files:
1. cleaned_medical_appointments.csv: Cleaned version of the dataset
2. task1_cleaning.ipynb: Notebook with all steps and code
3. Task_1_Detailed_Report.docx: Word document summary with step-by-step explanation

Learning Outcomes:
Practiced real-world data preprocessing using Python
Understood how to identify and fix common issues like nulls, duplicates and format inconsistencies
Learned to prepare datasets for deeper data analysis or machine learning

Submission:
GitHub Repository: https://github.com/Rithikkaa-17/TASK-1-Data-Cleaning-and-Preprocessing-
Submitted on: 26-05-2025
