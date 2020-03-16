# final-project-WaleedIftikhar-SameerSwarup
A repository for our final project which aims to answer one of the most important questions of all time: Ronaldo or Messi. 
**link**:

## Datasets
1. *MessiComplete.csv:* 
   This dataset contains statistics (appearances, goals and assists)  on the performance of Lionel Messi over a period of 17 years from 2004-2020. The statistics have been scraped from various different websites. The dataset contains the total of each type of statistic and there are also variables that breakdown these statistics into country and club. E.g. The dataset contains the total number of Goals Messi scored in 2019 and how many of those he scored while playing for his club, FC Barcelona, and how many he scored playing for his country: Argentina.
2. *RonaldoComplete.csv:*
   It is the exact same dataset as `MessiComplete.csv` in that it contains the exact same information as that Dataset just for Cristiano Ronaldo.
3. *TrophyComparsion.csv:*
   It contains data on the number of team trophies won by both players over their playing careers up to this point. The three types of trophies that we are considering include the European Cup (a competition between the top soccer clubs in Europe), the National League (a competition between the first division clubs in a particular country e.g England) and the Domestic League (a competition between the first, second and third division clubs in a particular country).
 4. *MessiRonaldoComplete.csv:*
    This is a complete version of our dataset which gather the MessiComplete.csv, RonaldoComplete.csv and the TrophyComparison.csv datasets. It also contains the variable `BallonDor` which is an annual award given to the best soccer player of the year. We aim to use this dataset for statistical learning purposes splitting it into a test and training dataset to fit a model on the training data, eventually choosing the model which has the highest accuracy in predicting the BallonDor winner based on the entries in the test dataset. 
5. *MessiRonaldoLonger.csv:*
   This is a longer version of `MessiRonaldoComplete.csv` and it only contains the quantitative variables. It contains the same data with twice the number of rows and half the number of columns. We created this dataset to conduct different types of data visualizations. 
6. *messiAndRonaldoLaLiga.csv*: Since we also aim to compare the performance of the two players in the same league, in this dataset we are comparing the Goals, Assists and Appearances of both Players in La Liga (the Spanish national soccer league). Ronaldo played for Real Madrid (in Spain) between 2009 and 2018 during which both players often came face to face with each other. This dataset will allow us to determine which player fared better during the time period that both players were playing in La Liga.
7. *messiAndRonaldoUEFA.csv*: Much like the `messiAndRonaldoLaLiga.csv` dataset, this dataset compares the two performance of the two players in the UEFA Champions League/European Cup (the biggest soccer tournament for soccer clubs in Europe). This dataset will allow us to determine who was the better player on the biggest stage of them all.
   
## .Rmd Files 
1. *Scraping and Analysis.Rmd:* 
   This file shows our web scraping process where we scraped data from various websites including Wikipedia, and sites dedicated to comparing the performance of the two players such as `messivsronaldo.net`. We scraped data from tables and containers on these web pages. We then cleaned these datasets, inserted appropriate variables where required and then gathered datasets to create two final versions of our data which were `MessiRonaldoComplete.csv` and `MessiRonaldoLonger.csv`. This is an **important file that should be considered to understand our data collection process**.
2. *BlogPost.Rmd:*
   **This is our most important file.** This file has been ultimately published to our website. It contains **the code which we used to display our datasets in the form of tabs, as well as our interactive scatterplots, and histograms**. Most of this code is hidden in our final output. Therefore, to understand our process in greater detail, this file should be considered. It also contains an overview of the final logistic regression model we chose. To view the various statistical learning models we tried before choosing this model, refer to `Scraping and Analysis.Rmd`.
