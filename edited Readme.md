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

.By combining the bet365 odds with other relevant variables like current form, head-to-head records, and injuries, you can potentially make a more informed prediction of the outcome of the match. However, it's important to keep in mind that these odds are not always 100% accurate and it's always wise to use multiple sources of information and analysis to make an informed decision.

# Target Variable
The researchers created a new column (named target) to label the Win or Loss outcome of a player, with a value of 1 indicating a win and 0 indicating a loss.

![Bild3](https://user-images.githubusercontent.com/129981869/236498243-70c1052e-0e2c-4600-ba29-ee1eaf9159db.png)

# Limitations

The dataset used in the project lacks significant feature variables that could determine a player's probability of winning, such as nationality (for potential home ground advantage), age (related to strength and stamina), height, weight, and right/left-handedness (relevant to strategy). While the available data provides information on location, tournament, date, series, court, surface, round, best of, winner, loser, their respective rankings, and the number of sets won, it may not capture all the factors contributing to a player's success, including physical condition, training regimen, mental state, or opponents' strategies. Therefore, it's important to recognize the limitations of the available data, even though it can provide valuable insights and predictions.

Analyzing tennis matches' winning probability is crucial for time-varying player-specific abilities on different court surfaces. Several extensions, including player-specific explanatory variables and specific configurations for Grand Slam tournaments, should be considered. The estimation results could help construct rankings of players for different court surface types.

# Exploring Relevant Variable Combinations

Based on your objective of beating bookmakers' algorithms on estimating the probability of a team winning a match.
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

![Bild17](https://user-images.githubusercontent.com/129981869/236504985-be7c066a-829c-4515-8840-76a5cd540d78.png)![Bild18](https://user-images.githubusercontent.com/129981869/236505074-dbfd201e-30aa-4537-8fa7-01a38c93cc31.png)

The images above illustrate the dataset before and after it was cleaned. A detailed discussion of the dataset cleaning process follows.


# Split

A verification process was conducted to ensure the accuracy of the date format which was in YYYY-MM-DD. The team visually checked the dates using excel and Python to interpret the data correctly.

To enhance the data analysis, a treatment process was also performed. The original date variable was converted into three separate variables representing year, month, and day. The team used the dateline library to perform this feature engineering, which can help in better understanding the data or building predictive models.

While splitting the date into year, month, and day may not be directly relevant to estimating the probability of a team winning a match, it can be useful in analyzing whether the time of year or day of the week affects the outcome of a match or whether the performance of a team changes over time.




![Bild19](https://user-images.githubusercontent.com/129981869/236505200-1ad2740f-61cd-4afe-9c55-6814322452b7.png)

# Outliers
To ensure accurate analysis, it is important to identify and handle any outliers in the data. This process can involve either removing the outliers or treating them as a separate category, depending on the situation




![Bild20](https://user-images.githubusercontent.com/129981869/236505299-1f57ff54-6ae2-4a6f-9dc4-a572ce4f47b0.png)




![Bild21](https://user-images.githubusercontent.com/129981869/236505407-a1b0bbad-07d7-4be3-8507-2c92732e28aa.png)![Bild22](https://user-images.githubusercontent.com/129981869/236505515-b7959fd5-d255-4a93-84b6-817746292d80.png)


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
    


![Bild26](https://user-images.githubusercontent.com/129981869/236506097-f3e41779-eaec-4baa-a7d1-8ce93d5c5355.png) ![Bild27](https://user-images.githubusercontent.com/129981869/236506180-d1b02f47-6deb-4181-9f42-90b6c02f8daa.png)

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



![Bild33](https://user-images.githubusercontent.com/129981869/236506898-c42016c5-93b6-4df7-b162-221046d38bfa.png) ![Bild34](https://user-images.githubusercontent.com/129981869/236506952-9047a427-778d-4dbc-ae92-ddab65326319.png)

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




![Bild100](https://user-images.githubusercontent.com/129981869/236585167-d21f3b80-ea1a-48e4-ae04-4a526c91b2ea.png)


The researchers created a bar graph to visually compare the top players in the dataset before and after the cleaning process. The graph clearly showed the impact of the cleaning process, as the number of unique players decreased from 1400 to 1297 for the losers and from 899 to 844 for the winners. This reduction in the number of unique names indicates that many of the previously identified "unique" names were actually misspelled or duplicates.

By using the strip() method to remove trailing spaces and the replace() method to correct misspelled names and initials, the researchers were able to identify the correct and unique names of players. This ensures that the dataset is more accurate and precise, and will lead to more reliable results in any future analyses.






Before![Bild45](https://user-images.githubusercontent.com/129981869/236509106-6a8c65a8-053e-49e9-9f86-8c50321cfac6.png)


After![Bild46](https://user-images.githubusercontent.com/129981869/236509219-8882d3c0-2f65-448e-8f49-49c6e7f089a6.png)





# Concatenation

In order to ensure that the dataset is player-based, the researchers chose to divide the dataframe into two separate dataframes, one for the winner and one for the loser. Each dataframe will have its own set of corresponding attributes. To better understand this strategy, refer to the images below.


![Bild101](https://user-images.githubusercontent.com/129981869/236585617-07d6602a-cd05-485f-9863-57b2987da723.png)![Bil102](https://user-images.githubusercontent.com/129981869/236585662-287e11cd-a807-413e-aa6b-1708eac6a8ad.png)

Splitting the dataset into separate dataframes for the winner and the loser allows for more accurate and targeted analysis of each player's performance. By separating the data in this way, researchers can identify trends and patterns in the players' performances and compare them against each other. It also allows for easier processing and analysis of the data, as it eliminates the need to filter and sort the data every time a specific analysis is required. This approach helps to ensure that any insights or conclusions drawn from the data are more precise and reliable.

After the separation of the dataset into winner and loser dataframes, a new column called 'target' was added by the researchers. The 'target' column serves as the target variable and has two values, 1 and 0. The value 1 represents the winner and 0 represents the loser.


![Bild103](https://user-images.githubusercontent.com/129981869/236585799-4b06ae4c-e94a-4559-b8e1-46b00e8d3995.png)![Bild104](https://user-images.githubusercontent.com/129981869/236585831-66592bf5-e7a8-4b32-af12-21b99abc98b3.png)
The researchers also added few more columns

The two dataframes are concatenated, they are combined vertically into a single dataframe. This means that the rows of one dataframe are appended to the rows of the other dataframe to create a larger dataframe. The columns in the two dataframes must have the same name and type, otherwise an error will occur. After concatenation, the resulting dataframe will have the same number of columns as the original dataframes, but with a larger number of rows. 

![Bild105](https://user-images.githubusercontent.com/129981869/236585899-8b927cad-4a71-4e48-bcf4-fba4b8b57aad.png)


In the tennis dataset project, the researchers concatenated the winner and loser dataframes to form a single dataframe that contained information about both the winner and loser players for each match. This combined dataframe is now ready for data encoding.


![Bild106](https://user-images.githubusercontent.com/129981869/236585996-8727c1fa-69bb-44ed-a2b2-43cb8267a9eb.png)


# Data Encoding

Data encoding is a crucial step in data preprocessing that involves converting categorical data into numerical format for use in machine learning algorithms. This process is essential because most machine learning algorithms only accept numerical inputs.

Data encoding helps to reduce the dimensionality of the data, making it easier for machine learning algorithms to process. It also helps to avoid misinterpretation of categorical data as numerical values, which could lead to incorrect predictions or conclusions. By converting categorical data into numerical format, data encoding ensures that machine learning algorithms can effectively use the data to make accurate predictions or classifications.

# One Hot Encoding (with Dummies)

One hot encoding with dummies is an important technique used in data preprocessing to convert categorical variables into numerical variables. In the dataset provided, the columns, ‘ATP’, 'Location', 'Tournament', 'Series', 'Surface' and Players contain categorical variables that need to be converted into numerical variables for further analysis.

One hot encoding with dummies creates new binary columns for each unique value in the original categorical column. For example, in the 'Location' column, there are 115 unique locations. One hot encoding with dummies creates 115 new binary columns, one for each unique location. If a match was played in Paris, the value in the Paris column will be 1, and all other location columns will be 0. This allows us to convert categorical variables into numerical variables that can be used in mathematical computations.


![Bild107](https://user-images.githubusercontent.com/129981869/236586082-b0af1f00-4305-433b-9fcc-39ab41278f5d.png)


The importance of one hot encoding with dummies before modelling lies in the fact that most machine learning algorithms cannot handle categorical variables as inputs. These algorithms require numerical inputs to make predictions or classifications. By converting categorical variables into numerical variables, we can use these variables as inputs in machine learning models.

In addition, one hot encoding with dummies preserves the information in the original categorical variables, and it does not introduce any arbitrary ordering or hierarchy into the data. This means that the transformed data can be used in a wide range of machine learning models, without affecting the performance of the models.

This is an important technique in data preprocessing, especially when dealing with categorical variables. It helps to convert categorical variables into numerical variables that can be used in mathematical computations and machine learning algorithms. It is also important to perform this technique before modelling to ensure the accuracy and reliability of the models.


# Binary Encoding

This type of encoding is a suitable method for encoding categorical data with only two possible values, such as the "Outdoor" and "Indoor" values in the "Court" column. This encoding method represents each category as a sequence of binary digits, with each digit corresponding to a power of two.

This leads to a concise representation of the categories, which can be beneficial for machine learning models that require numerical input. Furthermore, binary encoding retains the order of the categories and can efficiently manage missing data.

![Bild108](https://user-images.githubusercontent.com/129981869/236586188-5b6113dc-217a-4bf5-b1b5-7c5a6b1bbc61.png)

Also, the researchers converted the "Comment" column into a binary variable. Completed is assigned the value 1, which indicates that the match was completed, while the other values (Retired, Walkover, and Disqualified) are assigned the value 0, which indicates that the match was not completed.

![Bild109](https://user-images.githubusercontent.com/129981869/236586233-e1ad6a3a-bcf8-4623-9087-70eb674b1ec4.png)

This encoding is appropriate for cases where we are interested in whether an event has occurred or not, and there are only a few possible outcomes. It is a type of binary encoding that can simplify the data and reduce the number of variables required to represent the information.

# Ordinal Encoding

This encoding is a good choice for encoding categorical data with a natural order or hierarchy, such as the "Round" column in the dataframe. Ordinal encoding maps each category to a unique integer based on its position in the order, preserving the order of the categories. This can be useful for machine learning models that can benefit from knowing the order or hierarchy of the categories.

Additionally, ordinal encoding is a simple and efficient encoding method that can handle missing data by assigning a special value, such as -1, to represent missing values.

![Bild110](https://user-images.githubusercontent.com/129981869/236586398-51f3f2ad-5528-4fab-9d3f-96774eff2c87.png)

The researchers created a dictionary round_rank where each round is assigned a numerical value based on its rank. The lowest rank, Round Robin, is assigned the value 0, while The Final, the highest rank, is assigned the value 7. This assigns a unique integer value to each category in a categorical variable, based on their order or rank.


# Dropping

Dropping columns was used by the researchers in preprocessing the dateset. One such reason is that some columns in a dataset contain irrelevant or unnecessary information that is not required for analysis. In this project we dropped the columns, ‘Date’, ‘Wsets’, ‘Lsets’, ‘proba_elo’, ‘PSW’,  ‘PSL’, and ‘month’. 

Dropping these columns can help to simplify the dataset and make it more manageable. Additionally, dropping columns can also help to reduce the noise in the dataset by removing columns with a lot of missing data or noise.

Furthermore, these columns contain redundant information, and dropping them can help to reduce the redundancy in the dataset. By dropping such columns, memory requirements can be reduced, and the efficiency of the analysis can be improved.

# Assessment methods:  

Reconstituted professional situation: from a set of company data, the candidate must implement various pre-processing and data augmentation to make them usable through machine learning techniques.


Result of transformation and cleaning before encoding:


![Bild111](https://user-images.githubusercontent.com/129981869/236586539-6c065898-2502-4e4e-9609-891dff8537b9.png)![Bild112](https://user-images.githubusercontent.com/129981869/236586555-4c5d98bb-c0cf-4eb4-8312-1b417839bb22.png)
After joining Winner and Loser dataset to get an player based data for the modelling.








# Report 2:

# Machine Learning Models

                           # Stages of the projects


# Classification of the Problem

The project is a classification problem as the objective is to predict the probability of a team winning a tennis match based on various features such as player rankings, previous wins, and court type. This aims to improve the accuracy of predictions compared to bookmakers' algorithms.

The main performance metric used to compare the models is likely to be the accuracy, which measures the percentage of correctly predicted match outcomes in the test dataset. This metric is appropriate as it directly reflects the model's ability to correctly classify the match outcomes and is the most common metric used for classification problems.

In addition to accuracy, other quantitative performance metrics such as precision, recall, and F1 score can provide additional insights into the model's ability to correctly classify positive and negative instances, and can be useful in evaluating the model's performance. 

Qualitative performance metrics, such as the confusion matrix, can also be helpful in identifying where the model is performing well and where it needs improvement.

# Model Choice and Optimization

  # Model 1: Decision Tree Classification
Decision Tree classification can be a suitable machine learning technique for achieving the objective of beating bookmakers' algorithms on estimating the probability of a team winning a match. By using various features such as player rankings, previous wins, and court type, the Decision Tree classifier can predict the outcome of a tennis match.

One reason to use Decision Tree classification is its interpretability. The resulting tree structure can provide insights into which features are most important for predicting the match outcome. This information can be used to improve the accuracy of the bookmakers' algorithms.

Another reason to use Decision Tree classification is its ability to handle both categorical and numerical data, making it suitable for sports analytics. It can also handle missing values and outliers, which are common in real-world datasets.

Furthermore, Decision Tree classification can be computationally efficient for large datasets with high dimensionality, which is important for handling the large amount of data required for predicting tennis match outcomes. Overall, Decision Tree classification can be a valuable tool for achieving the objective of this project.

![Bild113](https://user-images.githubusercontent.com/129981869/236588007-31b845bc-906d-49b2-ac39-77109eeb8a66.png)


In the project, it could be used to predict the probability of a team winning a match based on various input variables. The model would be trained on historical data to learn the relationship between the input variables and the probability of a team winning a match. The trained model could then be used to make predictions on new data to estimate the probability of a team winning a match.

![Bild114](https://user-images.githubusercontent.com/129981869/236588038-08d53020-2a83-46a4-91b0-68ada2140220.png)
Accuracy Score: 0.9394989935137553 
Score Train :        1.0
Score test :          0.9394989935137553


The output indicates that the Decision Tree Classifier model achieved an accuracy of around 94% in predicting the target variable for the test set. However, this high accuracy score may also indicate overfitting, where the model has become too complex and tailored to the training data, resulting in poor performance on new, unseen data.

The training score of the decision tree classifier model is 1.0, indicating that it has achieved a perfect fit with the training data. However, this could suggest that the model is overfitting since it may have memorized the training data instead of learning the underlying patterns.

On the other hand, the test score of the model is 0.93, indicating that it has performed well on unseen data. However, the significant difference between the training and test scores confirms that the model is overfitting to some extent, as it is performing much better on the training data than on the test data.

The confusion matrix indicates that the model correctly predicted 8856 instances for the true negatives (TN) class, incorrectly predicted 80 instances for the false positives (FP) class, incorrectly predicted 105 instances for the false negatives (FN) class, and correctly predicted 8843 instances for the true positives (TP) class.


![Bild115](https://user-images.githubusercontent.com/129981869/236588098-1dac1964-5696-428f-9485-af262fc6e9de.png)

According to the classification report, the precision for both classes is 0.99, indicating that the model has a high proportion of correct predictions for both classes. The recall for both classes is also 0.99, indicating that the model has a high rate of identifying actual positives. The F1-score for both classes is 0.99, indicating high accuracy in predicting both classes.
The support is the number of actual occurrences of the class in the test data, and the accuracy of the model is 0.99, which is very high.
However, despite the high performance metrics, it is possible that the model is overfitting.

  # Model 2: Decision Tree Regression
  
In the context of trying to beat bookmakers' algorithms on estimating the probability of a team winning a match, Decision Tree regression can be a useful machine learning technique. By using input features such as team statistics, player performance, and match conditions, a Decision Tree model can predict the probability of a team winning a match.

The interpretability of Decision Tree regression can also be beneficial in this objective, as it allows for understanding the important factors that contribute to a team's likelihood of winning. Additionally, the flexibility of Decision Tree regression can handle both linear and nonlinear relationships between the input features and the target variable, allowing for capturing more complex patterns in the data.

Finally, the computational efficiency of Decision Tree regression can be advantageous for large datasets with high dimensionality, which can be useful in the context of predicting the outcomes of many matches. Overall, Decision Tree regression can be a useful tool in the objective of trying to beat bookmakers' algorithms on estimating the probability of a team winning a match.


![Bild116](https://user-images.githubusercontent.com/129981869/236588160-ae8e5eb6-e8b7-45cd-a52c-a4243d37ebbe.png)

The training dataset has a score of 1.0, indicating that the model has fit the data perfectly. However, this high score may also suggest overfitting, where the model is overly complex and has memorized the training data instead of learning the underlying patterns.

On the other hand, the test dataset has a score of 0.766, which suggests that the model is able to predict approximately 76.65% of the variance in the target variable in the test dataset. This performance can be considered decent.

score train : 1.0 
score test : 0.766493217097309

Mean Squared Error: 0.05837620219190338
Root Mean Squared Error: 0.24161167643949533
Mean Absolute Error: 0.05837620219190338
R2 Score: 0.766493217097309

The MSE, RMSE, MAE, and R2 Score are common evaluation metrics used to assess the performance of regression models.
The MSE measures the average squared difference between the predicted and actual target values, with a lower MSE indicating better performance. The MSE value of 0.05837620219190338 suggests that the predicted target values are off by around 0.06 on average from the actual target values.
The RMSE is the square root of the MSE and measures the average difference between the predicted and actual target values in the same units as the target variable. A lower RMSE also indicates better performance. The RMSE value of 0.24161167643949533 means that, on average, the predicted target values are off by around 0.24 from the actual target values.
The MAE measures the average absolute difference between the predicted and actual target values, with a lower MAE indicating better performance. The MAE value is the same as the MSE value of 0.05837620219190338, indicating that the predicted target values are off by around 0.06 on average from the actual target values.
The R2 score (or coefficient of determination) measures the proportion of the variance in the target variable that can be explained by the independent variables in the model. The score ranges from 0 to 1, with a higher value indicating better performance. The R2 score of 0.766493217097309 suggests that the model explains around 77% of the variance in the target variable, which is a good performance.

  # Model 3: Logistics Regression
  
Logistic regression is a popular machine learning technique for binary classification problems, such as predicting whether a team will win or lose a match. It models the probability of the target variable (win or lose) based on the input features, which can include various team statistics such as past performance, player injuries, and home/away field advantage.
In the context of trying to beat bookmakers' algorithms on estimating the probability of a team winning a match, logistic regression can be a useful tool. By accurately predicting the outcome of a match, it can help identify potential betting opportunities where the bookmakers' odds differ from the predicted outcome. Additionally, logistic regression can be easily interpretable, allowing for insights into the relationships between the input features and the predicted probability of a team winning.


![Bild117](https://user-images.githubusercontent.com/129981869/236588231-10ac33a2-ff00-482c-bf16-601f0e70b5de.png)

The scores shows that the model is performing consistently on both the training set and the test set, with a score of 0.744 on the training set and 0.747 on the test set. The slight increase in score on the test set compared to the training set could be due to the model generalizing well to unseen data. 

The Confusion Matrix shows that 6087 instances were correctly predicted as TN, 2881 instances were incorrectly predicted as FP, 1727 instances were incorrectly predicted as FN, and 7189 instances were correctly predicted as TP.

![Bild118](https://user-images.githubusercontent.com/129981869/236588279-a6951016-03c5-498f-806f-f9c9cc409410.png)

In this project aimed at beating bookmakers' algorithms on estimating the probability of a team winning a match, precision, recall, and F1-score were used to analyze the performance of the model.

Precision, which measures the proportion of true positive cases among positive predictions, was 0.78 for predicting a win and 0.78 for predicting a loss. Recall, which measures the proportion of true positive cases that are correctly identified by the model, was 0.81 for predicting a win and 0.68 for predicting a loss. The F1-score, which is the harmonic mean of precision and recall, was 0.76 for predicting a win and 0.73 for predicting a loss.

The overall performance of the model was considered good based on these scores. The weighted average and macro average of precision, recall, and F1-score were also taken into account to compare the performance of the model across different classes.


  # Model 4: Linear Regression
  
Linear regression can be used to estimate the probability of a team winning a match, which is the primary objective of this project - to beat bookmakers' algorithms on estimating this probability.

This model is a simple yet effective method for modeling the relationship between a dependent variable and one or more independent variables. In the context of predicting match outcomes, the independent variables could be factors such as team rankings, player statistics, match location, and past performance. By training a linear regression model on historical data and testing it on new data, the model can learn to make accurate predictions on the probability of a team winning a match. This can help in identifying potential betting opportunities where the model's predictions differ significantly from the bookmakers' odds, and the model can be used to make profitable bets.
  

![Bild119](https://user-images.githubusercontent.com/129981869/236588355-d9167fd7-db68-41ea-a3c3-a4b908881d18.png)

MSE on the training set: 4.658812858842604e-26
MSE on the test set: 0.0013319759046108758

The results show that the mean squared error (MSE) on the training set is significantly lower than the MSE on the test set, indicating that the model may have overfit the training data.

The MSE on the training set is extremely low at 4.658812858842604e-26, which suggests that the model is able to predict the target variable very accurately on the training data. 

However, the MSE on the test set is higher at 0.0013319759046108758, indicating that the model may not perform as well when presented with new, unseen data.

Therefore, the model may not generalize well to new data, indicating the presence of overfitting.

The researchers decided to apply Ridge and Lasso regression to verify if the model is overfitting or not. 

Ridge Result:
MSE on the training set: 0.0008325432220229922
MSE on the test set: 0.0020644337291440343

Based on the results of Ridge and Lasso, it appears that the models may be overfitting the data. In the case of Ridge, the mean squared error (MSE) on the training set is significantly lower than the MSE on the test set, which could be a sign of overfitting. The MSE on the training set is 0.0008325432220229922, which indicates that the model can predict the target variable very accurately on the training data. However, the MSE on the test set is higher at 0.0020644337291440343, which suggests that the model may not generalize well to new, unseen data.

Lasso Result:
MSE on the training set: 0.2355202640351613
MSE on the test set: 0.23583025208025807

Similarly, in the case of Lasso, the MSE on the training set is again significantly lower than the MSE on the test set, which is indicative of overfitting. The MSE on the training set is 0.2355202640351613, which suggests that the model is fitting the training data very closely. However, the MSE on the test set is 0.23583025208025807, which is not significantly different from the MSE on the training set, and suggests that the model may not be able to generalize well to new data.

Overall, the results of both Ridge and Lasso indicate that the models may be overfitting the data, and further analysis is needed to improve their performance on new, unseen data.

At the end it appears that the linear regression model without regularization is overfitting the training data and not generalizing well to the test data. It may not be the best model for this dataset without applying some form of regularization, such as Ridge or Lasso regression.


  # Model 5: Random Forest
  
  
Random Forest is a popular machine learning algorithm used for both classification and regression tasks. It is a powerful model that can handle complex relationships between features and target variables. In the context of this project, Random Forest is a suitable algorithm to use because it can potentially improve the accuracy of predicting the probability of a team winning a match, which aligns with the project objective of beating bookmakers' algorithms.

Additionally, Random Forest can handle non-linear relationships and interactions between variables, which may be present in the data.


![Bild120](https://user-images.githubusercontent.com/129981869/236588431-79699296-374c-42b9-b0af-91a0e2559aef.png)

The classification report for both the training and test sets shows high precision, recall, and f1-score values for both classes (0 and 1), with an accuracy of 1.00 for the training set and 0.94 for the test set. This suggests that the random forest model is able to accurately classify the target variable (win or lose) for both the training and test sets.

However, there is a slight decrease in accuracy on the test set compared to the training set, indicating that the model may have overfit the training data to some extent. Additionally, the computation time of 2 hours suggests that the model may be computationally expensive and may not be suitable for large-scale applications.

Overall, the random forest model shows promising results in accurately classifying the target variable, but further analysis and testing may be needed to ensure that it is not overfitting and can be used in a practical setting.


![Bild121](https://user-images.githubusercontent.com/129981869/236588489-fef4521f-bdd9-4f24-a833-cf5a4bc06f85.png)

  # Model 6: Support Vector Machine
  
  
Support Vector Machine (SVM) is also a popular machine learning algorithm used for classification and regression analysis. In this project, SVM may have been chosen because it is a powerful algorithm that can handle high-dimensional datasets, and can be effective at identifying non-linear relationships between features.

Regarding the project objective, SVM could be used to try to beat bookmakers' algorithms on estimating the probability of a team winning a match by using various features such as the team's past performance, player statistics, and other relevant factors to predict the outcome of a game. 

By training an SVM model on historical data, it could be possible to identify patterns and relationships that may not be apparent through manual analysis, potentially leading to more accurate predictions and improved betting strategies.


![Bild122](https://user-images.githubusercontent.com/129981869/236588538-7847e037-3f4c-480c-8e67-83ae37d06d8a.png)

The accuracy score shows that the SVM model achieved high accuracy on both the training set (0.9806939551529386) and the test set (0.9785282934466563), indicating that the model is able to classify new data with high accuracy.

However, the long computation time of 5 hours suggests that the model may not be scalable for larger datasets or real-time predictions.

It's important to note that accuracy alone may not be the only important metric to consider, especially in a classification problem where the classes are imbalanced. Other metrics such as precision, recall, and F1-score may provide a more comprehensive evaluation of the model's performance.


# Model Choice

After evaluating six different machine learning models, the team ultimately chose logistic regression as the primary option and decision tree regression as the secondary choice. The logistic regression model exhibited a precision score of 0.78 for both predicting a win and predicting a loss, while the recall score was 0.81 for predicting a win and 0.68 for predicting a loss. The F1-score was 0.76 for predicting a win and 0.73 for predicting a loss.

Meanwhile, the decision tree regression model showed a perfect score of 1.0 on the training set, but a lower score of 0.766493217097309 on the test set. The model had a mean squared error of 0.05837620219190338, a root mean squared error of 0.24161167643949533, a mean absolute error of 0.05837620219190338, and an R2 score of 0.766493217097309.

Based on these results, the logistic regression model performed better on the test set, while the decision tree regression model showed signs of overfitting on the training set.

# PCA - Principal Component Analysis

PCA (Principal Component Analysis) is a technique used for reducing the dimensionality of large datasets. In the context of this project, the objective is to beat bookmakers' algorithms on estimating the probability of a team winning a match. To achieve this goal, the model needs to be able to handle a large amount of data and extract meaningful information from it. PCA can help to achieve this by reducing the number of features in the dataset while retaining most of the important information.

By reducing the number of features, PCA can simplify the model and improve its performance by reducing the risk of overfitting. This is important because overfitting can lead to poor generalization of the model to new data, which is crucial for accurately predicting the outcome of a match. Additionally, PCA can help to identify the most important features in the dataset and eliminate any redundant or irrelevant features.

Overall, the use of PCA in this project can help to improve the performance of the model by reducing the dimensionality of the data, simplifying the model, and identifying the most important features for accurately predicting the outcome of a match.



![Bild123](https://user-images.githubusercontent.com/129981869/236588603-a540b1b2-56ca-4758-a267-127950cf6ae9.png)

The researchers identified the eigenvalues which represent the variance explained by each principal component in the PCA analysis. It suggests that the first principal component explains the most variance (0.00200492), followed by the second (0.00190119), and so on.

![Bild124](https://user-images.githubusercontent.com/129981869/236588620-899fdc36-398c-411f-aada-4cf490bfc42a.png)

The second set of values represent the importance or weight of each principal component in the analysis. The first principal component has the highest weight (4.66350113), followed by the second (4.42223503), and so on. This suggests that the first few principal components are the most important in explaining the underlying variability in the data.

These eigenvalue were plotted below: 

![Bild125](https://user-images.githubusercontent.com/129981869/236588652-21b4d1e0-220f-44a6-8ed5-8046a2bb0e1e.png)

The pca.explained_variance_ratio_ attribute returns an array of the variance explained by each principal component as a fraction of the total variance. The array indicates that the first principal component accounts for 0.1999% of the total variance, the second principal component accounts for 0.1894%, the third principal component accounts for 0.1777%, the fourth principal component accounts for 0.1607%, and the fifth principal component accounts for 0.1567%. See graph below for visualization.


![Bild126](https://user-images.githubusercontent.com/129981869/236588675-4df91f70-8d73-47e5-b0c5-211dfb0a1db4.png)

Based on this analysis, it can be inferred that the first principal component explains the highest variance, while the subsequent components explain a progressively smaller amount of variance. The sum of the values in the array gives the total amount of variance explained by the five components, which is approximately 0.69%.

This information is helpful in deciding the number of principal components to include in the analysis, based on the desired level of explained variance.


![Bild127](https://user-images.githubusercontent.com/129981869/236588754-2e2d0fe2-ee75-43d6-afd3-a5060286f851.png)



![Bild128](https://user-images.githubusercontent.com/129981869/236588775-58bcf668-babe-4741-800a-75a3fb49fab2.png)


![Bild129](https://user-images.githubusercontent.com/129981869/236588797-fe27b589-f5f5-4948-a00d-6f369ed2753a.png)












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







                       # Final report  
                       # Conclusion drawn
#Difficulties encountered during the project
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

