# EDA on Spotify 2023

## Start
#### Function/s Used:
  - Import pandas as pd
  - Import numpy as np
  - Import matplotlib.pyplot as plt
  - Import seaborn as sns
  - pd.read_csv()

#### Documentation:
a. Importing necessary libraries
  - Initially import the pandas Library using import pandas as pd to access pandas functions.
  - Initially import the numpy Library using import numpy as np to access numpy functions.
  - Initially import the mathplot Library using import matplotlib.pyplot as plt to access matplotlib functions.
  - Initially import the seaborn Library using import seaborn as sns to access seaborn functions.
    
b. Read the CSV file
  - Using the function pd.read_csv('spotify-2023.csv'), the program then reads the CSV file "spotify-2023" from the repository.
    
Note: 
  - The spotify-2023.csv is an external file located at this repository or can be downloaded on, Most Streamed Spotify Songs 2023 (https://www.kaggle.com/datasets/nelgiriyewithana/top-spotify-songs-2023).

## Overview of Data Set
#### Function/s Used:
  - .shape()
  - .dtypes()
  - .isna().sum()

#### Documentation:
a. Number of Rows and Columns
  - Using the .shape function the rows and columns can now be counted and store it

b. Shows each data types
  - Using the .dtypes() function on the matrix collate the data types of the matrix and store it

c. Missing Value
  - Using the .isna() along with .sum() break down the matrix and make it numerical, after that finding the missing value only counts as less than zero or no value. 
  
Note:
- I only found .isna().sum() function from online sources

  ## Basic Descriptive Statistics
#### Function/s Used:
  - .tolist
  - pd.series()
  - pd.to_numeric(errors='coerce')
  - .isna().sum()
  - .dropna()
  - .mean()
  - .median()
  - .std()
  - plt.figure()
  - sns.histplot()
  - sns.boxplot()
  - plt.title()
  - plt.xlabel()
  - plt.ylabel()
  - plt.show()

#### Documentation:
a. Setup of list
  - In order to calculate any matrix, it needs to be in the correct setup. Using .tolist(), pd.series() and pd.to_numeric(errors='coerce'). These functions act as a "conversion" in order to make do with the data.
  - Also calculating data means that there must be no error or no value, using .isna().sum() to show if there are NaN values and .dropna() to basically remove it or exclude it from the data calculations.

b. Calculate the mean, median, and standard deviation
  - With all data in order, using .mean(), .median(), and .std() will compute their mean, median, and standard deviation, respectively.

c. Plot and Graphs
  - Using mathplot and sns Library, the graph of the data calculated can now be shown. 

Note:
- None 

## Top Performers
#### Function/s Used:
  - .loc[]
  - .nlargest()
  - pd.to_numeric(errors='coerce')
  - .value_counts()
  - .head()

#### Documentation:
a. Shows of Top streams 
  - As always use pd.to_numeric(errors='coerce') function to setup the data from the matrix to avoid error.
  - Using .loc[] in order to locate the top 1 streamed and .nlargest(#) to locate the top # within the matrix.

b. Shows the Top frequent artists
  - using .value_count() to collate the artist along with .head(#) for range of artist with a #

Note:
- None

## Temporal
#### Function/s Used:
  - .size()
  - .plot()
  - plt.title()
  - plt.xlabel()
  - plt.ylabel()
  - plt.show()
  - .idmax()
  - .max()

#### Documentation:
a. Groupings of time of tracks
  - Using .size() function will collate and organize the matrix of a given column's

b. Graphing of tracks
  - Using the standard .plot() function the specific time frame and the number of tracks

c. Top track in a month time frame
  - Using .idmax() we can located which month it was and .max() for how many that month contains

Note:
- None

## Genre and Music Characterization
#### Function/s Used:
  - .corr()
  - .loc[]
    
#### Documentation:
a. Correlation of Characterization
  - Using the .corr() function which is in its name "corr" it will correlate the given datatypes from the matrix

b. Correlation between danceability and acousticness
  - Using the .loc[] function the correlation between danceability and acousticness can now be located and shown
  
c. Correlation between valence and acousticness
  - Using the .loc[] function the correlation between valence and acousticness can now be located and shown
    
Note:
- None

## Platform Popularity
#### Function/s Used:
  - .sum()
  - .mean()
  - .items()
  - plt.figure()
  - plt.bar()
  - plt.title()
  - plt.xlabel()
  - plt.ylabel()
  - plt.show()

#### Documentation:
a. Platform Calculations
  - Using the .sum() and .mean() functions, calculate the total and the average of the given platform.

b. Comparison of Platforms
  - Storing all platforms in one value to collate them for comparison later in the graph
  - Using the plt.bar() the graph will show the comparison of each of the platforms given with respect to the total appearance from each platform

Note:
- None

## Advance Analysis
#### Function/s Used:
  - .groupby()
  - .mean()
  - .unstack()
  - plt.figure()
  - sns.heatmap()
  - plt.title()
  - plt.xlabel()
  - plt.ylabel()
  - plt.show()

#### Documentation:
a. Pattern of same key and/or mode
  - Using the .groupby() along with .mean().unstack(), will then group the given data types 

b. Graphing of the pattern data
  - Using the sns.heatmap() functions, the pattern can now be seen in a heatmap graph with scaling "heat" values and the comparison between both the major and minor

c. Total appearance of artist in playlist and charts
  - Also using the .groupby() function along with .sum(), groups the artist in order.
  - using .nlargest(#) function shows the range of top # of artist.

d. Using the standard .plot() with a 'kind=bar', the graph of each artist can now be shown in a bar graph.

Note:
- I only found the .groupby().mean().unstack() from online sources

## Updates:
- Posted EDA on Spotify.ipynb File (Incomplete)
- Added spotify-2023.csv File
- Added ReadMe File (Incomplete)
- Reposted EDA on Spotify.ipynb File (Complete)
- Update ReadMeFile (Complete)
- 

