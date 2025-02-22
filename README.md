# Data exploration and analysis with DataViz
Dateset Used: ATP matches dataset | All atp matches between 2000 and March 2018
Downloaded in Kaggle: https://www.kaggle.com/datasets/edouardthomas/atp-matches-dataset?resource=download
Available for Download (FREE)
Dataset is paired with another dataset named Confidence Data. The 2nd dataset describes the PSW numbers.


# or Rows: 44708
# of Columns: 23

# Columns Descriptions:
1. ATP: The ATP tournament number, which is a unique identifier for each ATP tournament in the dataset.
2. Location: The location where the tournament was held, such as a city or country.
3. Tournament: The name of the tournament.
4. Date: The date on which the match was played.
5. Series: The ATP tournament series, which indicates the level of the tournament (e.g. Grand Slam, Masters 1000, ATP 500, etc.).
6. Court: The type of court where the match was played (e.g. indoor, outdoor).
7. Surface: The type of playing surface where the match was played (e.g. clay, grass, hard court).
8. Round: The round of the tournament in which the match was played (e.g. first round, quarterfinals, etc.).
9. Best of: The number of sets needed to win the match (e.g. best of three, best of five).
10. Winner: The name of the player who won the match.
11. Loser: The name of the player who lost the match.
12. WRank: The ATP ranking of the winning player at the time of the match.
13. LRank: The ATP ranking of the losing player at the time of the match.
14. Wsets: The number of sets won by the winning player.
15. Lsets: The number of sets won by the losing player.
16. Comment: Additional information about the match (e.g. retirement, walkover, etc.).
17. PSW: The odds of the winning player according to Pinnacle Sports.
18. PSL: The odds of the losing player according to Pinnacle Sports.
19. B365W: The odds of the winning player according to Bet365.
20. B365L: The odds of the losing player according to Bet365.
21. elo_winner: The Elo rating of the winning player before the match.
22. elo_loser: The Elo rating of the losing player before the match.
23. proba_elo: The probability of the winning player winning the match according to the Elo ratings.

# Introduction

CONTEXT

Integration into your business:
If your business is in the tennis industry or you offer services related to tennis, such as coaching or equipment sales, the ATP matches dataset can be useful for market research, trend analysis, and player performance evaluation. For example, dataset can be used to identify popular tournaments and players, analyze the popularity of different court surfaces, and track player rankings over time. This information can help make informed business decisions, such as which tournaments to sponsor or which players to hire for endorsement deals.

Technical point of view:
The ATP matches dataset contains data on more than 50,000 matches played between 2000 and March 2018, including information on the players, tournament, surface, and outcome. The dataset is in a structured format and can be easily imported into a variety of data analysis tools, such as Python, R, and Excel. It can be used for various data analysis tasks, including data visualization, statistical analysis, and machine learning.

Economic point of view:
The ATP matches dataset can be valuable for businesses in the tennis industry as well as for sports betting companies. By analyzing the historical data, businesses can make informed decisions about where to allocate their resources and make profitable investments. For example, sports betting companies can use the dataset to develop betting strategies and adjust their odds based on the performance of individual players and tournaments.

Scientific point of view:
The ATP matches dataset can be used by researchers to study various aspects of tennis, including player performance, tournament outcomes, and the effects of different court surfaces on player performance. Researchers can also use the dataset to test hypotheses and develop new theories about the game of tennis. The dataset can be used in conjunction with other data sources, such as weather data and player demographics, to perform more complex analyses and gain deeper insights into the game.

# OBJECTIVE

This ATP matches dataset is to provide a comprehensive data source for analyzing professional men's tennis matches played between 2000 and March 2018. The dataset includes information on the location, tournament, date, court, surface, round, best of, winner, loser, rank, sets won, and odds for each match.

This dataset can contribute to the understanding of the performance and trends in men's professional tennis over an 18-year period. It can also help identify patterns and correlations between various factors such as location, court type, and player rankings. This dataset can be used by analysts, researchers, and tennis enthusiasts for various purposes such as player performance analysis, match prediction, and trend analysis.

# POTENTIAL ISSUES

Potential issues with the dataset that needs to check:

Missing values: As we saw earlier, some columns have a significant number of missing values. Depending on the analysis you want to do, you may need to deal with these missing values.

Outliers: There may be outliers in the data, which could affect the results of your analysis. You may need to identify and handle these outliers appropriately.

