#Using MRP to Drive Sales
##I used machine learning to create a model that predicts sales from 12 grocery stores in India

Author: Mary Burns
Business Problems: Which features should these grocery stores focus on in order to drive sales.
Data: the source for this model is from a handful of grocery stores and supermarkets in India. The data features such as Item Type(ie dairy, meat, veggies), Fat Content, Location Area type, Item MRP, and Item Visibility


##Methods
Data preparation steps included filling in missing data with most frequent as well as changing categories titles in Fat Content. I dropped a few columns to keep the features the machine worked with relevant. I dropped Item Weight(this didn't correlate with sales and was missing a lot of data), Item Identifier (each row was unique making this column useless to the machine), Location size (redundant information), Location Year (no correlation to sales). 

##Results
[foodbox.pdf](https://github.com/meburns2011/Food-Sales-Predictions/files/9023737/foodbox.pdf)
This box and whiskers plot compares the performance of the different store types



[barfat.pdf](https://github.com/meburns2011/Food-Sales-Predictions/files/9023743/barfat.pdf)
This is a barplot showing sales from each location type of both Low Fat and Regular items. 

[scatter.pdf](https://github.com/meburns2011/Food-Sales-Predictions/files/9023780/scatter.pdf)
This scatterplot shows a close correlation with MRP and Sales


##Model
My final model was a simple regression tree and a linear regression model. Both models shows similar results for testing and training data. The results were moderate but reliable. I say they are reliabel because both the training and testing data were close together rather than the training data being much higher than the testing data. What I believe would increase the results for the tesing data would be to increase the amount of data available for the machine to train with. From the data set there are only 10 locations for the machine to pull from with two locations having much lower sales outputs the other 8 locations. 

##Recommendations
Stores should focus on item MRP when deciding on what to stock in their stores and what price to sell them at. Because there are two outlier stores that sell so much less than the other 8 stores I would recommend reevaluating those stores and the surrounding area (is there a larger supermarket close by that theyre competing with? Could those supermarkets be owned by the same company making them compete with themselves?) 


##Limitations and Next Steps
More data will definitely increase the accuracy of this model. 
