# Model-based-clustering-classification-and-Mem-Analysis-of-Performance-and-Salaries-of-NBA-Players
In this project I've applied different methods to extract patterns in the performance and salaries of NBA players. I've used mixture models, model based clustering, model based classification and model based clustering with covariates to understand connection between the salaries and the performance  during the games of players. 
## Overview
This project analyzes the relationship between the **performance** and **salaries** of NBA players during the **2017–2018 season**.  
It was developed as part of an academic project by *Giulia de Innocentiis* and *Tommaso Pozzi*.

## Objectives
- Explore and clean the datasets containing player statistics and salary information.  
- Create per-game performance metrics (e.g., PPG, RPG, APG, etc.) for better comparability among players.  
- Investigate patterns and relationships between player performance and compensation levels.  
- Apply statistical and clustering models to identify groups of players with similar characteristics.

## Data
The analysis is based on two datasets:
- `Seasons_Stats.csv` — comprehensive NBA player performance data (2017–2018 season).  
- `NBA_season1718_salary.csv` — salary data for the same set of players.

Both datasets were merged using the common variable `Player`, and observations with missing values were removed when necessary.

## Methods and Tools
The analysis was conducted in **R** using the following packages:
- `tidyverse`, `data.table` — data cleaning and manipulation  
- `corrplot`, `GGally`, `PerformanceAnalytics`, `plotly` — exploratory and graphical analysis  
- `mclust`, `Rmixmod`, `flexmix`, `caret` — clustering and statistical modeling  

## Results
The project explores how different performance indicators (e.g., scoring, assists, rebounds) correlate with player salaries.  
Clustering techniques are used to group players by performance and examine salary distributions within clusters.

## Reproducibility
To reproduce the analysis:
```r
# Required packages
library(data.table)
library(tidyverse)
library(mclust)
library(caret)
# ...

# Run the R Markdown file
rmarkdown::render("deInnocentiis_Pozzi_appendice.Rmd")
