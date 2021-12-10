# Personal-Dataset
Data115

HW11 Visualization
![image](https://user-images.githubusercontent.com/91580800/145515802-d91acffa-89aa-464f-a79f-561cb86030d1.png)
Code: library(ggplot2)
starbucks <- read.csv("Starbucks World Stats.csv")
ggplot(starbucks, aes(x=Population, y=Starbucks.per.million.inhabitants, color=Numer.of.Starbucks)) + geom_point()
*Note: The spelling error is from the orignal data source, not my own work. I fixed this later.*

Motivation:
The dataset I selected was Starbucks World data. With this data I set out, initially, to find out information about their sales of drinks and popularity, however, once thoroughly going over the data I found I was unable to come to any conclusions in this aspect due to the data I was given. Although I was uable to find the type of data I was looking for, this dataset still intrigued me, so I used it anyway. I just had to develop a new underlying question for this data to answer which ended up being, "How many Starbucks exist across the world per million inhabitants?" 

Data Process:
Initially, I had made the visualization above in Homework Assignment 11 to attempt to answer the question at hand. At the time, I though it would suffise, but after coming to a more recent conclusion I have decided to update the visual after going over the data, and understanding more thoroughly what I was asking. The initial visualization was close, but not perfect. I wanted to change the way the data is viewed in the visual, and give a better representation of how many Starbucks exist per million inhabitants overall. The outliers in the data, for visual purposes, were the only issues with this dataset; but everything was helpful and necessary to answer my underlying question, so there really wasn't much cleaning to be done. To recreate and update the visualization I decided to switch the "Number of Starbucks per Million Inhabitants" by country to color the visual, while the "Number of Starbucks" is the new Y scale. Keep in mind that the outliers are included for accuracy in this analysis because some countries are much larger than most others and contain many more Starbucks, but these data points are neccessary for an accurate depiction overall. I also fixed a spelling mistake on the data source's behalf and added a title.

Updated Visualization:
![image](https://user-images.githubusercontent.com/91580800/145515682-1cd60803-2091-49a4-8964-413f9ee27043.png)
Code: library(ggplot2)
starbucks <- read.csv("StarbucksWorldStats.csv")
ggplot(starbuck, aes(x=Population, y=Number.of.Starbucks, color=Starbucks.per.million.inhabitants)) + geom_point() + ggtitle("Number of Starbucks per Million Inhabitants")
This figure illustrates how many Starbucks exist per million inhabitants in 63 countries around the world. It is labeled with the number of Starbucks in that country on the y-axis, and the population along the x-axis, as well as colored by number of Starbucks per million inhabitants to show density. Overall, most countries have fewer than 15 Starbucks per million inhabitants, though the visual shows that there are some countries that have many more than that per million inhabitants, those countries being more mainstream and populated overall. China and India, for instance, have much higher populations than most other countries surveyed. And the United States accounts for the majority number of Starbucks overall.

Analysis:
This is the boxplot I created of the datset to help me initially realize that there were outliers affecting the data. I used this method in Homework Assignment 11, as the prompt to question 1C. This boxplot illustrates that some countries contain thousands more Starbucks than other smaller countries, but are therefore outliers of the data. This boxplot illustrates that the median number of Starbucks per million inhabitants is 2.16, the minimum is 0.04, the maximum is 13.62 and the interquartile range of number of Starbucks per million inhabitants is from approximately 1 to 8.  The largest outlier of Starbucks per million inhabitants is actually Canada with 40.53 because for the population being mildly average, they have quite a lot of Starbucks.
![image](https://user-images.githubusercontent.com/91580800/145489115-30a47783-ee8b-4999-a2e2-d8814741a728.png)

Conclusion:
After looking at specific data points and examples in this set, I decided to take the mean of number of Starbucks per million inhabitants to best answer my underlying question of "How many Starbucks exist per million inhabitants worldwide?" The answer to this question requires outliers to be included to find an accurate depiction of the data. I found that the average number of Starbucks per million inhabitants is 6.144. So, this data analysis has shown that there are about 6 Starbucks per million inhabitants worldwide.
