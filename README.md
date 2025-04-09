![Covid image](https://github.com/BiswaRanjan8596/Covid19/blob/main/Effective-Data-Visualization-In-the-Era-of-COVID-19.jpg)


Covid-19 Analysis and Visualization using Plotly Express
Last Updated : 02 Sep, 2024
In this article, we will discuss Analyse Covid-19 data and will visualize it using Plotly Express in Python. This article deals with creating dozens of bar charts, line graphs, bubble charts, scatter plots. The graph that will be made in this project will be of excellent quality. Envisioning COVID-19 will primarily be using Plotly Express for this project. The analysis and visualization enable people to understand complex scenarios and make predictions about the future from the current situation.

This analysis summarizes the modeling, simulation, and analytics work around the COVID-19 outbreak around the world from the perspective of data science and visual analytics. It examines the impact of best practices and preventive measures in various sectors and enables outbreaks to be managed with available health resources.

Tools and Technologies Used in the Project: Google Colab(Runtime type – GPU).

Requirements to Build the Project: 

Basic knowledge of Python
Basic understanding of graphs and charts
Data visualization
Pandas
Numpy
Matplotlib
Plotly Express
Choropleth
Wordcloud
Stepwise Implementation
Step 1: Importing Necessary Libraries
The task is simple, once the installation of all the required libraries is successful, they need to be imported to the working space, since they will provide the additional support for analysis and visualization.

Example: importing libraries


# Data analysis and Manipulation
import plotly.graph_objs as go
import plotly.io as pio
import plotly.express as px
import pandas as pd

# Data Visualization
import matplotlib.pyplot as plt

# Importing Plotly
import plotly.offline as py
py.init_notebook_mode(connected=True)

# Initializing Plotly
pio.renderers.default = 'colab'
Step 2: Importing the Datasets
Importing three datasets into this project

covid– This dataset contains Country/Region, Continent,  Population, TotalCases, NewCases, TotalDeaths, NewDeaths,  TotalRecovered, NewRecovered, ActiveCases, Serious, Critical, Tot Cases/1M pop, Deaths/1M pop, TotalTests, Tests/1M pop, WHO Region, iso_alpha.
covid_grouped– This dataset contains Date(from 20-01-22 to 20-07-27), Country/Region, Confirmed, Deaths, Recovered, Active, New cases, New deaths, New recovered, WHO Region, iso_alpha.
coviddeath– This dataset contains real-world examples of a number of Covid-19 deaths and the reasons behind the deaths.
To import datasets to the working space pandas read_csv() method can be used.

Syntax:

read_csv(path)


