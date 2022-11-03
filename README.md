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
- $\alpha$ (Significance level): 0.05

![mpaa](https://github.com/bustyAI/Movie-Project/blob/main/assets/mpaa%20rating.PNG)

- Using Kruskal-Wallis test we received a p-value of 1.15e<sup>-98</sup>
- Reject the null hypothesis, so MPAA rating does have an affect on the revenue that a movie generates.
- From the graph we can see that movies rated PG-13 and PG generate significantly more revenue than those rated R and G
- One reason PG and PG-13 rated movies generate more revenue is because the target audience. Since almost anyone can go in and watch the movie, it would make sense that for those to generate more revenue.
- Another reason could be that parents take their kids to watch these movies. Not only do they pay for their kids tickets but also theirs increasing the amount of tickets sold.
#

### Is there a difference in rating between movies that are 2 hours long or less than 2 hours long?

- H<sub>0</sub> (Null Hypothesis): There is no difference in rating between movies that are over 2 hours or less than 2 hours.
- H<sub>1</sub> (Alternate Hypothesis): There is a difference in rating betwen movies that are over 2 hours long or less than 2 hours long.
- $\alpha$ (Significance level): 0.05

![length](https://github.com/bustyAI/Movie-Project/blob/main/assets/length.PNG)

- Using Welch's T-Test we received a p-value of 0.0
- Reject the null hypothesis, so there is a difference in rating between movies that are over 2 hours long or less than 2 hours long.
- From the graph we can see that the mean rating for movies that are over 2 hours is greater than the mean rating for movies less than 2 hours long.
#

### Does genre affect the amount of revenue a movie generates?

- H<sub>0</sub> (Null Hypothesis): Different genres generate the same amount of revenue.
- H<sub>1</sub> (Alternate Hypothesis): Different genres generate different amounts of revenue.
- $\alpha$ (Significance level): 0.05

![genre](https://github.com/bustyAI/Movie-Project/blob/main/assets/genre.PNG)

- Using Kruskal-Wallis test we received a p-value of 1.53<sup>-230</sup>
- Reject the null hypothesis, so different genres generate different amounts of revenue.
- From the graph we can see that Adventure, Sci-Fi, Animation, and Fantasy generate the most revenue.
