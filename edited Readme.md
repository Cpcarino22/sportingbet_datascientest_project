# Introduction

# Context

This project seeks to enhance match outcome predictions by surpassing bookmakers' algorithms through the application of data science techniques.

To achieve this, we will utilize a comprehensive dataset containing data on over 44,700 tennis matches played between 2000 and March 2018. This dataset contains information on players, tournaments, surfaces, and outcomes, providing a wealth of data to analyze.

By utilizing tools like Python and Excel, we can effectively clean and organize the data, select important features, and build a model to predict match outcomes. Our ultimate goal is to create a more precise and reliable model than existing bookmakers' algorithms, allowing us to accurately predict the outcome of tennis matches with greater confidence.

Not only will the research provide a valuable contribution to the tennis industry, but it will also have practical applications for businesses, sports bettors, and researchers alike. 

Businesses can use the dataset for market research, trend analysis, and player evaluation, while sports betting companies can leverage the data to develop betting strategies and adjust their odds based on player and tournament performance.

Additionally, researchers can utilize the dataset to study player performance, tournament outcomes, and court surface effects on player performance, potentially leading to the development of new theories and strategies in the sport of tennis.

Overall, the project aims to push the boundaries of match outcome prediction and provide valuable insights to various stakeholders in the tennis industry.

# Objectives
The objective of this project is to try to beat bookmakers' algorithms on estimating the probability of a team winning a match.

The ATP matches dataset provides a wealth of information on men's professional tennis matches played between 2000 and March 2018, making it an essential resource for developing predictive models. By analyzing the data and identifying correlations between factors such as player performance, location, and tournament outcomes, the project seeks to create a more reliable and precise model for predicting match outcomes. Ultimately, this will provide valuable insights and inform decision-making in the tennis industry.

It's important to know the level of expertise each member of the group has in addressing this problem.

Here are some potential issues that need to be checked when working with the ATP matches dataset:

1.Missing values: Some columns have a significant number of missing values, which may require handling depending on the analysis being performed.

2.Outliers: Outliers in the data can affect the results of analysis and should be identified and handled appropriately.

3.Data quality: It's important to check the data for accuracy and reliability, including identifying typos or errors.

4.Data consistency: The data should be consistent across all columns to avoid issues when grouping or analyzing the data.

5.Data integrity: Ensure that the data has not been tampered with or altered in any way.

6.Data format: The data should be in a consistent format across all columns to facilitate analysis, such as standardized date formats.

7.Data relevance: Ensure that the data is relevant to the analysis being performed, such as analyzing data from a specific time period.

# Understanding and manipulation of data

# Framework
The project utilized the ATP matches dataset, which consists of all ATP matches played between 2000 and March 2018. The dataset was downloaded from Kaggle and is freely available for download. It contains 44,708 rows and 23 columns of data. The dataset is paired with another dataset called Confidence Data, which provides PSW numbers.

