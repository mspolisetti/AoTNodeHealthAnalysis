## Problem Statement :

The Array of things (AoT) project is an urban sensing project involving collaboration of the University of Chicago, Argonne National Laboratory, and the School of the Art Institute of Chicago. As part of the new Smart Cities Initiative announced in 2015, AoT will provide real-time, location-based data about urban environment, infrastructure and activity to researchers and the public. This initiative has the potential to allow researchers, policymakers, developers and residents to work together and take specific actions that will make cities healthier, more efficient and more livable.

 As part of the project, a network of interactive, modular sensor boxes is installed around Chicago to collect real-time data of the city’s environment, infrastructure, and activity. The first set of nodes started measuring factors such as barometric pressure, light, carbon monoxide, ambient sound, and temperature since 2017.  In partnership with the City of Chicago, a total of 500 nodes will be mounted on street light traffic signal poles around the city over two to three years timespan.
Our capstone project is about developing a methodology for analyzing health of these AoT Nodes, identifying various factors affecting the health of the Nodes, and predicting malfunction within a given future time period. 
 
Currently AoT project lacks 

(1) Data-driven evaluation of the health of the existing AoT nodes 

(2) Data-driven analysis or explainability of factors that will be key in assessing health of AoT Node - Factors such as sensors manufacturer’s brand, installation date, node’s location, power stability  and weather conditions. 

Also, (3) AoT Project lacks an Analytical tool that can effectively predict possible malfunctions ahead of time and predict and assign sensor readings in case of a malfunction. 
 
These shortcomings slow down AoT project’s efforts in designing and installing second and third generations of sensor nodes to capture consistent and infallible data. 

## Research Purpose:

The purpose of this research is to develop an analytical tool that could enable data-driven evaluation of the existing AoT Node health and explain the various factors affecting Node’s health. In addition, we will develop analytical tools that can effectively predict possible malfunctions based on historical data. Lastly, we might develop analytical tools to predict sensor readings in case of a malfunction. In particular, the research aims to achieve the following objectives:
Define the health of sensor nodes and develop an automated data analysis method  to label  malfunctions in  a given Node
Develop a classification method to predict malfunctioning node and explain various factors that are common across malfunctioning nodes. Some examples of factors affecting the AoT Node health are : types of sensors on the node, installation date, manufacturer’s brand, weather conditions, and node location.
Develop a tool to predict remaining lifetime of an AoT Node given characteristics such as manufacturer’s brand, weather conditions, location and other factors identified in Step 2.
Impute sensor readings using analytical tools developed, in case of a malfunction and when appropriate.


### Data Format: 

AoT nodes collect data in Time Series format. Sensor readings represent the changes in environment around them over time. We were to extract data for 20+ sensors of each of the 90+ nodes. Each of this sensors record a reading once every 5 seconds or so.

### Data Storage : 

Our data was typically big, with complete CSV file needing storage of around 200GB. Data for this project was stored in a Cassandra database. Data is streamed from the Database into CSV files for public use. 

### Output of our Analysis : 

Goal of our project was to identify failures in the nodes and there by hone into various factors that potentially impact failure of these nodes over time.  Output of the analysis was saved in GitHub and presented to our project leader. This analysis will further be used in future work that involves predicting remaining useful life(RUL) of these AoT Nodes.

Our team will writing a paper detailing our work towards the summer of 2019.

### Tools/Algorithms/methods :

Our team downloaded data and separated data into monthly files using tools developed in Python for our exploration purposes.  We developed a R program that would read monthly datasets and extract node-wise files for analysis.

We used R packages (for e.g: dplyr) & Python libraries  to tabulate data for exploration. We used packages such as purr and ggplot2 for our visualizations in R. We used Python Seaborn heatmaps for visualizing failure patterns.

We also used Tableau for finer visualizations. 
