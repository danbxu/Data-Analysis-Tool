# Data-Analysis-Tool


Daniel Xu <br />
Tech used: Python, Pandas <br/>
Next steps: Use Scikit-Learn to apply machine learning concepts


Exploratory analysis indicated that there are no significant issues with the provided dataset. <br/>
- Null values in the  'area_name' column are due to an unmarked area in the spawn location on the CT side during the start of the game. <br />
- Null values in the 'inventory' column are a result of when the player dies, the game empties the dead player's inventory on the ground, making the weapons <br />
  retrievable by other players <br />
  
The dataset does not require further ETL. The correlation heatmap does show a few features that are correlated with one another. Although it is generally good practice to remove correlated features, but because of the nature of those features, the strong correlation should not affect my analysis. The correlated features are listed below:
  
  - 'armor,' 'hp,' and 'is_alive' 
  - 'tick' and 'round_num
  - 'z' and 'x' 
  - 'bomb_planted' and 'ct_alive'
  
Data extraction is needed to obtain the weapon classes in the 'inventory' columns containing JSON objects.

Users can use this script to make game predictions, calculate the average time for a player to enter a specified boundary with specific weapons, and create visualizations of player movement patterns.

The next steps of this script are implementing machine learning concepts and using the Scikit-Learn library to make further predictions and data analysis.
