# Does Size Matter?
### _The Impact of College Football Player Size on Team Success_

Final Project for Columbia University STAT 4001: Probability & Statistics - Spring 2023 by [Sean Osier](mailto:smo2152@columbia.edu)

## Abstract

We explore the variability and importance of player size in top-level (FBS, formerly Division 1-A) college football. Looking at height, weight, and Body Mass Index (BMI), we demonstrate that there are statistically significant differences in the average size of players playing different positions. More importantly, we demonstrate that “team size” has a small, but statistically significant impact on a team’s ultimate success as measured by wins and losses. In doing so, we determine that weight is the measure of size most correlated with team success. Finally, we identify Tight End (TE), Defensive Line (DL), and Defensive Back (DB) as the positions where size differences matter most (simultaneously revealing that size differences at other positions don’t have a statistically significant impact).

<img width="794" alt="image" src="https://github.com/user-attachments/assets/19c28021-cfa1-418e-8fc4-433fb0f437c7" />

<img width="787" alt="image" src="https://github.com/user-attachments/assets/3d3ad6e0-c29f-497f-9517-99a6caf2951c" />

## Full Results

For full results see the [report](report.pdf).

## How to Run the Code / Replicate Our Experiments

1. All data used can be found in the [`data/`](data/) folder.
   - (Optional) The [Get_Save_CFB_Data.ipynb](data/Get_Save_CFB_Data.ipynb) notebook can be used to pull the data again if necessary:
     - This requires a [College Football Data (CFBD) API](https://api.collegefootballdata.com/api/docs/?url=/api-docs.json) key
     - The code assumes the API key is stored in a `.env` file, but you can pass in the API key however you like by replacing `os.getenv("CFBD_API_KEY")` in the first cell of the notebook
2. All the analysis code can be found in the [CFB_Player_Size_Exploration.Rmd](CFB_Player_Size_Exploration.Rmd) notebook
   - This file expects the data has already been retrieved (see #1 above)
   - It requires the common `tidyverse` and `glue` R packages to be installed, but there are otherwise no special dependencies
