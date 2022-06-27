# Transfer-Market-Webscraping
Webscraping of the Football Transfer Market page of individual career goals
this Rmd file includes code that scrapes data using the rvest library and interacts with HTML. There are imperfections with the data cleaning portion, particularly in the column `For.1` which describes football club the player was on when they scored the goal.

The `clean_data` function has two specific arguments:

1. The name of the player (`player_name`) : This is in case an individual wants to bind rows with another player data set, this creates a new column to keep track of who score which goal. This will effectively populate the entire column of an individual player's name.
2. The weblink (`link`) : For the function to work properly, enter the player name and arrive at their general page. Next, hover over "Stats" to obtain a dropdown menu. Undr the tab "Goals", clic on "All Goals". Lastly, select the "Detailed" view rather than the "Compact". Your desired URL for any player should contain "plus/1" at the end.