![Bild1](https://user-images.githubusercontent.com/129981869/236496973-c50d8caf-7351-41cd-af78-ecc41896b310.png)

# Relevance
In order to achieve their objective of beating the bookmaker's algorithms on estimating match outcomes, the researchers conducted an analysis of the columns available in the ATP dataset.


![Bild2](https://user-images.githubusercontent.com/129981869/236497692-71711dcd-10be-4924-8dd3-40204ec9aece.png)

# Feature Variables
Some of the feature variables that could be relevant in a dataset aimed at beating bookmakers' algorithms on estimating the probability of a team winning a match could include:
# Player rankings (WRank,LRank)
.The dataset includes the current and highest ranking of each player. This information could be useful in predicting the outcome of a match, as players with higher rankings may be more likely to win.
# Previous tournament performances (elo_rating)
.The dataset includes information on the previous tournament performances of each player. This information could be useful in predicting the outcome of a match, as players who have performed well in previous tournaments may be more likely to win.

.The ELO rating categorizes players based on their skill level, with Beginner players (below 1400), Novice to Intermediate players (1400-1600), Intermediate to Advanced players (1600-1800), Advanced to Expert players (1800-2000), and Elite players (2000 and above).
# Odds of the bookmakers (B365W/B365L , PSW/PSL)
.Betting odds: This includes the odds offered by bookmakers, such as bet365, and can be used to evaluate the probability of a team winning the match.

.The bet365 odds for the winner of the match can help in predicting the outcome of the match. These odds are based on various factors such as a player's current form, head-to-head records, and other relevant factors, which reflect the perceived probability of a player winning the match.

.If a player has high odds of winning, it means that they are expected to perform well and have a better chance of winning the match. Conversely, if a player has low odds of winning, it means that they are not expected to perform as well and have a lower chance of winning the match.
By combining the bet365 odds with other relevant variables like current form, head-to-head records, and injuries, you can potentially make a more informed prediction of the outcome of the match. However, it's important to keep in mind that these odds are not always 100% accurate and it's always wise to use multiple sources of information and analysis to make an informed decision.

# Target Variable
The researchers created a new column (named target) to label the Win or Loss outcome of a player, with a value of 1 indicating a win and 0 indicating a loss.

![Bild3](https://user-images.githubusercontent.com/129981869/236498243-70c1052e-0e2c-4600-ba29-ee1eaf9159db.png)

# Limitations

The dataset used in the project lacks significant feature variables that could determine a player's probability of winning, such as nationality (for potential home ground advantage), age (related to strength and stamina), height, weight, and right/left-handedness (relevant to strategy). While the available data provides information on location, tournament, date, series, court, surface, round, best of, winner, loser, their respective rankings, and the number of sets won, it may not capture all the factors contributing to a player's success, including physical condition, training regimen, mental state, or opponents' strategies. Therefore, it's important to recognize the limitations of the available data, even though it can provide valuable insights and predictions.

Analyzing tennis matches' winning probability is crucial for time-varying player-specific abilities on different court surfaces. Several extensions, including player-specific explanatory variables and specific configurations for Grand Slam tournaments, should be considered. The estimation results could help construct rankings of players for different court surface types.

# Exploring Relevant Variable Combinations

Based on your objective of beating bookmakers' algorithms on estimating the probability of a team winning a match,
1. Tournament, Surface, and Round
For the combination of Tournament, Surface, and Round, this would show how players perform on different surfaces across different rounds of a tournament. For example, could analyze how the performance of players varies between the early rounds and the later rounds, or how certain players perform better on certain surfaces in different rounds. This could potentially help in predicting which players might have an advantage in certain matchups.
2. Location, Surface, and Round
For the combination of Location, Surface, and Round, this would show how players perform on different surfaces across different locations. For example, could analyze how certain players perform better on grass surfaces in Europe versus grass surfaces in North America, or how players might perform differently on clay surfaces in South America versus clay surfaces in Europe. This could potentially help in predicting which players might have an advantage in certain matchups based on their past performances in similar conditions.
3. Surface, Round, and Best of
For the combination of Surface, Round, and Best of, this could potentially show how players perform under different conditions of a match. Best of determines how many sets are required to win the match, so this could help to understand how players might perform under pressure in a 3-set versus a 5-set match on different surfaces. It could also help to identify which players might have an advantage in shorter or longer matches on certain surfaces.

These combinations can help you identify any trends or patterns that may exist between these variables and the probability of a team winning a match. However, it is important to keep in mind that these variables alone may not provide a complete picture, and you may need to consider other factors such as the players' current form, head-to-head records, and injuries.




# Visualizations and Statistics (Initial)

The project requires the creation of at least 5 graphical representations that are visually relevant and built from the dataset. 
# Frequencies of Series


![Bild4](https://user-images.githubusercontent.com/129981869/236498619-7acd8023-e2e5-42d5-ab6b-a2bd23a34ecc.png)



![Bild5](https://user-images.githubusercontent.com/129981869/236498818-f03bb104-cbd1-4e8e-a337-3434fa13bb59.png)


The graph shows the frequency of each tournament series in the dataset. The dataset contains matches from eight different tournament series, namely International, ATP250, Grand Slam, Masters, Masters 1000, ATP500, International Gold, and Masters Cup. The International series has the highest frequency with 10792 matches, followed by ATP250 with 9550 matches and Grand Slam with 8255 matches. The Masters Cup series has the lowest frequency with only 240 matches.

The graph also provides insights into the distribution of tournaments across different levels of prestige, with the International and ATP250 series representing the lower-tier tournaments and the Grand Slam and Masters 1000 series representing the higher-tier tournaments. This suggests that players may have a higher probability of winning in higher-ranked tournaments, such as Grand Slam and Masters 1000, compared to lower-ranked tournaments such as ATP250 and International.

Overall, the countplot provides an easy way to visualize the frequency of each series in the dataset, which can be useful in understanding the distribution of the data.

# Frequencies of Surfaces



![Bild6](https://user-images.githubusercontent.com/129981869/236499087-13a24dc1-ed74-44e9-b988-b25a2d7a6701.png)



![Bild7](https://user-images.githubusercontent.com/129981869/236499161-e95d8438-ff13-49d3-9dd1-9b15dc574684.png)

Tennis is played on different surfaces, such as clay, grass, hard court, and carpet. Each surface has its unique characteristics that favor different playing styles.

For example, clay is slower and provides more bounce, which benefits defensive players who are patient. Grass, on the other hand, is faster and favors players with an aggressive style of play and a powerful serve.

Hard court is the most common surface in professional tennis, and players who do well on it tend to be adaptable and versatile. Carpet courts are the least common surface and are fast-paced, which benefits players with excellent footwork and powerful serves.

The plot shows that hard courts are the most popular surface, followed by clay and grass courts. Carpet courts have the least number of matches played on them. This plot can help players and coaches make strategic decisions about which surface to play on based on the popularity and unique characteristics of each type of court.

# Win Percentage of Top 10 Players


![Bild8](https://user-images.githubusercontent.com/129981869/236499304-dfff27dd-cd84-45c3-b16e-20f42f6628dd.png)



![Bild9](https://user-images.githubusercontent.com/129981869/236499395-70e5fcfa-63f0-4ebc-9929-3e328e2d8a95.png)


The bar graph displays the win percentage of the top 10 tennis players in the dataset, calculated by dividing the number of matches won by each player by their total number of matches played. The higher the percentage, the better the player's record.

Djokovic N. and Murray A. have a perfect 100% win percentage, meaning they won every match they played in the dataset. Federer R. is close behind with an 83.62% win percentage, followed by Djokovic N. again at 82.47%.

The win percentages for Nadal R., Federer R., Youzhny M., Murray A., Agassi A., and Chiudinelli M. range from 80% to 75%. This indicates that these players are highly skilled and have performed well in their matches.

The dataset may have some repeating names, which is why you see the same name twice with slightly different win percentages. This could happen because of spelling or formatting differences in the dataset, or there could be two different players with similar names. It's hard to know for sure without more information on the dataset.




# Distribution of variables (numbers)

![Bild10](https://user-images.githubusercontent.com/129981869/236499556-1f33ef96-4214-41f2-901b-a49f62a57c5e.png)



![Bild11](https://user-images.githubusercontent.com/129981869/236499657-007b7069-fc89-41f4-b5c1-774382c27f9e.png)

The code above plotted the figure with six subplots, each displaying a histogram of a different type of information from the dataset. The types of information include the rankings of the winning and losing players, the number of sets won by each player, the match format, and the probability of the winning player winning the match based on their Elo rating.

The histograms are displayed in a way that shows the frequency of different values within each variable, with bars stacked on top of each other to create a visual summary of the distribution of each variable in the dataset. This can help to identify any unusual patterns or outliers that may be worth further investigation.

Overall, this code provides a useful way to get a quick overview of the distribution of different variables in the dataset, and can help researchers to identify areas of interest for further analysis.



# Correlation  of Elo-rating and probability of winning


![Bild12](https://user-images.githubusercontent.com/129981869/236499802-c0b4a743-d332-4e88-b2b4-b853dbdcb0f2.png)

The scatter plot displays the relationship between the probability of Elo rating (represented by color) and the Elo ratings of the winner and loser. The blue dots represent matches where the loser had a higher Elo rating than the winner, while the red dots represent matches where the winner had a higher Elo rating than the loser.

The scatter plot suggests that there is a positive correlation between 'proba_elo' and 'elo_ratings'. The trend line formed by the lighter shade of blue and red dots indicates that as the 'proba_elo' score increases, so does the 'elo_ratings' score. However, there are still a significant number of matches where the lower-rated player wins, as seen by the blue dots in the upper part of the plot.

Overall, this suggests that while higher Elo ratings tend to correspond with a higher probability of winning, there are other factors at play in determining the outcome of a match.
# Matches played on Surface and Rounds


![Bild13](https://user-images.githubusercontent.com/129981869/236499945-c039f146-3e44-4128-b049-461eef70da67.png)




![Bild14](https://user-images.githubusercontent.com/129981869/236500071-2800f41f-5e4f-4b3e-9ac4-878b4d01b693.png)


The bar chart visualizes the number of matches played by surface and round, providing insights into the distribution of tennis matches across different surfaces and tournament stages. The x-axis represents the round of the match, while the y-axis represents the total number of matches played. The bars are color-coded according to the surface on which the matches were played.

The chart highlights that hard surfaces, such as hard courts and asphalt, are the most popular playing surface for ATP tournaments, followed by clay and grass. This could be due to various reasons, including the availability of facilities, player preferences, and climatic conditions. Moreover, the number of matches played decreases as the tournament progresses, with the highest number of matches played in the 1st round and the lowest number of matches played in the final round.

The decrease in the number of matches played from the first to the final round can be attributed to the single-elimination format of the ATP tournaments. In this format, players who lose a match are eliminated from the tournament, while the winners advance to the next round. Therefore, as the competition progresses, fewer players remain in the running, resulting in a lower number of matches played.

It is worth noting that a round-robin system, in which players compete against each other in a group, is relatively rare in ATP tournaments. In this system, the group winner advances to the next stage, leading to the final. As a result, the number of matches played in such tournaments is significantly lower.




# Probability of Elo rating by Series

![Bild15](https://user-images.githubusercontent.com/129981869/236500194-f48288fa-d99d-42a9-bd8c-ccaea33f8830.png)



![Bild16](https://user-images.githubusercontent.com/129981869/236500522-a42db482-0f64-403b-8a0e-846f634dc8f5.png)

Based on the analysis of the boxplot, it is evident that the probability of winning varies among the different tennis tournament series based on their proba_elo scores. The height of the box and whiskers represents the proba_elo scores for each series, with the median value depicted by the line in the middle of the box, while the box itself represents the interquartile range (IQR) of the data. The whiskers extend to the most extreme data points that are not considered outliers.

The International series has several outliers with lower proba_elo scores, as indicated by the long dots at the bottom whiskers. Conversely, the International and International Gold series have more concentrated proba_elo scores, represented by their small boxes. The Grand Slam and Masters 1000 series have the widest range of proba_elo scores, as reflected by the length of their boxes and whiskers.

The analysis indicates that players have a higher probability of winning in higher-ranked tournaments, such as Grand Slam and Masters 1000, compared to lower-ranked tournaments such as ATP250 and International. This is because the box plot shows that the median probability of winning is higher for Grand Slam and Masters 1000 than for lower-ranked tournaments.

Additionally, the upper whisker of the box plot, which represents the highest probability of winning within 1.5 times the interquartile range, is also higher for Grand Slam and Masters 1000 than for lower-ranked tournaments. This implies that the top players have a higher probability of winning in higher-ranked tournaments, likely due to the higher level of competition and prize money in those tournaments.

Moreover, higher-ranked tournaments such as Grand Slam and Masters 1000 are considered more prestigious, offer more ranking points, prize money, and media exposure compared to lower-ranked tournaments such as ATP250 and International. These factors often result in stronger fields of players and more intense competition, leading to a higher level of performance and a greater likelihood of winning for top players. Additionally, players may be more motivated to perform well in higher-ranked tournaments due to the potential rewards and recognition they offer.

On the other hand, higher-ranked tournaments like Grand Slam and Masters 1000 typically attract the top-ranked players in the world, who have demonstrated higher levels of skill and performance. This could also contribute to their higher probabilities of winning in these tournaments.

# Pre-processing and feature engineering
There are several reasons why cleaning data before machine learning modeling is crucial. Firstly, it improves accuracy by ensuring that the models are more precise. If the data is noisy, inconsistent, or contains errors, the machine learning algorithm may not recognize the patterns or relationships in the data, leading to inaccurate predictions.

Secondly, cleaning data enhances interpretability. When data is clean, it becomes easier to interpret and comprehend the results of the machine learning model. This is because the model is based on reliable and consistent data, which helps to explain the connections between the input variables and the output variable.

Lastly, cleaning data can help reduce computation time. The machine learning algorithm doesn't have to process irrelevant or incorrect data, resulting in faster computation. By eliminating unnecessary data, the algorithm can focus on analyzing the relevant data and improve its performance.

Overall, data cleaning is widely recognized as a critical step in the machine learning pipeline, with the potential to significantly impact the accuracy and effectiveness of the resulting model. As such, it is imperative that data cleaning is performed diligently and with care.

Before   				 



![Bild17](https://user-images.githubusercontent.com/129981869/236504985-be7c066a-829c-4515-8840-76a5cd540d78.png)


After




![Bild18](https://user-images.githubusercontent.com/129981869/236505074-dbfd201e-30aa-4537-8fa7-01a38c93cc31.png)

The images above illustrate the dataset before and after it was cleaned. A detailed discussion of the dataset cleaning process follows.


# Split

A verification process was conducted to ensure the accuracy of the date format which was in YYYY-MM-DD. The team visually checked the dates using excel and Python to interpret the data correctly.

To enhance the data analysis, a treatment process was also performed. The original date variable was converted into three separate variables representing year, month, and day. The team used the dateline library to perform this feature engineering, which can help in better understanding the data or building predictive models.

While splitting the date into year, month, and day may not be directly relevant to estimating the probability of a team winning a match, it can be useful in analyzing whether the time of year or day of the week affects the outcome of a match or whether the performance of a team changes over time.




![Bild19](https://user-images.githubusercontent.com/129981869/236505200-1ad2740f-61cd-4afe-9c55-6814322452b7.png)

# Outliers
To ensure accurate analysis, it is important to identify and handle any outliers in the data. This process can involve either removing the outliers or treating them as a separate category, depending on the situation




![Bild20](https://user-images.githubusercontent.com/129981869/236505299-1f57ff54-6ae2-4a6f-9dc4-a572ce4f47b0.png)




![Bild21](https://user-images.githubusercontent.com/129981869/236505407-a1b0bbad-07d7-4be3-8507-2c92732e28aa.png)



![Bild22](https://user-images.githubusercontent.com/129981869/236505515-b7959fd5-d255-4a93-84b6-817746292d80.png)


First, the verification process for PSW, PSL, B365W, and B365L involved using box plots and scatter plots. After visual inspection of the data, the extreme values and outliers were retained rather than removed.

The reason for retaining these values is that they represent the bookmaker odds for tennis players. It is possible that the extreme values observed for these columns could be due to factors such as player injuries, changes in weather or court conditions, or shifts in public perception or betting trends. Bookmakers use a variety of methods to set odds for sporting events, and the values observed may reflect the bookmaker's assessment of the relative chances of each player winning, which can be influenced by a range of factors.

It is important to carefully consider the context and specific circumstances of the data when interpreting extreme or unusual values. In the case of bookmaker odds, these values may be valid and important indicators of the relative chances of different players winning, even if they seem extreme or unusual at first glance.

The treatment of outliers and extreme values has been completed, and the analysis will now proceed with imputing missing values.

# Missing Values
To identify missing values in the ATP dataset, the researchers employed the isnull method within a Jupyter notebook. The resulting image provides a visual representation of the percentage of missing values in the dataset, enabling the researchers to quickly identify areas that require imputation. This step is crucial in ensuring that the data is complete and accurate before any analysis is conducted, as missing values can skew results and lead to incorrect conclusions. By using the isnull method and creating a visual representation of the missing values, the researchers are able to efficiently and effectively address any gaps in the dataset and proceed with subsequent analyses.




![Bild23](https://user-images.githubusercontent.com/129981869/236505639-ecb338d1-6847-4ef2-ac1c-ed9a0a649d18.png)

The researchers checked and interpreted the PSW and PSL values using Microsoft Excel. These values represent the odds offered by Pinnacle Sports for a player winning or losing a match, respectively.

For instance, a PSW value of 46 implies that the odds offered by Pinnacle Sports for that player winning the match are 46:1, indicating that the player is viewed as a significant underdog. Similarly, a PSL value of 121 indicates that the odds offered by Pinnacle Sports for a player losing the match are 1:121, suggesting that the player is considered a strong favorite to win.




![Bild24](https://user-images.githubusercontent.com/129981869/236505943-7c994b7f-0095-4ee6-bb67-a2da06467db1.png)


The distribution of PSW values was analyzed using the histograph above, which revealed a highly skewed distribution with a long right tail of high values. The majority of values were found to be concentrated in the lower PSW range of 2-4, while a few extreme values were observed to be much higher. To further analyze the distribution, the researchers used skewness and kurtosis measures.

The Skewness and kurtosis measures (below) were utilized to assess the distribution of the odds for winning and losing. Positive skewness values indicate a long right tail, while negative values indicate a long left tail. Both Skewness PSW and Skewness PSL were positive, indicating that the distributions are skewed to the right, with some high values far from the mean. Kurtosis, on the other hand, measures the peakedness of the distribution, with higher values indicating more extreme values, both high and low. In this case, both Kurtosis PSW and Kurtosis PSL were high, indicating that the distributions of the odds for winning and losing were more peaked than a normal distribution.



![Bild25](https://user-images.githubusercontent.com/129981869/236506018-e4896a6c-fa43-443b-9e6b-6d7c26522c02.png)


The histograms below for the 'B365W' and 'B365L' columns show similar distributions and the presence of outliers as the 'PSW' and 'PSL' columns. Thus, the same approach for imputing missing values will be used. The distribution is right-skewed with a long tail and the presence of outliers. Therefore, median imputation would be a better choice than mean imputation.
    


![Bild26](https://user-images.githubusercontent.com/129981869/236506097-f3e41779-eaec-4baa-a7d1-8ce93d5c5355.png)




![Bild27](https://user-images.githubusercontent.com/129981869/236506180-d1b02f47-6deb-4181-9f42-90b6c02f8daa.png)

The researchers found that the skewness values for both B365W and B365L are positive, indicating that the distributions are skewed to the right, with more extreme values on the right side of the distribution. Furthermore, the kurtosis values for both B365W and B365L are greater than 3, suggesting that the distributions are more peaked than the normal distribution, indicating the presence of more outliers.

Additionally, they found that the kurtosis value for B365W is greater than that of B365L, suggesting that the distribution of B365W is more peaked (has more outliers) than the distribution of B365L.



![Bild28](https://user-images.githubusercontent.com/129981869/236506282-62a8f8f9-249c-4d49-be10-b7c1dabbce28.png)

Imputing missing values is a crucial step in data analysis to avoid bias in statistical inference. After analyzing the Excel sheets, histograms, and skewness/kurtosis measures, researchers recommend using median imputation to handle missing values in the 'PSW', 'PSL', B365W, and B365L columns. The data shows a right-skewed distribution with a long tail and several outliers, making median imputation a more robust measure of central tendency than mean imputation. Median imputation is less sensitive to extreme values and outliers, making it a suitable method for filling in missing data.


![Bild29](https://user-images.githubusercontent.com/129981869/236506545-3762de9c-cb80-446f-b56b-047df12f322f.png)


Imputing missing values is a crucial step in data analysis to avoid bias in statistical inference. After analyzing the Excel sheets, histograms, and skewness/kurtosis measures, researchers recommend using median imputation to handle missing values in the 'PSW', 'PSL', B365W, and B365L columns. The data shows a right-skewed distribution with a long tail and several outliers, making median imputation a more robust measure of central tendency than mean imputation. Median imputation is less sensitive to extreme values and outliers, making it a suitable method for filling in missing data.




![Bild30](https://user-images.githubusercontent.com/129981869/236506634-6120117f-cb72-4cf2-a240-bbf896994279.png)


The researchers used the same process for evaluating the missing values in Wsets and Lsets as they did for PSW, PSL, B365W, and B365L. The first step was to use the value count method to obtain an understanding of the distribution of values in a column of the dataset.




![Bild31](https://user-images.githubusercontent.com/129981869/236506708-e5a0a863-93d9-44ee-a4a3-e6cf8beb72ed.png)

Skewness is a statistical measure that indicates the degree of symmetry of a distribution. A skewness score of zero indicates that the distribution is perfectly symmetrical, while a positive skewness score indicates that the distribution is skewed to the right, with a tail extending to the right of the peak. On the other hand, a negative skewness score indicates that the distribution is skewed to the left, with a tail extending to the left of the peak.

In this case, the skewness score for Wsets is -0.023765413101382634, which indicates that the distribution is almost symmetric or has a slight left skew. On the other hand, the skewness score for Lsets is 0.9750401902167463, which indicates a strong right skew, with more values on the right side of the distribution. The histograms would also visually show the distribution of values and how they are skewed to the right or left.

![Bild32](https://user-images.githubusercontent.com/129981869/236506816-1ddced14-3919-4f14-bb88-47ee0925eeb0.png)



![Bild33](https://user-images.githubusercontent.com/129981869/236506898-c42016c5-93b6-4df7-b162-221046d38bfa.png)




![Bild34](https://user-images.githubusercontent.com/129981869/236506952-9047a427-778d-4dbc-ae92-ddab65326319.png)

Based on the skewness scores and histograms, it is recommended to use different imputation methods for Wsets and Lsets. For Wsets, since the distribution is almost symmetrical or has a slight left skew, a reasonable imputation method would be to use the mean or median value to fill in the missing values. However, based on the calculated mean, median, and mode values, the median value of 2.0 is recommended to fill in the missing values of Wsets.

On the other hand, for Lsets, the strong right skewness of the distribution suggests that using the mean or median value may not be the best approach. Instead, other imputation methods such as regression imputation or hot-deck imputation may be more appropriate to fill in the missing values. The choice of imputation method should be based on the specific characteristics of the dataset and the research question at hand, and it may be helpful to compare the results obtained using different imputation methods to assess their impact on subsequent analyses




![Bild35](https://user-images.githubusercontent.com/129981869/236507103-1a3cea32-b5ff-40c1-a556-e8c9d8a79334.png)


During the imputation process, new columns were created for the filled columns, and the original ones were dropped to avoid duplicates. Once the imputation process was completed, the researchers verified its effectiveness by using the isnull method. This step was crucial in ensuring that all missing values were successfully filled in and that the dataset was complete and ready for further analysis.




![Bild36](https://user-images.githubusercontent.com/129981869/236507173-4669780a-13ea-4921-b32d-5e06d46a2469.png)



After completing the imputation process and verifying that all missing values were filled in, the researchers created a heatmap to visualize the correlation among the columns in the dataset.

The heatmap provides a visual representation of the correlation matrix between the columns in the dataset. The correlation coefficient ranges from -1 to 1, where a value of 1 indicates a perfect positive correlation, a value of -1 indicates a perfect negative correlation, and a value of 0 indicates no correlation.

Based on the heatmap, we can see that there is a relatively strong positive correlation (0.82) between Best of and Wsets, which suggests that these two variables are related and may have a significant impact on each other.

We also see a moderate positive correlation (0.66) between elo_winner and proba_elo, which indicates that these variables are somewhat related but may not have a strong impact on each other.

Furthermore, we can see a strong positive correlation (0.9) between psw_filled and B365W_filled, which suggests that these variables are highly related and may have a significant impact on each other. Similarly, we can see a strong positive correlation (0.84) between PSL_filled and B365L_filled, indicating a high level of association between these variables.

Overall, the heatmap provides valuable information about the correlation between the variables in the dataset, which can be useful in identifying patterns and relationships and for further analysis.




![Bild37](https://user-images.githubusercontent.com/129981869/236507332-eebeac31-e30b-4a6b-ba93-513b6a098ce6.png)

# Duplicates
The researchers utilized the duplicated method to detect any duplicate rows in the dataset.




![Bild38](https://user-images.githubusercontent.com/129981869/236507411-27bc3a47-b374-43be-911f-8828b27799a0.png)


The resulting output revealed that there are no duplicate rows in the DataFrame. The first line of the output displays that the DataFrame is empty, signifying the absence of rows in the DataFrame. This finding implies that every row in the initial DataFrame is distinct, and there are no exact duplicates.




![Bild39](https://user-images.githubusercontent.com/129981869/236507526-6ecd000b-5e0f-4b51-80fe-db5c2ba9d1ec.png)

# Misspelled Names
The dataset underwent a visual check of the names by the researchers using Microsoft Excel, revealing various issues such as misspelled names, incorrect initials, missing spaces between initials, and extra spaces before and after names.






![Bild40](https://user-images.githubusercontent.com/129981869/236507619-4243cb5e-84e6-48fe-aa49-2ddd9721d613.png)

To address these issues, the researchers utilized the strip() method to remove trailing spaces in the strings of all columns in Winner and Loser. They also defined the strip_string() function to eliminate any whitespace characters from the beginning and end of a string.




![Bild41](https://user-images.githubusercontent.com/129981869/236508593-4e1dd660-bd1a-4652-ac4d-c998f082a634.png)

Subsequently, a dictionary was created, and the researchers used the replace() method to correct the misspelled names and initials. For instance, the misspelled name 'Nadal-Parera R.' was corrected to 'Nadal R.' in the dataset.


![Bild42](https://user-images.githubusercontent.com/129981869/236508867-75dde0e4-888c-4f6d-a614-959cc863db52.png)
After performing the data cleaning process, the researchers were left with 844 unique Winner names and 1297 unique Loser names from the initial 899 and 1400 unique names, respectively.


![Bild43](https://user-images.githubusercontent.com/129981869/236508949-733612aa-290a-430e-912f-354357dd4884.png)

The researchers created a bar graph to visually compare the top players in the dataset before and after the cleaning process. The graph clearly showed the impact of the cleaning process, as the number of unique players decreased from 1400 to 1297 for the losers and from 899 to 844 for the winners. This reduction in the number of unique names indicates that many of the previously identified "unique" names were actually misspelled or duplicates.

By using the strip() method to remove trailing spaces and the replace() method to correct misspelled names and initials, the researchers were able to identify the correct and unique names of players. This ensures that the dataset is more accurate and precise, and will lead to more reliable results in any future analyses.


![Bild44](https://user-images.githubusercontent.com/129981869/236509032-15a9eb17-59db-4186-a657-6a51f47aae36.png)

![Bild45](https://user-images.githubusercontent.com/129981869/236509106-6a8c65a8-053e-49e9-9f86-8c50321cfac6.png)


![Bild46](https://user-images.githubusercontent.com/129981869/236509219-8882d3c0-2f65-448e-8f49-49c6e7f089a6.png)

# Data Transformation
# Preprocessing
Technics:
1. ATP: OneHotEncoder with dummies
2.Location: OneHotEncoder with dummies
3.Tournament: OneHotEncoder with dummies
4.Date: Already splitted to Year and Month
5.Series: OneHotEncoder
6.Court: replace({'Outdoor': 0, 'Indoor': 1})
7.Surface: OneHotEncoding "Surface_Carpet", "Surface_Clay", "Surface_Grass", and "Surface_Hard",
8.Round: Round Robin': 0, '1st Round': 1, '2nd Round': 2, '3rd Round': 3, '4th Round': 4, 'Quarterfinals': 5, 'Semifinals': 6, 'The Final': 7
9.Best of: retain as it is as actual numbers represent the Best of
10.Winner and Loser: One hot Encoding with Dummies
11.WRank and LRank: grouped with Winner and Loser
12.Comment: replace({'Completed': 1, 'Retired': 0, 'Walkover': 0, 'Disqualified': 0})
13.elo_winner, elo_loser, and proba_elo: num already
14.Year and Month: result of the Date split
15.B365W_filled and B365L_filled: num already





# Assessment methods:  
Reconstituted professional situation: from a set of company data, the candidate must implement various pre-processing and data augmentation to make them usable through machine learning techniques.



# Report 2
# Machine Learning Models
# Decision Tree Regression
# Model Brief: 
A type of supervised learning algorithm used for both classification and regression problems. It is used to predict a continuous output variable based on one or more input variables. It tries to establish a relationship between a target variable and a set of predictor variables by constructing a decision tree. A decision tree is a tree-like structure where each internal node represents a test on an attribute, each branch represents an outcome of the test, and each leaf node represents a prediction of the target variable.

In the project, it could be used to predict the probability of a team winning a match based on various input variables. The model would be trained on historical data to learn the relationship between the input variables and the probability of a team winning a match. The trained model could then be used to make predictions on new data to estimate the probability of a team winning a match.
# Result of the Modelling
score train : 1.0 
score test : 0.766493217097309
Mean Squared Error: 0.05837620219190338 Root Mean Squared Error: 0.24161167643949533 Mean Absolute Error: 0.05837620219190338 R2 Score: 0.766493217097309
# Analysis 
The model has a score of 1.0 on the training set, which indicates overfitting. It has lower accuracy score of 0.766 on the test set compared to the Decision Tree Classifier.

The R2 score is 0.766 on the test set, which indicates that the model is performing reasonably well but there is room for improvement. The Mean Squared Error, Root Mean Squared Error, and Mean Absolute Error indicate that the model is making errors in its predictions. 
The numbers are also high, indicating a poor fit to the data.

This model is not recommended for your project.

# Linear Regression
# Model Brief: 
A statistical method for modeling the relationship between a dependent variable and one or more independent variables. In the project, the dependent variable is the probability of a team winning a match, and the independent variables are various input variables such as team stats, player stats, bookmakers ratings, etc.

The goal of linear regression is to find the line of best fit that describes the relationship between the dependent variable and the independent variables. The line of best fit is a straight line that minimizes the sum of the squared differences between the actual values of the dependent variable and the predicted values from the independent variables.
# Result of the Modelling
MSE on the training set: 4.658812858842604e-26 MSE on the test set: 0.0013319759046108758
# Overfitting test
Ridge result: MSE on the training set: 0.0008325432220229922 MSE on the test set: 0.0020644337291440343
Lasso Result: MSE on the training set: 0.2355202640351613 MSE on the test set: 0.23583025208025807
Analysis The model has a very low MSE on the training set, which indicates overfitting.
The MSE on the test set is higher than the training set, which indicates that the model is not performing well on new data. The model is likely overfitting the training data, and regularization techniques may be needed to improve the model's performance on the test set.

# This model is not recommended for your project.
Both models (Ridge and Lasso Regression) have a high MSE on the test set, indicating that they may not fit the data well. These models are not recommended for your project.

# Random Forest
# Model Brief: 
A type of ensemble learning algorithm that uses multiple decision trees to make predictions.

In the project objective, it could be used to estimate the probability of a team winning a match based on various input variables such as team stats, player stats, bookmaker ratings, etc. The model is trained on historical data to learn the relationship between the input variables and the probability of a team winning a match.
# Result of the Modelling
Classification Report (Training): precision recall f1-score support
      0       1.00      1.00      1.00     35825
       1       1.00      1.00      1.00     35707

accuracy                           1.00     71532


macro avg 1.00 1.00 1.00 71532 weighted avg 1.00 1.00 1.00 71532
Classification Report (Test): precision recall f1-score support
      0       0.93      0.96      0.94      8883
       1       0.96      0.93      0.94      9001

accuracy                           0.94     17884


macro avg 0.94 0.94 0.94 17884 weighted avg 0.94 0.94 0.94 17884
MSE on the training set: 0.004705176704132417 MSE on the test set: 0.031402823753075376
# Analysis 
The model performs very well on both the training and test sets with an accuracy of 1.00 and 0.94, respectively. The model's precision, recall, and f1-score are also high for both classes (winning and losing teams), indicating that the model is able to correctly predict both outcomes with high confidence.
However, it's important to note that the objective of the project is to beat bookmakers' algorithms on estimating the probability of a team winning a match. While the model's accuracy is high, it's not clear if it is able to outperform the bookmakers' algorithms. Additionally, the Mean Squared Error (MSE) is low for the training set but relatively higher for the test set, which may indicate that the model is overfitting on the training data and may not generalize well to new data.
Overall, while the Random Forest model shows promising results, further analysis and comparison with bookmakers' algorithms would be needed to determine its effectiveness in beating the bookmakers.
# Support Vector Machines:
# Model Brief: 
A type of supervised learning algorithm that can be used for classification or regression problems. In classification, the algorithm tries to find a hyperplane in a high-dimensional space that can best separate the different classes of data. In regression, the algorithm tries to find a function that can fit the data as closely as possible while still having a smooth and regular shape.

SVMs could be used to predict the probability of a team winning a match based on various input variables. The model would be trained on historical data to learn the relationship between the input variables and the probability of a team winning a match. SVMs have been shown to be effective in solving classification problems with high-dimensional data, which is often the case in sports betting where there are many variables to consider.
# Result of Modelling
Accuracy score on the training set: 0.9806939551529386 Accuracy score on the test set: 0.9785282934466563
# Analysis
Based on the objective of beating bookmakers' algorithms on estimating the probability of a team winning a match, the accuracy scores for the Support Vector Machine model on both the training and test sets are high, indicating that the model is performing well.
However, without additional information on the bookmakers' algorithms and their performance on this specific task, it is difficult to determine whether this model is actually outperforming the bookmakers.
Further analysis and comparison with the bookmakers' algorithms would be necessary to draw any conclusions about the effectiveness of the SVM model in achieving the project's objective.

# Decision Tree Classifier: OUR CHOICE
# Model Brief: 
A type of supervised learning algorithm used for classification problems. It is used to predict the probability of a binary outcome (0 or 1) based on one or more input variables. The goal of classification is to predict a binary outcome, in which the outcome can be one of two classes, for example, whether a team will win or lose a match. The algorithm is called a decision tree because it builds a tree-like model of decisions and their possible consequences.

In our project, it could be used to predict the probability of a team winning a match (1) or losing a match (0) based on various input variables. The model would be trained on historical data to learn the relationship between the input variables and the probability of a team winning or losing a match. The trained model could then be used to make predictions on new data to estimate the probability of a team winning or losing a match.

# Result of Modelling
Accuracy: 0.9464325654216059
score train : 1.0 score test : 0.9464325654216059
Prediction 0 1 True 0 8550 428 1 530 8376
precision recall f1-score support
      0       0.94      0.95      0.95      8978
       1       0.95      0.94      0.95      8906

accuracy                           0.95     17884


macro avg 0.95 0.95 0.95 17884 weighted avg 0.95 0.95 0.95 17884
# Analysis: 
The model has an accuracy score of 0.946 on both the train and test sets, which is a good indicator that the model is not overfitting.

The precision, recall, and f1-score for both classes are above 0.9, which is also a good indicator of a good performing model. Based on the classification report, the model performs well in predicting both class 0 and class 1, with a slightly higher recall for class 0.



# Logistic Regression:
# Model Brief: 
A type of supervised learning algorithm used for binary classification problems. It is used to predict the probability of a binary outcome (0 or 1) based on one or more input variables.
In our project, it could be used to predict the probability of a team winning a match (1) or losing a match (0) based on various input variables. The model would be trained on historical data to learn the relationship between the input variables and the probability of a team winning or losing a match. The trained model could then be used to make predictions on new data to estimate the probability of a team winning or losing a match.
# Result of the Modelling
Score on the train set 0.741570206341218 
Score on the test set 0.7423395213598748

Prediction	0	1
True		
0	6561	2359
1	1999	6965
             precision    recall  f1-score   support

           0       0.77      0.74      0.75      8920
           1       0.75      0.78      0.76      8964

    accuracy                           0.76     17884
   macro avg       0.76      0.76      0.76     17884
weighted avg       0.76      0.76      0.76     17884

accuracy                           0.74     17884


macro avg 0.75 0.74 0.74 17884 weighted avg 0.75 0.74 0.74 17884
# Analysis:
The model has an accuracy score of 0.741 on the training set and 0.742 on the test set, which indicates that the model is not overfitting. Also means that it can predict the outcome of the match with moderate accuracy.

The precision, recall, and f1-score for both classes are above 0.7, which is also a good indicator of a good performing model. Based on the classification report, the model performs better in predicting class 1 than class 0, with a higher recall for class. All scores are also moderate for both classes, indicating average performance on predicting wins and losses. This model may be useful as a complement to other models, but may not be sufficient on its own to beat bookmakers' algorithms.





# Data Analysis
# PCA
The output below the graph shows the actual eigenvalues for the top 5 principal components, as well as their corresponding explained variance ratios. These values give an idea of the importance of each principal component in explaining the variability of the data.
The higher the eigenvalue, the more important the corresponding principal component is in capturing the underlying patterns in the data. In this case, the first principal component has the highest eigenvalue, followed by the second, third, fourth, and fifth.
[0.00200492 0.00190119 0.00178492 0.00161347 0.00157185] Eigenvalues are: [4.66350113 4.42223503 4.15179269 3.752989 3.65617574]




![Bild47](https://user-images.githubusercontent.com/129981869/236512348-415319bb-5e75-4147-a336-0d6e32445ef9.png)





![Bild48](https://user-images.githubusercontent.com/129981869/236512405-92b7d860-8ae7-45fd-99ed-dc7f861a3612.png)




![Bild49](https://user-images.githubusercontent.com/129981869/236512494-ea50611c-0b23-49a1-88fe-e99572b2dd98.png)





![Bild50](https://user-images.githubusercontent.com/129981869/236512550-709f38ee-9250-4483-bf2f-99a3b1ed58e7.png)




![Bild51](https://user-images.githubusercontent.com/129981869/236512628-bff7b8c5-a287-4275-88e7-d5769a338bd3.png)

# tSNE
# K-means

# Stages of the project
# Classification of the problem 
What kind of machine learning problem is your project like? (classification, regression, clustering, etc)
What task does your project relate to? (fraud detection, facial recognition, sentiment analysis, etc)?
What is the main performance metric used to compare your models? Why this one?
Did you use other qualitative or quantitative performance metrics? If yes, detail it.
# Model choice and optimization
What algorithms have you tried?
Describe which one(s) you selected and why?
Did you use parameter optimization techniques such as Grid Search and Cross Validation?
Have you tested advanced models? Bagging, Boosting, Deep Learning… Why?  
# Interpretation of results
Have you analyzed the errors in your model? 
Did this contribute to his improvement? If yes, describe.
Have you used interpretability techniques such as SHAP, LIME, Skater… (Grad-CAM for Deep Learning…)
What has (or not) generated a significant improvement in your performance? 


# Assessment methods: 
Professional scenario: based on a proposed solution, the candidate will have to produce a summary report including: the explanation of the choices of AI solutions implemented, the interpretation of the results, the evaluation of the reliability of the algorithms and an optimization proposal.







# Final report : 
Conclusion drawn
Difficulties encountered during the project
What was the main scientific obstacle encountered during this project?
For each of the following points, if you encountered difficulties, detail how they slowed you down in setting up your project.
Forecast: tasks that took longer than expected, etc.
Datasets: acquisition, volumetry, processing, aggregation, etc.
Technical/theoretical skills: timing of skill acquisition, skill not offered in training, etc.
Relevance: of the approach, model, data, etc.
IT: storage power, computational power, etc. 
Other
# Report
Detail what was your main contribution to achieving the project's goals.
Have you changed the model since the last iteration? If yes, provide details.
Present the results obtained and compare them to the benchmark
For each of the project's goals, detail how they were achieved or not.
If they have been reached, in which process(es) can your model fit? Detail.

# Continuation of the project

What avenues for improvement do you suggest to increase the performance of your model?
How has your project contributed to an increase in scientific knowledge?
# Bibliography
What bibliographical elements (research articles, blog, books, etc.) did you rely on to carry out your project?

OTHER STUDIES
The time varying player-specific abilities for different court surfaces are of key importance for analyzing tennis matches.
Consider several other extensions including player-specific explanatory variables and the accountance of specific configurations for Grand Slam tournaments. The estimation results can be used to construct rankings of players for different court surface types.

REFERENCE TO REVIEW:
https://www.econstor.eu/bitstream/10419/177699/1/18009.pdf
TITLE: The analysis and forecasting of ATP tennis matches using a high-dimensional dynamic model

# Appendices 
Gantt diagram.
Description of code files.

