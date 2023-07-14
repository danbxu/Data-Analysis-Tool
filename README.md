# Data-Analysis-Tool


Daniel Xu <br />
Tech used: Python, Pandas <br/>
Next steps: Use Scikit-Learn to apply machine learning concepts


Exploratory analysis indicated that there are no major issues with the provided dataset. <br/>
- Null values in 'area_name' column are a result of an unmarked area in the spawn location on CT side during the start of the game. <br />
- Null values in 'inventory' column are a result of when the player dies, the game empties the dead player's inventory on the ground, making the weapons <br />
  retrievable by other players <br />
  
  Conclusion: Dataset does not require further ETL. The correlation heatmap does show a few columns are strongly correlated with one another. Although it is generally good practice
  to remove correlated features, because of the nature of those features, the strong correlation should not affect my analysis and will not be removed. The correlated features are listed below:
  
  - 'armor', 'hp', and 'is_alive' 
  - 'tick' and 'round_num
  - 'z' and 'x' 
  - 'bomb_planted' and 'ct_alive'
  
Data extraction will be needed to obtain the weapon classes in the 'inventory' columns containing JSON objects.

Users can use this script to make game predictions such as the average time it takes players to enter a specified boundary with certain weapons and creating visualizations of player movement patterns.

The next steps of this script are implementing machine learning concepts and using Scikit-Learn library to make further predictions and analysis

