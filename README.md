# food-sales-predictions
Predicts the potential foods consumers will buy
This goal of this project was to help retailers understand that the properties of their products and outlets play a role in predicting sales.
Our data consisted of [Item_Identifier, Item_Weight, Item_Fat_Content, Item_Visibility, Item_Type, Item_MRP, Outlet_Identifier,
                       Outlet_Establishment_Year, Outlet_Size, Outlet_Location_Type, Outlet_Type, Item_Outlet_Sales]

All which were used to predict sales except the Item_Identifier and the Outlet_Identifier. This data was unimportant when it came to predicting sales since they were only identifiers for the items and outlets.

- Explanation of the data
  * In this data set there were missing values only in the Item_Weight and Outlet_Size columns. I filled all Item_Weight null values with the median of entire column.
  * I filled the Outlet_Size null values with "unknown".


# Graphs
- For this graph I created a barplot. I ranked all the categories by their sales and we can see that there is no clear winner or loser. The important thing that we can           take from this graph is all the categories of food fall within similar ranges of sales.

  ![foods_sales_graph](https://user-images.githubusercontent.com/97921525/157774535-2ab3c7ed-3919-43cc-a43c-0976d5e4afec.PNG)
    
    
   
  ![density_of_item_sales](https://user-images.githubusercontent.com/97921525/157774842-9e265ae6-27b6-4460-996a-033244f4de7d.PNG) 
   - For my second graph I created a density plot. With this graph we can see the distribution of sales prices between each outlet. We can see more or less how much each            outlet has in total sales. 
    
# Results
   * Our random forest model scored the best with a score of 61% on our training data and 60% on our testing data. Our Decision Tree Model performed similar with a training          score of 60% and a testing score of 59.5%. From our results we can see that we did not overfit or underfit our model althought our results weren't the highest. 

# Recommendations
  *  After completing the the project one thing that stood out to me was filling in the unknown outlets with "unknown". I believe if I did a little more digging I could've          maybe found a reason as to why a lot of those values were missing and instead filled them in with a better corresponding value rather than "unknown". I believe this            would'be led to better visualizations and maybe even a better score in our model. Although our Decision Tree model performed similar to our Random Forest model, the Random      Forest model would be the better option here since it has more variance and covers more of a range than our Decision Tree model. On top of having a higher overall score.
