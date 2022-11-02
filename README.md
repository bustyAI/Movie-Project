# Movie-Project

### What makes a good movie? Is it revenue, budget, or Robert De Niro?

![goodfellas](https://github.com/bustyAI/Movie-Project/blob/main/assets/goodfellas.png)

 # Project Goal
- For this project I analyzed data from the tmdb and imdb database to find out what exactly makes a good movie. As someone who enjoys watching movies this was a very interesting project for me. 

# Tools Used
***Click on folders for coresponding notebooks with libraries used***
- :snake: Python

### EDA
- :panda_face: pandas, matplotlib, seaborn --> [:open_file_folder:](https://github.com/bustyAI/Movie-Project/tree/main/EDA)

### Extract
- :cloud: os, json, tmdbsimple, tqdm.notebook --> [:open_file_folder:](https://github.com/bustyAI/Movie-Project/tree/main/Extracting)

### Transform/Load
- :rocket: pymysql, sqlalchemy, sqlalchemy_utils --> [:open_file_folder:](https://github.com/bustyAI/Movie-Project/tree/main/Transforming) [:open_file_folder:](https://github.com/bustyAI/Movie-Project/tree/main/Loading)

### Hypothesis Testing
- :chart_with_upwards_trend: numpy, scipy --> [:open_file_folder:](https://github.com/bustyAI/Movie-Project/tree/main/Hypothesis_Testing)
#

# Outcome
### Does MPAA rating affect how much revenue a movie generates?

- H<sub>0</sub> (Null Hypothesis): Different MPAA rating does not affect the revenue a movie generates.
- H<sub>1</sub> (Alternate Hypothesis): Different MPAA rating does affect the revenue a movie generates.

![mpaa](https://github.com/bustyAI/Movie-Project/blob/main/assets/mpaa%20rating.PNG)

- Using Kruskal-Wallis test we recieved a p-value of 1.15e<sup>-98</sup> less than 0.05
- Reject the null hypothesis, so MPAA rating does have an affect on the revenue that a movie generates.
- From the graph we can see that movies rated PG-13 and PG generate significantly more revenue than those rated R and G
