# Exploratory-Data-Analysis
# Introduction

This assignment uses data from the UC Irvine Machine Learning Repository, a popular repository for machine learning datasets. In particular, we will be using the "Individual household electric power consumption Data Set" which I have made available on the course web site:

Dataset: Electric power consumption [20Mb]

Description: Measurements of electric power consumption in one household with a one-minute sampling rate over a period of almost 4 years. Different electrical quantities and some sub-metering values are available.

The following descriptions of the 9 variables in the dataset are taken from the UCI web site:

Date: Date in format dd/mm/yyyy
Time: time in format hh:mm:ss
Global_active_power: household global minute-averaged active power (in kilowatt)
Global_reactive_power: household global minute-averaged reactive power (in kilowatt)
Voltage: minute-averaged voltage (in volt)
Global_intensity: household global minute-averaged current intensity (in ampere)
Sub_metering_1: energy sub-metering No. 1 (in watt-hour of active energy). It corresponds to the kitchen, containing mainly a dishwasher, an oven and a microwave (hot plates are not electric but gas powered).
Sub_metering_2: energy sub-metering No. 2 (in watt-hour of active energy). It corresponds to the laundry room, containing a washing-machine, a tumble-drier, a refrigerator and a light.
Sub_metering_3: energy sub-metering No. 3 (in watt-hour of active energy). It corresponds to an electric water-heater and an air-conditioner.
# Loading the data

data.frame':	2075259 obs. of  9 variables:
 $ Date                 : Factor w/ 1442 levels "1/1/2007","1/1/2008",..: 342 342 342 342 342 342 342 342 342 342 ...
 $ Time                 : Factor w/ 1440 levels "00:00:00","00:01:00",..: 1045 1046 1047 1048 1049 1050 1051 1052 1053 1054 ...
 $ Global_active_power  : Factor w/ 4187 levels "?","0.076","0.078",..: 2082 2654 2661 2668 1807 1734 1825 1824 1808 1805 ...
 $ Global_reactive_power: Factor w/ 533 levels "?","0.000","0.046",..: 189 198 229 231 244 241 240 240 235 235 ...
 $ Voltage              : Factor w/ 2838 levels "?","223.200",..: 992 871 837 882 1076 1010 1017 1030 907 894 ...
 $ Global_intensity     : Factor w/ 222 levels "?","0.200","0.400",..: 53 81 81 81 40 36 40 40 40 40 ...
 $ Sub_metering_1       : Factor w/ 89 levels "?","0.000","1.000",..: 2 2 2 2 2 2 2 2 2 2 ...
 $ Sub_metering_2       : Factor w/ 82 levels "?","0.000","1.000",..: 3 3 14 3 3 14 3 3 3 14 ...
 $ Sub_metering_3       : num  17 16 17 17 17 17 17 17 17 16 ...


We will only be using data from the dates 2007-02-01 and 2007-02-02. One alternative is to read the data from just those dates rather than reading in the entire dataset and subsetting to those dates.

You may find it useful to convert the Date and Time variables to Date/Time classes in R using the strptime() and as.Date() functions.

Note that in this dataset missing values are coded as ?.

# Making Plots

Our overall goal here is simply to examine how household energy usage varies over a 2-day period in February, 2007. Your task is to reconstruct the following plots below, all of which were constructed using the base plotting system.

First you will need to fork and clone the following GitHub repository: https://github.com/rdpeng/ExData_Plotting1

For each plot you should

Construct the plot and save it to a PNG file with a width of 480 pixels and a height of 480 pixels.

Name each of the plot files as plot1.png, plot2.png, etc.

Create a separate R code file (plot1.R, plot2.R, etc.) that constructs the corresponding plot, i.e. code in plot1.R constructs the plot1.png plot. Your code file should include code for reading the data so that the plot can be fully reproduced. You should also include the code that creates the PNG file.

Add the PNG file and R code file to your git repository

When you are finished with the assignment, push your git repository to GitHub so that the GitHub version of your repository is up to date. There should be four PNG files and four R code files.
