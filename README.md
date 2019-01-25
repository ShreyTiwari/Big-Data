# IPL Match Simulation and Score Prediction.

This repository contains the files related to the project that was carried out as a part of the 'Big Data' course.<br />
The main phases of the project are placed in different dictories:<br />
- Data<br />
- Clustering<br />
- Probabilities<br />
- Test (Final simulation using decision trees)<br /><br />

## Data
This directory contains the data that will be used for the project. The data is got from online sources such as cricsheets, cricinfo, espn...etc. The folder also contains scripts for converting data into suitable format. An important part of the project was to build player profiles. The player profiles are present here and have been scraped off different website pages.<br /><br />

## Clustering
This is a preprocessing performed on the data to make sense and gain insights about the player to player similarities. The codes are written in scala and packaged into jars using the sbt tool. The K-Means algorithm uses the Spark MlLib library so as to maximize performance and scalability.<br /><br />

## Probabilities
Here we perform some processing on the data and use the results to train our future machine learning models. The players are grouped together using K-Means and then we try to find out the probabilities of different events for two given groups/ players. Ex: If Virat is batting and Z Khan is bowling what is the probabiliy of a four being scored. For further information see the ProjectDoc file.

## Test
There we try to simulate the matches, try to predict the scores and end result of the matches. The input to the matches is in a specific format and the simulation code reads this format of input only. If format of input is to be changed, the code can be modified easily.
