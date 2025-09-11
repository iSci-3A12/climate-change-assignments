---
layout: default
title: 04-Analyze a Station
nav_order: 6
parent: 03 - Scientific Programming
grand_parent: Assignment Instructions
---

# Lesson 4: Analyzing one station's data

**Estimated time to complete: 30-90 minutes**  
In this exercise, you will complete the code and comments for the script ```process_adelaide.m``` (which is found in your MATLAB Drive). When completed, this script will load data for the climate station ```ADELAIDE_AIRPORT```, and carry out the same analysis as you completed in a spreadsheet for the first part of your Climate Data Assignment. You will also load data for the climate station `DETROIT_METRO_AP` (Detroit Metro Airport) and create a scatterplot of annual temperature anomalies between the two sites. This should give you a good understanding of the power of scripted approaches, and you'll build on this script to create a final deliverable that can complete analysis for all sites at once. 
  
By the end of this lesson, you will have created the following required deliverable: 
- A script called ```process_adelaide.m```, which completes analyses successfully and produces ***three figures*** named":
  - `Adelaide Airport_timeseries.png`
  - `Adelaide Airport_barcode.png`
  - `Adelaide_vs_Detroit.png`

### Video
<iframe height="540" width="853" allowfullscreen frameborder=0 src="https://echo360.ca/media/853400bb-4fa9-4b53-bd15-4c100c08b462/public?autoplay=false&automute=false"></iframe>
[Direct link to video](https://echo360.ca/media/853400bb-4fa9-4b53-bd15-4c100c08b462/public).

## 1. Setup
1. Make sure your **Working Directory** is set to ```/ > MATLAB Drive > iSci3A12-SciProgramming```. This is where we will run our scripts and analyses. 
1. In MATLAB, open the file ```process_adelaide.m```. This script has been mostly completed for you. Your tasks are described below: 

## 2. Your tasks
1. Execute the script line-by-line (hint: use the ```F9``` key, read comments, and view the resulting variables to understand what each line of code is doing.
1. Look for comments that contain ```<**TO DO**>``` and instructions. Complete the code on these lines. 
1. Ensure that the script runs without issues (i.e. by clicking the ```Run``` button) and produces ***three figures*** in the \Figs directory.
1. Add comments to the top comment section and on other lines where you've added code. 

## 3. Hints
1. Already included in the function is some code that will remove -9999s from your data. If your timeseries graph shows a steep drop in values (e.g. equal to -9999), you've likely used the wrong variable to calculate anomalies. 

## 4. Deliverables
- Ensure that all changes to your script ```process_adelaide``` are saved.
- **NOTE** that you are submitting the script and not the output (Jay is going to run the script on his computer to evaluate that it creates the proper outputs).

## 5. Head to the next exercise
Now that you've processed one site, the challenge is to generalize this code into a function that can analyze all sites in your data folder at once! Head to the [final lesson](a3-lesson5). One more to go! 
