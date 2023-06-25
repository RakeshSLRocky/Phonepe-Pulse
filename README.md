<h1 align="center"> Phonepe_Pulse Data Visualisation</h1>

**Problem Statement**
```bash
The Phonepe pulse Github repository contains a large amount of data related to
various metrics and statistics. The goal is to extract this data and process it to obtain
insights and information that can be visualized in a user-friendly manner.
```
## Installations
Install the below packages

```bash
import streamlit as st
from streamlit_option_menu import option_menu
import pandas as pd
import mysql.connector as msql
from babel.numbers import format_currency
from PIL import Image
import webbrowser
import plotly.express as px
import plotly.graph_objects as go
import base64
import ast
```

## Clone the data from phonepe pulse Repository

```bash
# Funtion to clone the data from phonepe github repository
def clone():

    repo_url = "https://github.com/PhonePe/pulse.git" #path of repo need to be cloned
    clone_path = r"D:\Phonepe_pluse"   #path where to store

    if not os.path.exists(clone_path):
        os.makedirs(clone_path)

    Repo.clone_from(repo_url, clone_path)
# calling the function to clone
clone()
```
## Creating  Data-Tables 

After Cloning data from Git-hub repository create a corresponding DataFrame of given pulse data's and insert it into SQL database and transform the tables as per the requirement  


## Create SQL queries to fetch the data from database

```python
SELECT * FROM "Table"
WHERE "Condition"
GROUP BY "Columns"
ORDER BY "Data"
```
## Let's have some visualizations with streamlit - webpage

## Home

![Home](https://github.com/RakeshSLRocky/Phonepe-Pulse/blob/main/images/Home.png)

## MAP

![top queries](https://github.com/RakeshSLRocky/Phonepe-Pulse/blob/main/images/Map.png)

## Insights

![customized queries](https://github.com/RakeshSLRocky/Phonepe-Pulse/blob/main/images/Insights.png)

## Support

For support, email : rakeshslrocky@gmail.com