Data quality: It's important to ensure that the data is accurate and reliable. This could include checking for typos or other errors in the data.

Data consistency: The data should be consistent across all columns. For example, if the tournament name is spelled differently in different rows, this could cause issues when trying to group or analyze the data.

Data integrity: Ensure that the data has not been tampered with or altered in any way.

Data format: The data should be in a consistent format across all columns. For example, if the date is not in a standardized format, this could make it difficult to perform analyses based on date.

Data relevance: Ensure that the data is relevant to the analysis you want to perform. For example, if you are analyzing data from a specific time period, ensure that the data is from that time period.


References
Quantitative: This refers to variables that can take on numeric values and can be measured on a continuous or discrete scale. Examples include age, height, weight, and income.

Categorical - Binary: This refers to variables that have only two possible values, often represented as 0 and 1 or as yes and no. Examples include gender (male/female), smoker (yes/no), and married (yes/no).

Categorical - 3 to 5 categories: This refers to variables that have a small number of categories, typically between 3 and 5. Examples include educational level (high school, some college, college graduate), job type (managerial, professional, administrative, manual, other), and marital status (single, married, divorced, widowed).

Categorical - 6 to 10 categories: This refers to variables that have a moderate number of categories, typically between 6 and 10. Examples include race/ethnicity, type of housing (house, apartment, condo, etc.), and level of satisfaction (very dissatisfied, somewhat dissatisfied, neutral, somewhat satisfied, very satisfied).

Categorical - more than 10 categories: This refers to variables that have a large number of categories, typically more than 10. Examples include occupation, industry, and type of car.

Unique Value: This refers to variables that have a unique value for each observation in the dataset, such as an ID number or a name.

General Rule: Data Cleaning before data manipulation:
1. Cross-validation
2. Hypothesis testing
3. Replication
4. Statistical Tests
5. Peer Review - Can do
6. Visualizations - Can do

REFERENCE ELO RATING:
A. Below 1400: Beginner level players who are new to the sport or have limited experience

B. 1400-1600: Novice to intermediate level players who have some experience and knowledge of the game

C. 1600-1800: Intermediate to advanced level players who have been playing for a few years and have developed a strong understanding of the game

D. 1800-2000: Advanced to expert level players who have significant experience and skill in the game and may have competed in local or regional tournaments

E. 2000 and above: Elite level players who have exceptional skill and experience and may compete at a national or international level

