---
layout: default
title: 06-Analysis Function (Your Final Boss)
nav_order: 8
parent: 03 - Scientific Programming
grand_parent: Assignment Instructions
---

# Lesson 6: Create Your own Site Analysis Function
**Estimated time to complete: 90-120 minutes**  
In this final exercise, you will leverage and synthesize what you've learned in the previous lessons to create a function (from scratch) that allows a user to run a quick statistical analysis of any station dataset in your /Data folder. 

## 1. Setup
1. Make sure your **Working Directory** is set to ```/ > MATLAB Drive > iSci3A12-SciProgramming```. This is where we will run our scripts and analyses. 
1. In MATLAB, open the file ```station_stats.m```. This function has been partially completed for you. Your tasks are described below:
   
## 2. Your tasks 
The function `station_stats.m` should calculate and present the user with basic statistics for their station of choice in `/Data`. The function should do the following:
1. Accept station name (as a string) as an input to select which file to load from the /Data folder (e.g. `Adelaide Airport`, `Bremen`, etc.).
	- *Note*: The function should accept station name only (and not `.csv`, as this should be appended when you load the file). 
	- *Hint*: Reuse code from previous scripts and functions
2. Load station data from the `/Data` folder 
3. Analyze the station data to produce a 7 x 2 numeric array (matrix) that contains the following values:

| Row | **Column 1 (Use decimal degrees Celsius for all temperatures)** | **Column 2**                              |
|-----|------------------------------------------------------------|-------------------------------------------|
| 1   | Mean annual temperature for the dataset *                  | Number of years used in the calculation   |
| 2   | Standard deviation of annual temperatures *               | Number of years used in the calculation   |
| 3   | Maximum annual temperature in the dataset *                 | Year or maximum annual temperature        |
| 4   | Minimum annual temperature in the dataset *                 | Year or minimum annual temperature        |
| 5   | Temperature of the coldest month                           | Year of coldest month                     |
| 6   | Temperature of warmest month                               | Year of warmest month                     |
| 7   | Number of missing months (-9999 / NaNs) in the dataset                    | Number of incomplete years in the dataset |

  - *Note*: "*" Denotes calculations where years with missing values should be excluded.
4. Print 7 lines to the Command Window (to be viewed by the user) that communicates the values in the first columns. e.g., 	
```
Mean annual temperature for the dataset: 16.45 Celsius
Standard deviation of annual temperatures: 1.23 Celsius
Maximum annual temperature: 27.10
Minimum annual ...
...
```

  - *Hint*: Build strings (taking advantage of the `num2str` function) and use the `disp` function (7 times) to display the message in the Command Window. 
5. The function should be appropriately commented so a user understands what it does, how it operates, how to use it, who made it, etc.

## 4. (Oh no, not another) Reflection
Don’t worry too much. This one is short and sweet. In 100 words or less, I would like to know what you thought of the workshop and the programming experience. *Was this a useful exercise? Do you see the benefits of taking a scripted approach to analysis? What was/wasn’t useful? Is there anything that you would have liked to have done differently?* Add your reflection to the ```reflection.md``` file in your assignment GitHub repository.

## 5. Ready to submit? 
Go to the [submission](a3-submission) page to prepare your materials for submission. 
