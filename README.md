# Frozen Days Analysis Program

## Overview

This program analyzes historical data of ice cover days on Lake Mendota, Wisconsin, from 1855 to 2021. It performs linear regression to model the relationship between years and the number of frozen days, makes predictions about future ice cover, and visualizes the data trends.

## Files

1. **Data Files**:
   - `hw5.csv` - Cleaned dataset containing years and corresponding frozen days (1855-2021)
   - `original_data.csv` - Original dataset with additional details about freeze/thaw dates
   - `toy.csv` - Small test dataset for verification

2. **Program Files**:
   - `hw5.py` - Main Python script that performs the analysis
   - `plot.jpg` - Output graph showing the trend of frozen days over time
   - `toy_output.txt` - Sample output from running the program with the toy dataset

## Requirements

- Python 3.x
- Required libraries:
  - numpy
  - pandas
  - matplotlib

Install requirements with:
```
pip install numpy pandas matplotlib
```

## Usage

Run the program with:
```
python hw5.py hw5.csv
```

## Program Output

The program produces:

1. A plot (`plot.jpg`) showing the number of frozen days per year
2. Console output with:
   - Intermediate matrices (Q3a-Q3f)
   - Prediction for 2022 (Q4)
   - Trend analysis (Q5a-Q5b)
   - Year when Lake Mendota might stop freezing (Q6a-Q6b)

## Key Features

1. **Data Visualization**:
   - Generates a line plot showing the downward trend in frozen days

2. **Linear Regression**:
   - Computes regression coefficients using matrix operations
   - Models the relationship: `days = B0 + B1*year`

3. **Predictions**:
   - Predicts frozen days for future years (e.g., 2022)
   - Estimates the year when freezing might stop (x*)

## Sample Output

When run with the toy dataset:
```
Q3a:
[[   1 1800]
 [   1 1801]
 [   1 1802]]
Q3b:
[120 155  99]
...
Q4: -2195.833334037743
Q5a: <
Q6a: 1812.873015872499
```

## Interpretation

- **Q5a**: The '<' symbol indicates a negative trend (decreasing frozen days over time)
- **Q6a**: The predicted year when Lake Mendota might stop freezing based on current trends

## Notes

- The program uses ordinary least squares (OLS) for linear regression
- The analysis suggests a clear downward trend in the number of frozen days
- Results should be interpreted with consideration of climate change impacts

## Visual Output

![plot](https://github.com/user-attachments/assets/29f9a975-f9e6-420a-a00d-d4ca5dd2cf95)
