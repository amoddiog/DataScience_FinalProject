# Analysis of WNBA Stats

## Introduction
For this project, I have chosen to exam statistics from the Women's National Basketbal Association (WNBA). This project was undertaken to further develop my skills and understanding in data analysis. As a basketball player myself, I thought it would be interesting to see if there are any trends or relationships between the different types of stats. 

I decided to focus on three main research questions:  
1. **Do certain positions tend to get more assists than others?**  
* In basketball, there are five positions that we'll call 1, 2, 3, 4, and 5 for now. Typically the shorter players will play the 1 spot and the taller players will play the 5 spot. From the dataset, 1s, 2s, and 3s are considered Guards (G), 4s are considered Small Forwards (SF) or Forwards(F), and 5s are considered Centers (C). It's expected that Guards will have more assists because they bring the ball up the court the majority of the time and are the better ball-handlers. I'm interested to see if this holds true or if assists are more evenly distributed.

2. **Do centers/forwards have a better field goal percentage than guards?**  
* Because Centers and Forwards are taller and bigger, they tend to take more shots closer to the basket while guards take more shots from mid-range and beyond. Because of this, it would make sense that they would have a better field goal percentage (the percentage of shots made) because the shots they're taking are easier than the shots the guards take.

3. **Is there any correlation between offensive rebounds and 2 point field goal attempts?**  
* An offensive rebound is when a team shoots the ball, misses, and then someone on that same team grabs the ball before someone else on the other team does. Most of the time, the rebound is grabbed close to the basket and the team is able to put up another shot almost immediately, so it would make sense that more offensive rebounds would lead to more 2 point field goal attempts.

The main purpose of this research is to gain some insight on how where you are on the court can affect your stats and to see how the stats are related.

## Selection of Data
The data used in this analysis comes from a dataset called WNBA Stats 2018-2022 found on [kaggle](https://www.kaggle.com/datasets/jessalynlim/wnba-stats-20182022/) [1]. The creator of this dataset gathered all the information from [Basketball-Reference.com](https://www.basketball-reference.com/wnba/) [2].

The dataset includes stats for 885 players. Examples of the statistics included are team, position, field goal percentage, assists, rebounds, turnovers, and points. In total, there are 25 types of statistics listed for each player.  
Here's a preview of the data:  

![Picture 1](https://github.com/amoddiog/DataScience_FinalProject/blob/main/graph/data_overview.png)

Because I don't need all 25 statistics, I deleted the columns of the statistics I didn't need to make it easier to view.  

![Picture 2](https://github.com/amoddiog/DataScience_FinalProject/blob/main/graph/updated_data.png)

## Methodology
Tools:
* NumPy, Pandas, Matplotlib, and Scikit-learn for data analysis and inference
* Jupyter Notebook for code

**Scikit**  
Scikit-learn was used alongside NumPy to create a linear regression model for my third research question to see if there's a relationship between offensive rebounds and 2 point field goal attempts. A linear regression tests to see if there is a linear relationship between two varaibles, that is if one variable predicts another variable. A linear regression will give us a correlation coefficient that will tell us how strong the relationship is, if there is one at all.

**Pandas**  
Pandas was used to import the data and to manipulate the data set (delete rows, access certain data points, etc)

**Matplotlib**  
Matplotlib was used to create plots/visualizations for the data.

## Results  
**Do certain positions tend to get more assists than others?**  
It was found that guards average 2.4 assists, small forwards average 1.5 assists, forwards average 1.1 assists, and centers average 0.9 assists. These values were found by adding up all the assists for each position then dividing by the number of players in each positon. Visually, this is what this information looks like:
 
![Picture 3](https://github.com/amoddiog/DataScience_FinalProject/blob/main/graph/assists_barplot.png)  
The barplot clearly shows that guards tend to get more assists than the other positions. This result confirms my hypothesis that guards get more assists because they are the main ball handlers.

**Do centers/forwards have a better field goal percentage than guards?**  
It was found that centers and forwards had a combined average field goal percentage of 42.40% and guards had an average field goal percentage of 37.23%. These values were found by summing the field goal percentages for each position then dividing by the number of players in each position. Once again, my hypothesis was confirmed because the centers and forwards had a better field goal percentage.

**Is there any correlation between offensive rebounds and 2 point field goal attempts?**  
It was found that there is a correlation between offensive rebounds and 2 point field goal attempts, although it's not very strong. Here are the results from the linear regression:

![Picture 4](https://github.com/amoddiog/DataScience_FinalProject/blob/main/graph/linear_regression.png)  
Here we can see that the correlation coefficient is 0.39, which means 39% of the variance in 2 point field goal attempts is explained by offensive rebounds. The model also has a mean squared error of 6.37, which is pretty low. This indicates that the model fits the data well.

## Discussion
From this analysis, it seems that what position you play may have some effect on your stats. In the future, I think it would be interesting to take a deeper look into this to see what other stats are affected by what position you play, or just to see if there truly is any significant effect. I would also like to take a look at some of the other stats I didn't include to gain even more understanding on WNBA stats and how they interact with each other.

## References
[1] [WNBA Stats 2018-2022](https://www.kaggle.com/datasets/jessalynlim/wnba-stats-20182022/)  
[2] [Basketball-Reference.com](https://www.basketball-reference.com/wnba/)  
[3] [Jupyter Notebook Code](https://github.com/amoddiog/DataScience_FinalProject/blob/main/codes/Project_Code.ipynb)