PSW - so much missing values that we cannot really identify how it was created based on the dataset.
The PSW (Pinnacle Sports' Winning percentage) is a proprietary algorithm used by Pinnacle Sports to estimate the probability of a team winning a match. The exact details of how the PSW is calculated are not publicly available, but it is likely based on a combination of factors such as team performance history, team and player statistics, and other relevant factors.

Pinnacle Sports has a reputation for being one of the most accurate and reliable sportsbooks in the industry, and their PSW algorithm is one of the reasons for this. However, like any algorithm, it is not perfect and can sometimes be inaccurate in its predictions. This is where using alternative methods, such as Elo ratings and win percentages, can be useful for making more accurate predictions.

# MOST RELEVANT VARIABLES
Based on your objective of beating bookmakers' algorithms on estimating the probability of a team winning a match,
SUGGESTION: consider to check the following combinations:

1. Tournament, Surface, and Round
For the combination of Tournament, Surface, and Round, this would show how players perform on different surfaces across different rounds of a tournament. For example, could analyze how the performance of players varies between the early rounds and the later rounds, or how certain players perform better on certain surfaces in different rounds. This could potentially help in predicting which players might have an advantage in certain matchups.

2. Location, Surface, and Round
For the combination of Location, Surface, and Round, this would show how players perform on different surfaces across different locations. For example, could analyze how certain players perform better on grass surfaces in Europe versus grass surfaces in North America, or how players might perform differently on clay surfaces in South America versus clay surfaces in Europe. This could potentially help in predicting which players might have an advantage in certain matchups based on their past performances in similar conditions.

3. Surface, Round, and Best of
For the combination of Surface, Round, and Best of, this could potentially show how players perform under different conditions of a match. Best of determines how many sets are required to win the match, so this could help to understand how players might perform under pressure in a 3-set versus a 5-set match on different surfaces. It could also help to identify which players might have an advantage in shorter or longer matches on certain surfaces.

These combinations can help you identify any trends or patterns that may exist between these variables and the probability of a team winning a match. However, it is important to keep in mind that these variables alone may not provide a complete picture, and you may need to consider other factors such as the players' current form, head-to-head records, and injuries.

OTHER STUDIES
The time varying player-specific abilities for different court surfaces are of key importance for analyzing tennis matches.
Consider several other extensions including player-specific explanatory variables and the accountance of specific configurations for Grand Slam tournaments. The estimation results can be used to construct rankings of players for different court surface types.

REFERENCE TO REVIEW:
https://www.econstor.eu/bitstream/10419/177699/1/18009.pdf
TITLE: The analysis and forecasting of ATP tennis matches using a high-dimensional dynamic model

# GRAPHICAL REPRESENTATIONS WITH INTERPRETATION

# Graph #1
>>> The graph shows the frequency of each tournament series in the dataset. The dataset contains matches from eight different tournament series, namely International, ATP250, Grand Slam, Masters, Masters 1000, ATP500, International Gold, and Masters Cup. The International series has the highest frequency with 10792 matches, followed by ATP250 with 9550 matches and Grand Slam with 8255 matches. The Masters Cup series has the lowest frequency with only 240 matches.

>>> The graph also provides insights into the distribution of tournaments across different levels of prestige, with the International and ATP250 series representing the lower-tier tournaments and the Grand Slam and Masters 1000 series representing the higher-tier tournaments. This suggests that players may have a higher probability of winning in higher-ranked tournaments, such as Grand Slam and Masters 1000, compared to lower-ranked tournaments such as ATP250 and International.

>>> Overall, the countplot provides an easy way to visualize the frequency of each series in the dataset, which can be useful in understanding the distribution of the data.

![image](https://user-images.githubusercontent.com/129508864/230340832-085e67d6-0bb3-4789-b219-ac269a37b91d.png)

# Graph #2
>>> Playing Surface: Different tennis surfaces, such as clay, grass, and hard court, can favor different types of players. 
For example, clay court is generally considered to be a slower surface, which can give an advantage to players who are more patient and defensive. 
Grass court, on the other hand, is faster and can favor players who have a big serve and aggressive playing style.

>>> Hard courts are the most common surface in professional tennis. Players who perform well on hard surface,
are more versatile and adaptable.

>>> Clay courts are generally slower and provide more bounce. Players can having a benefit when they comfortable 
with long rallies and with good defensive skills.Good players on clay are more defensive players.
Grass courts are generally faster und provide less bounce. Players can have a benefit with more attacking style of play
and a strong serve-and-volley game. Good players on grass have more agressive style of play
Carpet is the least common surface. The carpet courts are fast and low-bouncing. Players with powerful serves and good footwork 
can benefit on this surface

>>> The plot shows the number of matches played on each court surface. The x-axis represents the different court surfaces, which are Hard, Clay, Grass, and Carpet. The y-axis shows the number of matches played on each surface.

>>> From the plot, we can see that the most number of matches were played on Hard court surface, followed by Clay and Grass surfaces. There were very few matches played on Carpet surface, which is now a rare surface in professional tennis.

>>> This plot provides insight into the popularity of each court surface in professional tennis and can be useful for players and coaches to make strategic decisions based on the surface they are playing on.

![image](https://user-images.githubusercontent.com/129508864/230341854-341b223c-d7db-4af0-8b96-c0fed369a17d.png)

# GRAPH #3
>>> The bar graph shows the win percentage for the top 10 tennis players in the dataset. The win percentage is calculated by dividing the number of matches won by each player by the total number of matches played by the player.

>>> From this, we can see that Djokovic N. and Murray A. have a 100% win percentage, which means that they have won all the matches they have played in the dataset. Federer R. has the third-highest win percentage of 83.62%, followed by Djokovic N. again with a slightly lower percentage of 82.47%.

>>> The next two players, Nadal R. and Federer R. have win percentages of 82.11% and 80%, respectively. Youzhny M., Murray A., Agassi A., and Chiudinelli M. complete the top 10 with win percentages of 80%, 77.24%, 76.03%, and 75%, respectively.

>>> Overall, the top 10 players in the dataset have very high win percentages, indicating that they are highly skilled players who have been successful in the matches they have played.

>>> Note: The reason why some names appear twice in the output is most likely due to the fact that the dataset includes matches where these players played against each other, and they were either listed as the winner or the loser. For example, Djokovic N. appears twice in the output with win percentages of 100% and 82.47%, which means that he has won all matches where he was the winner and has lost some matches where he was the loser. Similarly, Federer R. appears twice with win percentages of 83.62% and 80%, indicating that he has won most matches he has played, but has also lost some.

>>> or It looks like there may be some duplicate player names in the dataset, which is causing the same name to appear twice in the output. For example, "Djokovic N." appears twice in the output with slightly different win percentages. This could be due to different spellings or formatting of the same name in the dataset, or it could be because there are two different players with the same or similar names. Without further information on the dataset, it is difficult to determine the exact cause of the duplicate names.


![image](https://user-images.githubusercontent.com/129508864/230326253-5809b1b8-7862-4db1-a6bf-ec28c88bbd0a.png)

# GRAPH #4
>>> This code generates a figure with six subplots, each of which displays a histogram of a different numerical variable from the dataset. The six variables are:

>>>>>> WRank: The ranking of the winning player
>>>>>> LRank: The ranking of the losing player
>>>>>> Wsets: The number of sets won by the winning player
>>>>>> Lsets: The number of sets won by the losing player
>>>>>> Best of: The format of the match (e.g. best of 3 or best of 5 sets)
>>>>>> proba_elo: The Elo rating-based probability of the winning player winning the match.

>>> The histograms are displayed using the "barstacked" style, which stacks bars on top of each other to show the relative frequencies of different values within each variable.

>>> Overall, this code provides a visual summary of the distribution of each variable in the dataset, which can help to identify patterns and outliers that may be of interest to further investigate.

![image](https://user-images.githubusercontent.com/129508864/230327243-f34bb4aa-9ea9-4dbd-a86f-834a61852026.png)

# GRAPH #5
>>> The scatter plot shows the correlation between the probability of Elo rating (represented by color) and the Elo ratings of the winner and loser. The blue dots represent matches where the loser had a higher Elo rating than the winner, while the red dots represent matches where the winner had a higher Elo rating than the loser.

>>> The scatter plot suggests a correlation between 'proba_elo' and 'elo_ratings'. The red and blue dots seem to be following a general trend upwards, indicating that as the 'proba_elo' score increases, so does the 'elo_ratings' score. This is also supported by the lighter shade of blue and red dots in the middle, which form a line going up. However, there are still a significant number of matches where the lower-rated player wins, as seen by the blue dots in the upper part of the plot.

>>> Overall, it seems that while higher Elo ratings do generally lead to a higher probability of winning, other factors can also play a role in determining the outcome of a match.

![image](https://user-images.githubusercontent.com/129508864/230316862-ffd7aa8c-10ca-40e9-8b0a-e4b839cc1bcc.png)

# GRAPH #6
>>> The bar chart shows the number of matches played by surface and round. The x-axis represents the round of the match, while the y-axis represents the number of matches played. The bars are color-coded according to the surface on which the matches were played. From the chart, it can be seen that the most number of matches were played on hard surfaces, followed by clay and grass. It can also be seen that the number of matches played decreases as the rounds progress, with the highest number of matches played in the 1st round and the lowest number of matches played in the final round.

>>> The decrease in match count from the first to the fourth round of the tournament can be attributed to the single-elimination format, which means that as the competition progresses towards the final, fewer players remain in the running.
In a round-robin system, players compete against each other and the group winner advances to the next stage leading to the final. However, this system is relatively rare and there are only a few tournaments that use it. As a result, the number of matches played in such tournaments is significantly lower.

![image](https://user-images.githubusercontent.com/129508864/230348723-e2e2ab6e-fe8d-4d84-9f3c-d28168aa8a37.png)

# GRAPH #7
>>> Based on the boxplot analysis, we can see that the different tennis tournament series have varying ranges of probability of winning based on their proba_elo scores. The proba_elo scores for each series are represented by the height of the box and whiskers. The line in the middle of the box represents the median value, while the box itself represents the interquartile range (IQR) of the data. The whiskers extend to the most extreme data points that are not considered outliers.

>>> The long dots at the bottom whiskers of the International series suggest that there are several outliers with lower proba_elo scores in this series. Meanwhile, the small boxes for the International and International Gold series suggest that the proba_elo scores for these tournaments are more concentrated within a narrow range. The Grand Slam and Masters 1000 series have the widest range of proba_elo scores, as represented by the length of their boxes and whiskers.

>>> The analysis suggests that players have a higher probability of winning in higher-ranked tournaments, such as Grand Slam and Masters 1000, compared to lower-ranked tournaments such as ATP250 and International, because the box plot shows that the median probability of winning, represented by the line in the middle of the box, is higher for Grand Slam and Masters 1000 than for lower-ranked tournaments.

>>> Additionally, the upper whisker of the box plot, which represents the highest probability of winning within 1.5 times the interquartile range, is also higher for Grand Slam and Masters 1000 than for lower-ranked tournaments. This suggests that the top players have a higher probability of winning in higher-ranked tournaments, which is likely due to the higher level of competition and prize money in those tournaments.

>>> Also, higher-ranked tournaments such as Grand Slam and Masters 1000 are considered more prestigious and offer more ranking points, prize money, and media exposure compared to lower-ranked tournaments such as ATP250 and International. This often results in stronger fields of players and more intense competition, which can lead to a higher level of performance and a greater likelihood of winning for top players. Additionally, players may be more motivated to perform well in higher-ranked tournaments due to the potential rewards and recognition they offer.

>>> On the other hand, higher-ranked tournaments like Grand Slam and Masters 1000 typically attract the top-ranked players in the world. These players have demonstrated higher levels of skill and performance, which could also contribute to their higher probabilities of winning in these tournaments.

![image](https://user-images.githubusercontent.com/129508864/230322376-89c26efc-e828-4ea0-a5fd-5d7285666f77.png)

# --- END of Step 1

# STEP 2
CLEAN the DATASET

NEED TO CONVERT
SPLIT the column for MONTH, DAY, YEAR
Date Type should be INT64 and not OBJECT

MISSING VALUES
Wsets, Lsets, PSW, PSL, B365W, and B365L columns are non-null values but has missing values maybe because some matches may not have had data available for those particular fields.

CATEGORICAL VARIABLES CONVERT TO NUMERICAL VARIABLES
Location, Tournament, Series, and Comment columns are categorical variables.
Possible methods to use: one-hot encoding, label encoding, and target encoding.

ADD NEW COLUMNS
- for players countries
- 3 target variables

METHODS TO CONVERT:
1. One-hot encoding: This method creates new binary columns for each unique category in the original categorical column. For example, if we have a "Location" column with the categories "Adelaide", "Doha", and "Dubai", one-hot encoding would create three new columns: "Location_Adelaide", "Location_Doha", and "Location_Dubai". The value in each new column would be 1 if the corresponding category is present for that row, and 0 otherwise.

2. Label encoding: This method assigns a unique numerical value to each category in the original categorical column. For example, if we have a "Location" column with the categories "Adelaide", "Doha", and "Dubai", label encoding would assign the values 0, 1, and 2 to these categories, respectively. (this is the most fitting)

3. Target encoding: This method replaces each category in the original categorical column with the mean target value for that category. For example, if we have a "Location" column and the target variable is the probability of a team winning a match, target encoding would replace each location with the mean probability of winning for matches played in that location.

TRY TO CHECH IF ATP AND CONFIDENCE DATASETS ARE RELATED
based on the date (which is the common column)

PSW has 27% missing values - that can affect ML model

# Machine Learning Models

# Decision Tree Regression

>>> Model Brief: A type of supervised learning algorithm used for both classification and regression problems. It is used to predict a continuous output variable based on one or more input variables. It tries to establish a relationship between a target variable and a set of predictor variables by constructing a decision tree. A decision tree is a tree-like structure where each internal node represents a test on an attribute, each branch represents an outcome of the test, and each leaf node represents a prediction of the target variable.

In the project, it could be used to predict the probability of a team winning a match based on various input variables. The model would be trained on historical data to learn the relationship between the input variables and the probability of a team winning a match. The trained model could then be used to make predictions on new data to estimate the probability of a team winning a match.

>>> Result of the Modelling

score train :  1.0
score test :  0.766493217097309

Mean Squared Error: 0.05837620219190338
Root Mean Squared Error: 0.24161167643949533
Mean Absolute Error: 0.05837620219190338
R2 Score: 0.766493217097309

>>> Analysis
The model has a score of 1.0 on the training set, which indicates overfitting. It has lower accuracy score of 0.766 on the test set compared to the Decision Tree Classifier. 

The R2 score is 0.766 on the test set, which indicates that the model is performing reasonably well but there is room for improvement. The Mean Squared Error, Root Mean Squared Error, and Mean Absolute Error indicate that the model is making errors in its predictions. The numbers are also high, indicating a poor fit to the data.

This model is not recommended for your project.


# Logistic Regression:

>>> Model Brief: A type of supervised learning algorithm used for binary classification problems. It is used to predict the probability of a binary outcome (0 or 1) based on one or more input variables.

In our project, it could be used to predict the probability of a team winning a match (1) or losing a match (0) based on various input variables. The model would be trained on historical data to learn the relationship between the input variables and the probability of a team winning or losing a match. The trained model could then be used to make predictions on new data to estimate the probability of a team winning or losing a match.

>>> Result of the Modelling

Score on the train set 0.741570206341218
Score on the test set 0.7423395213598748

Prediction	0	1
True		
0	6087	2881
1	1727	7189

precision    recall  f1-score   support

           0       0.78      0.68      0.73      8968
           1       0.71      0.81      0.76      8916

    accuracy                           0.74     17884
   macro avg       0.75      0.74      0.74     17884
weighted avg       0.75      0.74      0.74     17884

>>> Analysis
The model has an accuracy score of 0.741 on the training set and 0.742 on the test set, which indicates that the model is not overfitting. Also means that it can predict the outcome of the match with moderate accuracy.

The precision, recall, and f1-score for both classes are above 0.7, which is also a good indicator of a good performing model.
Based on the classification report, the model performs better in predicting class 1 than class 0, with a higher recall for class. All scores are also moderate for both classes, indicating average performance on predicting wins and losses. This model may be useful as a complement to other models, but may not be sufficient on its own to beat bookmakers' algorithms.


# Linear Regression
>>> Model Brief: A statistical method for modeling the relationship between a dependent variable and one or more independent variables. In the project, the dependent variable is the probability of a team winning a match, and the independent variables are various input variables such as team stats, player stats, bookmakers ratings, etc.

The goal of linear regression is to find the line of best fit that describes the relationship between the dependent variable and the independent variables. The line of best fit is a straight line that minimizes the sum of the squared differences between the actual values of the dependent variable and the predicted values from the independent variables.

>>> Result of the Modelling

MSE on the training set: 4.658812858842604e-26
MSE on the test set: 0.0013319759046108758

Overfitting test

Ridge result:
MSE on the training set: 0.0008325432220229922
MSE on the test set: 0.0020644337291440343

Lasso Result:
MSE on the training set: 0.2355202640351613
MSE on the test set: 0.23583025208025807

>>> Analysis
The model has a very low MSE on the training set, which indicates overfitting.

The MSE on the test set is higher than the training set, which indicates that the model is not performing well on new data.
The model is likely overfitting the training data, and regularization techniques may be needed to improve the model's performance on the test set.

This model is not recommended for your project.

Both models (Ridge and Lasso Regression) have a high MSE on the test set, indicating that they may not fit the data well. These models are not recommended for your project.

# Random Forest
>>> Model Brief: A type of ensemble learning algorithm that uses multiple decision trees to make predictions.

In the project objective, it could be used to estimate the probability of a team winning a match based on various input variables such as team stats, player stats, bookmaker ratings, etc. The model is trained on historical data to learn the relationship between the input variables and the probability of a team winning a match.

>>> Result of the Modelling

Classification Report (Training):
              precision    recall  f1-score   support

           0       1.00      1.00      1.00     35825
           1       1.00      1.00      1.00     35707

    accuracy                           1.00     71532
   macro avg       1.00      1.00      1.00     71532
weighted avg       1.00      1.00      1.00     71532

Classification Report (Test):
              precision    recall  f1-score   support

           0       0.93      0.96      0.94      8883
           1       0.96      0.93      0.94      9001

    accuracy                           0.94     17884
   macro avg       0.94      0.94      0.94     17884
weighted avg       0.94      0.94      0.94     17884

MSE on the training set: 0.004705176704132417
MSE on the test set: 0.031402823753075376

>>> Analysis
The model performs very well on both the training and test sets with an accuracy of 1.00 and 0.94, respectively. The model's precision, recall, and f1-score are also high for both classes (winning and losing teams), indicating that the model is able to correctly predict both outcomes with high confidence.

However, it's important to note that the objective of the project is to beat bookmakers' algorithms on estimating the probability of a team winning a match. While the model's accuracy is high, it's not clear if it is able to outperform the bookmakers' algorithms. Additionally, the Mean Squared Error (MSE) is low for the training set but relatively higher for the test set, which may indicate that the model is overfitting on the training data and may not generalize well to new data.

Overall, while the Random Forest model shows promising results, further analysis and comparison with bookmakers' algorithms would be needed to determine its effectiveness in beating the bookmakers.


# Support Vector Machines:
>>> Model Brief: A type of supervised learning algorithm that can be used for classification or regression problems. In classification, the algorithm tries to find a hyperplane in a high-dimensional space that can best separate the different classes of data. In regression, the algorithm tries to find a function that can fit the data as closely as possible while still having a smooth and regular shape.

SVMs could be used to predict the probability of a team winning a match based on various input variables. The model would be trained on historical data to learn the relationship between the input variables and the probability of a team winning a match. SVMs have been shown to be effective in solving classification problems with high-dimensional data, which is often the case in sports betting where there are many variables to consider.

>>> Result of Modelling

Accuracy score on the training set: 0.9806939551529386
Accuracy score on the test set: 0.9785282934466563

>>> Analysis

Based on the objective of beating bookmakers' algorithms on estimating the probability of a team winning a match, the accuracy scores for the Support Vector Machine model on both the training and test sets are high, indicating that the model is performing well.

However, without additional information on the bookmakers' algorithms and their performance on this specific task, it is difficult to determine whether this model is actually outperforming the bookmakers.

Further analysis and comparison with the bookmakers' algorithms would be necessary to draw any conclusions about the effectiveness of the SVM model in achieving the project's objective.


# Decision Tree Classifier: OUR CHOICE

>>> Model Brief: A type of supervised learning algorithm used for classification problems. It is used to predict the probability of a binary outcome (0 or 1) based on one or more input variables. The goal of classification is to predict a binary outcome, in which the outcome can be one of two classes, for example, whether a team will win or lose a match. The algorithm is called a decision tree because it builds a tree-like model of decisions and their possible consequences.

In our project, it could be used to predict the probability of a team winning a match (1) or losing a match (0) based on various input variables. The model would be trained on historical data to learn the relationship between the input variables and the probability of a team winning or losing a match. The trained model could then be used to make predictions on new data to estimate the probability of a team winning or losing a match.

>>> Result of Modelling

Accuracy: 0.9464325654216059

score train :  1.0
score test :  0.9464325654216059

Prediction	0	1
True		
0	8550	428
1	530	8376

precision    recall  f1-score   support

           0       0.94      0.95      0.95      8978
           1       0.95      0.94      0.95      8906

    accuracy                           0.95     17884
   macro avg       0.95      0.95      0.95     17884
weighted avg       0.95      0.95      0.95     17884

>>> Analysis:
The model has an accuracy score of 0.946 on both the train and test sets, which is a good indicator that the model is not overfitting.

The precision, recall, and f1-score for both classes are above 0.9, which is also a good indicator of a good performing model.
Based on the classification report, the model performs well in predicting both class 0 and class 1, with a slightly higher recall for class 0.

This model is a good candidate for your project.

# Data Analysis

# PCA
The output below the graph shows the actual eigenvalues for the top 5 principal components, as well as their corresponding explained variance ratios. These values give an idea of the importance of each principal component in explaining the variability of the data.

The higher the eigenvalue, the more important the corresponding principal component is in capturing the underlying patterns in the data. In this case, the first principal component has the highest eigenvalue, followed by the second, third, fourth, and fifth.

[0.00200492 0.00190119 0.00178492 0.00161347 0.00157185]
Eigenvalues are: [4.66350113 4.42223503 4.15179269 3.752989   3.65617574]

![image](https://user-images.githubusercontent.com/129508864/235892679-d7a58de9-f426-4ee8-b49a-9d146ccd0a5f.png)

![image](https://user-images.githubusercontent.com/129508864/235892749-19726c41-2c48-412a-aa7b-cfbe78c7fac1.png)

![image](https://user-images.githubusercontent.com/129508864/235892851-22c0fca7-c9c3-4900-a7fe-d258c31d8922.png)

![image](https://user-images.githubusercontent.com/129508864/235892910-7d41b81e-aeb0-4949-8985-0c1e81b325b4.png)

![image](https://user-images.githubusercontent.com/129508864/235893057-5e4d5062-1a41-4735-86ee-01f39cceddf9.png)

# tSNE

# K-means






END
