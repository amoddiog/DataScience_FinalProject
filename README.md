# DataScience_FinalProject

## Introduction
Why was the project undertaken? What was the research question, the tested hypothesis or the purpose of the research?	

For this project, I have chosen to exam statistics from the Women's National Basketbal Association (WNBA). This project was undertaken to further develop my skills and understanding in data analysis. As a basketball player myself, I thought it would be interesting to see if there are any trends or relationships between the different types of stats. 

I decided to focus on three main research questions:  
1. **Do certain positions tend to get more assists than others?**  
* In basketball, there are five positions that we'll call 1, 2, 3, 4, and 5 for now. Typically the shorter players will play the 1 spot and the taller players will play the 5 spot. From the dataset, 1s, 2s, and 3s are considered Guards (G), 4s are considered Small Forwards (SF) or Forwards(F), and 5s are considered Centers (C). It's expected that Guards will have more assists because they bring the ball up the court the majority of the time and are the better ball-handlers. I'm interested to see if this holds true or if assists are more evenly distributed.

2. **Do centers/forwards have a better field goal percentage than guards?**  
* Because Centers and Forwards are taller and bigger, they tend to take more shots closer to the basket while guards take more shots from mid-range and beyond. Because of this, it would make sense that they would have a better field goal percentage (the percentage of shots made) because the shots they're taking are easier than the shots the guards take

3. **Is there any correlation between offensive rebounds and 2 point field goal attempts?**  
* An offensive rebound is when a team shoots the ball, misses, and then someone on that same team grabs the ball before someone else on the other team does. Most of the time, the rebound is grabbed close to the basket and the team is able to put up another shot almost immediately, so it would make sense that more offensive rebounds would lead to more 2 point field goal attempts.

The main purpose of this research is to gain some insight on how where you are on the court can affect your stats and to see how the stats are related.

## Selection of Data
What is the source of the dataset? Characteristics of data? Any munging, imputation, or feature engineering?

The data used in this analysis comes from a dataset called WNBA Stats 2018-2022 found on [kaggle](https://www.kaggle.com/datasets/jessalynlim/wnba-stats-20182022/) [1]. The creator of this dataset gathered all the information from [Basketball-Reference.com](https://www.basketball-reference.com/wnba/) [2].

The dataset includes stats for 885 players. Examples of the statistics included are team, position, field goal percentage, assists, rebounds, turnovers, and points. In total, there are 25 types of statistics listed for each player.  
Here's a preview of the data:  
(_insert preview of data here_)

Because I don't need all 25 statistics, I deleted the columns of the statistics I didn't need to make it easier to view.  
(_insert picture of new data_)

## Methodology
Tools:
* NumPy, Pandas, and Scikit-learn for data analysis and inference
* Jupyter Notebook for code

**Scikit**  
Scikit-learn was used to create a linear regression model for my third research question to see if there's a relationship between offensive rebounds and 2 point field goal attempts. A linear regression tests to see if there is a linear relationship between two varaibles, that is if one variable predicts another variable. A linear regression will give us a correlation coefficient that will tell us how strong the relationship is, if there is one at all.

## Results

## Discussion

## References
[1] [WNBA Stats 2018-2022](https://www.kaggle.com/datasets/jessalynlim/wnba-stats-20182022/)  
[2] [Basketball-Reference.com](https://www.basketball-reference.com/wnba/)
