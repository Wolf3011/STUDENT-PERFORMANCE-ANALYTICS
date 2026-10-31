# Student Performance Analytics System

## 1. Project Title
**Student Performance Analytics System**

- **Student Name:** Ayan
- **Course:** Python with AI – EWB Courses
- **College / Roll No.:** [Add here]
- **Submission Date:** [Add here]

## 2. Objective
Teachers often have to calculate marks, grades and pass/fail results by hand, which is slow and error-prone. This project automates that work with Python. It reads student data, calculates totals, averages, grades and results, and produces clear insights such as subject-wise performance, department-wise performance and top performers.

## 3. Technologies Used
- **Python 3**
- **NumPy**: numerical calculations (totals, averages, min/max, conditions)
- **Pandas**: DataFrame creation, grouping, sorting and analysis
- **Google Colab**: development environment

No other libraries were used.

## 4. Dataset Description
The dataset was created manually inside the code (no CSV file) and contains **24 Indian student records**.

| Column | Description |
|---|---|
| Student ID | Unique ID (S101–S124) |
| Name | Student name |
| Department | CSE, ECE, EEE or ME |
| Maths, Physics, Chemistry, English, Computer Science | Marks out of 100 |
| Attendance | Attendance percentage |

Columns added during processing: **Total, Average, Grade, Result, Rank**.

## 5. Implementation
1. **Import libraries:** NumPy and Pandas.
2. **Create dataset:** student records stored as a list of lists.
3. **Load data:** converted into a Pandas DataFrame, then checked with `shape`, `info()` and missing-value count.
4. **Define functions:** reusable functions for total, average, grade and pass/fail.
5. **Process data:** marks converted to a NumPy array; totals and averages calculated with `np.sum` and `np.mean`; a loop assigns each student's grade and result.
6. **Analysis:** overall statistics, grade distribution and failed students list.
7. **Subject-wise analysis:** a loop calculates highest, lowest, average, passed and failed counts per subject.
8. **Top performers:** top 5 students by average and the topper in each subject.
9. **Department-wise analysis:** `groupby` used to compare departments.
10. **Final report:** a formatted summary of all key results.

### Grading Rule
| Average Marks | Grade |
|---|---|
| 90 and above | A+ |
| 80 – 89 | A |
| 70 – 79 | B |
| 60 – 69 | C |
| 50 – 59 | D |
| 40 – 49 | E |
| Any subject below 40 | F |

### Pass/Fail Condition
A student **passes** only if they score **at least 40 marks in every subject**; otherwise the result is **Fail**.

## 6. Key Features
- `calculate_total()`: total marks per student (NumPy)
- `calculate_average()`: average marks per student (NumPy)
- `assign_grade()`: grade based on the grading rule
- `check_result()`: pass/fail decision
- Class statistics: pass percentage, class average, highest and lowest performers
- Subject-wise performance analysis
- Department-wise performance comparison
- Top 5 students and subject toppers
- Final formatted report

## 7. Output / Screenshots
Add screenshots of your outputs to a `screenshots/` folder and link them here:

![DataFrame Output](screenshots/dataframe.png)
![Overall Analysis](screenshots/overall_analysis.png)
![Subject-wise Analysis](screenshots/subject_analysis.png)
![Top Performers](screenshots/top_performers.png)
![Final Report](screenshots/final_report.png)

## 8. Final Outcome
The project successfully:
- Loaded and organized 24 student records in a Pandas DataFrame
- Calculated total marks, average marks, grades and pass/fail status for every student
- Identified the highest and lowest performers and the overall class average
- Found the best and weakest subjects
- Compared the four departments
- Produced a clear final report that is understandable without reading the code

## 9. Challenges & Learning
- **Challenge:** Defining a fair grading rule when a student has a good average but fails one subject.
  **Solution:** Any subject below 40 results in grade F, so grade and result stay consistent.
- **Challenge:** Choosing where to use NumPy and where to use Pandas.
  **Solution:** NumPy for numerical calculations on arrays, Pandas for organizing, grouping and displaying data.
- **Learning:** Writing reusable functions, using loops where iteration is needed, handling DataFrames, and presenting results clearly.

## 10. GitHub Repository
[Paste your final repository link here]

## How to Run
1. Open `student_performance_analytics.ipynb` in Google Colab.
2. Click **Runtime → Run all**.
3. The analysis and final report appear in the output of each cell.
