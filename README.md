# GradeBook Analyzer

A Python-based tool for analyzing and reporting student grades efficiently.

## Overview

The GradeBook Analyzer is a command-line application that helps teachers quickly analyze student performance after class tests. Instead of relying on spreadsheets or manual calculations, this tool automates statistical computations, grade assignments, and performance summaries.

## Features

- **Manual Data Entry**: Input student names and marks directly through the console
- **Statistical Analysis**: Automatically calculate average, median, minimum, and maximum scores
- **Grade Assignment**: Assign letter grades based on predefined criteria
- **Pass/Fail Filtering**: Separate students into pass and fail categories
- **Formatted Results**: Display results in a clean, tabular format
- **Interactive Menu**: Re-run analysis or exit through a user-friendly loop interface

## Requirements

- Python 3.x
- No external libraries required (uses only standard Python libraries)

## Installation

1. Clone or download this repository
2. Navigate to the project folder:
   ```bash
   cd gradebook_analyzer
   ```
3. Ensure you have Python 3.x installed:
   ```bash
   python --version
   ```

## Usage

Run the program using:
```bash
python gradebook.py
```

### Input Format

1. Enter the number of students in the class
2. For each student, provide:
   - Student name
   - Marks (numerical score)

### Grading Scale

- **A**: 90 and above
- **B**: 80-89
- **C**: 70-79
- **D**: 60-69
- **F**: Below 60

### Pass/Fail Criteria

- **Pass**: Marks ≥ 40
- **Fail**: Marks < 40

## Project Structure

```
gradebook_analyzer/
│
├── gradebook.py          # Main script file
└── README.md            # This file
```

## Features Breakdown

### Task 1: Project Setup
- Welcome message and menu display
- Proper script header with metadata

### Task 2: Data Entry
- Manual input collection
- Data storage in dictionary format

### Task 3: Statistical Analysis
- `calculate_average()` - Computes mean score
- `calculate_median()` - Calculates median value
- `find_max_score()` - Identifies highest score
- `find_min_score()` - Identifies lowest score

### Task 4: Grade Assignment
- Automated grade assignment based on score ranges
- Grade distribution count

### Task 5: Pass/Fail Filter
- List comprehension-based filtering
- Separate display of passed and failed students

### Task 6: Results Display
- Formatted table output
- Interactive loop for multiple analyses

## Example Output

```
===========================================
       GRADEBOOK ANALYZER
===========================================

Name                Marks    Grade
-----------------------------------------
Aradhya Mathur      78       C
Aayan Srivastwa     92       A
Prabhat Bhatia      56       F
Muskaan Jangra      85       B
Ishant Singh        91       A

Statistics:
-----------------------------------------
Average:        80.4
Median:         85.0
Highest Score:  92 (Aayan Srivastwa)
Lowest Score:   56 (Prabhat Bhatia)

Grade Distribution:
-----------------------------------------
A: 2 students
B: 1 student
C: 1 student
D: 0 students
F: 1 student

Pass/Fail Summary:
-----------------------------------------
Passed (≥40):   5 students
Failed (<40):   0 students
```

## Code Quality

- Modular functions for reusability
- Comprehensive comments
- Clean and readable code structure
- Proper variable naming conventions

## Testing

Test the program with at least 5 students to ensure all features work correctly:
- Various score ranges (high, medium, low)
- Edge cases (exactly 40, 60, 70, 80, 90)
- Students with failing marks

## Troubleshooting

**Issue**: Program crashes on input  
**Solution**: Ensure you're entering numerical values for marks

**Issue**: Incorrect median calculation  
**Solution**: Verify the sorting logic in the median function

**Issue**: Grade distribution doesn't match  
**Solution**: Check the if-elif-else conditions in grade assignment
This project is created for educational purposes as part of a programming course assignment.

---

**Happy Coding! Stay Curious!**
