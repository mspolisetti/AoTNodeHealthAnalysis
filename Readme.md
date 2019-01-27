Data Format: AoT nodes collect data in Time Series format. Sensor readings represent the changes in environment around them over time. We were to extract data for 20+ sensors of each of the 90+ nodes. Each of this sensors record a reading once every 5 seconds or so.

Data Storage : Our data was typically big, with complete CSV file needing storage of around 200GB. Data for this project was stored in a Cassandra database. Data is streamed from the Database into CSV files for public use. 

Output of our Analysis : Goal of our project was to identify failures in the nodes and there by hone into various factors that potentially impact failure of these nodes over time.  Output of the analysis was saved in GitHub and presented to our project leader. This analysis will further be used in future work that involves predicting remaining useful life(RUL) of these AoT Nodes.

Our team will writing a paper detailing our work towards the summer of 2019.

Tools/Algorithms/methods :
Our team downloaded data and separated data into monthly files using tools developed in Python for our exploration purposes.  We developed a R program that would read monthly datasets and extract node-wise files for analysis.

We used R packages (for e.g: dplyr) & Python libraries  to tabulate data for exploration. We used packages such as purr and ggplot2 for our visualizations in R. We used Python Seaborn heatmaps for visualizing failure patterns.

We also used Tableau for finer visualizations. 
