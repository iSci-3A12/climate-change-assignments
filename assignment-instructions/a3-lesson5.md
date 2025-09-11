---
layout: default
title: 05-Analyze all Stations
nav_order: 7
parent: 03 - Scientific Programming
grand_parent: Assignment Instructions
---

# Lesson 5: Analyzing Any or All Stations

**Estimated time to complete: 30-90 minutes**  
In this final exercise, you'll take what you learned in the [previous lesson](a3-lesson4) to build a function (```plot_station_data.m```, which has been started for you) that can process any or all station data in your ```/Data``` folder. In completing this function, you will demonstrate the true value of using a scripted approach to create automated, repeatable, and extensible analyses.

By the end of this lesson, you will have created the following required deliverable: 
- A function called ```plot_station_data.m```. 

### Video
<iframe height="540" width="853" allowfullscreen frameborder=0 src="https://echo360.ca/media/1a9461b9-6d33-48ca-bc8a-f0122149f796/public?autoplay=false&automute=false"></iframe>
[Direct link to video](https://echo360.ca/media/1a9461b9-6d33-48ca-bc8a-f0122149f796/public).


## 1. Setup
1. Make sure your **Working Directory** is set to ```/ > MATLAB Drive > iSci3A12-SciProgramming```. This is where we will run our scripts and analyses. 
1. In MATLAB, open the file ```plot_station_data.m```. This function has been partially completed for you. Your tasks are described below: 

## 2. Your tasks

<!--
<table style="background-color: #ffff99;">
<tbody>
<tr>
<td>
<p><b>Update 2021-03-05</b>: If you downloaded your data pack before 06-March, there is a small bug in the <b>plot_station_data</b> code that needs to be corrected.</p>
<p>To correct this, near the bottom of the plot_station_data code, replace <b>delay(4000);</b> with <b>pause(4);</b>. Jay used the wrong programming language.</p>
</td>
</tr>
</tbody>
</table>
-->

In the last lesson, you created a script that processes and plots station data for a single station using a set reference period to calculate anomalies (i.e. 1951-1980). ***But what if you wanted to do the same analysis for other sites? For all sites? What if you wanted to change the reference period and run it again?*** This is where creating a function (where those preferences can be entered as inputs) becomes valuable. 
  
In this task, you need to complete the code in ```plot_station_data``` so that the function: 
- Allows a user to select one site to analyze by entering the name of a station's data file as it appears in ```/Data``` (e.g. ```ADELAIDE_AIRPORT.csv```, ```Dikson.csv```, etc.). Internally, this is assigned to the ```station_name``` variable.
- Allows a user to process all site data in ```/Data``` at once (in a loop) if they enter ```'all'``` in the place of a station file name.  
- Allows a user to specify the start (```ref_start```) and end (```end_year```) years for the *reference period* for calculating anomalies.
- Similar to the previous lesson, creates two png figures for each site: 
  - A *timeseries* figure named ```<stationName>_timeseries.png```, where ```<stationName>``` is the file name of the station data file, and 
  - A *barcode* figure named ```<stationName>_barcode.png```, where ```<stationName>``` is the file name of the station data file.
- Is properly commented in the top section and throughout the function.  
<br>
**NOTE** that the *function declaration* for ```plot_station_data``` has already been created to accommodate the inputs defined above: 
```
function [] = plot_station_data_soln(station_name, ref_start, ref_end)
```

### 2.1 Hints
- When you are ready to test your function, run each of the following lines in the Command Window separately to see if they create the desired outputs. **NOTE** That you must enter the name is it appears in the files (i.e., it is case sensitive):  
  - ```plot_station_data('Abashiri', 1961, 1990)```
  - ```plot_station_data('BAMBERG', 1971, 2000)```
  - ```plot_station_data('all', 1971, 2000)```

<!--
<table style="background-color: #ffff99;">
<tbody>
<tr>
<td>
<p><b>IMPORTANT NOTE:</b> For some reason, the Almaty dataset may be missing from the /Data folder in your MATLAB Drive; this will cause an error when trying to run the first example. To fix this issue, you can either: a) download the Almaty.csv file from your assignment GitHub repository and upload to the /Data folder in your MATLAB Drive, or b) simply test with a different station name as found in your /Data folder.</p>
</td>
</tr>
</tbody>
</table>
-->

## 3. Deliverables
- Ensure that all changes to your function ```plot_station_data``` is saved.
- **NOTE** that you are submitting the function and not the outputs (Jay is going to run the script on his computer to evaluate that it creates the proper outputs).

## 4. (Oh no, not another) Reflection
Don’t worry too much. This one is short and sweet. In 100 words or less, I would like to know what you thought of the workshop and the programming experience. *Was this a useful exercise? Do you see the benefits of taking a scripted approach to analysis? What was/wasn’t useful? Is there anything that you would have liked to have done differently?* Add your reflection to the ```reflection.md``` file in your assignment GitHub repository.

## 5. Ready to submit? 
Go to the [submission](a3-submission) page to prepare to submit your assignment. 
