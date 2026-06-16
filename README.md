# STUDY-OF-RELATION-BETWEEN-ROAD-ACCIDENTS-AND-BAD-WEATHER-CONDITION
 This project studies how bad weather affects road accidents using statistical analysis and Python. It examines rainfall, fog, and other conditions, calculates correlation, and builds a quadratic regression model to show how accident frequency changes. The results provide clear, data-driven insights for road safety planning.
# Study of Relation Between Road Accidents and Bad Weather Conditions

## Overview
This project is a Probability and Statistics case study that analyzes whether bad weather conditions increase the number of road accidents. The study focuses on the relationship between accident count and daily weather condition values collected from a sample dataset. Statistical methods such as correlation analysis and quadratic regression are used to understand the strength and pattern of this relationship.

## Problem Statement
Road safety is affected by multiple external factors, and weather is one of the most important among them. Rain, fog, poor visibility, and slippery roads can increase driving risk. The objective of this project is to check whether bad weather conditions are associated with a higher number of road accidents and to represent the relationship mathematically.

## Objectives
- Collect a sample dataset of road accidents and weather observations.
- Calculate the coefficient of correlation between accidents and weather conditions.
- Construct a quadratic regression curve suitable for the collected data.
- Interpret the statistical relationship between the two variables.

## Dataset
The sample data used in this study includes:
- Number of accidents
- Weather condition value for the day

### Sample Data

| Serial No. | No. of Accidents | Weather Value |
|-----------|------------------|---------------|
| 1 | 2 | 30 |
| 2 | 3 | 27 |
| 3 | 5 | 24 |
| 4 | 1 | 25 |
| 5 | 4 | 22 |
| 6 | 2 | 22 |
| 7 | 1 | 23 |
| 8 | 4 | 24 |
| 9 | 2 | 25 |
| 10 | 1 | 23 |

## Statistical Analysis

### Mean Values
- Mean of accidents \( \bar{x} = 2.5 \)
- Mean of weather values \( \bar{y} = 24.5 \)

### Correlation Coefficient
The Pearson correlation coefficient is calculated using the formula:

\[
r = \frac{\sum XY}{\sqrt{\sum X^2 \sum Y^2}}
\]

The computed correlation coefficient is:

**r = -0.248975**

This indicates a **weak negative correlation** between the number of accidents and the recorded weather values in the given sample. A negative value means that as the weather variable changes upward, accident counts tend to decrease slightly in this dataset. However, the relationship is weak, so the effect is not strong enough to claim a high linear association.

## Quadratic Regression Model
To model a possible curved relationship between weather conditions and accidents, a quadratic regression equation was fitted:

\[
Y = -0.5473x^2 + 2.9565x + 21.5421
\]

This quadratic model helps capture a non-linear trend in the data, which is useful because weather effects on accidents may not always follow a straight-line pattern.

## Technologies Used
- Python
- NumPy
- Matplotlib
- SciPy

## Python Tasks Performed
- Data storage using NumPy arrays
- Mean and correlation calculation
- Polynomial curve fitting using `np.polyfit()`
- Regression curve generation using `np.poly1d()`
- Data visualization using Matplotlib

## Sample Code
```python
import numpy as np
import matplotlib.pyplot as plt

accidents = np.array()[4][5][6][7][8]
weather = np.array()[9][10][11][12][13][14]

coefficients = np.polyfit(accidents, weather, 2)
curve = np.poly1d(coefficients)

print("Quadratic Regression Equation:")
print(curve)

plt.scatter(accidents, weather, label='Data Points')
plt.plot(accidents, curve(accidents), color='red', label='Quadratic Regression Curve')
plt.xlabel('Number of Accidents')
plt.ylabel('Weather Condition Value')
plt.legend()
plt.show()
```

## Result
The study found a weak negative correlation in the sample data, with a quadratic regression curve used to represent the relationship more effectively. This shows that weather conditions can influence accident patterns, but the strength and direction of the relationship depend on the collected data and the way the weather variable is measured.

## Conclusion
This project demonstrates the use of probability, statistics, and Python in analyzing a real-world problem. By combining correlation analysis and quadratic regression, the study provides a mathematical and visual understanding of how weather conditions may affect road accidents.

## Team
- O. Prudhvi Teja - 2203A51577
- G. Tharun - 2203A51567
- P. Meghanth Rao - 2203A51578
- P. Sunny - 2203A51511
- E. Sai Deekshith - 2203A51564
- A. Rohan - 2203A51537

## Guide
**Dr. G. Ravi Kiran**  
Department of Mathematics  
SR University, Ananthasagar, Hanamakonda
