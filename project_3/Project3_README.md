
# Project 3: Creating a machine learning model to categorized text

## Problem Statement

We are a team of data scientist that are currently employed by Twitch. As twitch has been successful in their streaming business, recently twitch plans to create a forum community and has created a beta forum where they engaged a small group of players to test the effectiveness of the forum by creating content and comments to attract users. Due to the overwhelming response, the beta forum is currently filled with comments ranging from Dota2, League of legends to other games such as Valorant. Players who are only interested in Dota 2 have to scroll through a bunch of comments that were not related and thus raised a feedback to Twitch. The company has engaged our team to create a machine learning model to learn and categorized the data into sub forum to ensure users who are only interested in dota 2 can read and comment only in dota 2 forums without all the noise. My team and i will be constructing two categorical model which is mainly the Multinominal Naive Bayes and Logistic regression models. The success of this project would be to ensure the best model is able to at least be able to obtain more than 85% accuracy. 

Our audience would be software engineers, sales and marketing peers who will be working with us hand in hand to improve the forum and build on the improving the functionality as well as interesting added features that will be included at the end of the report. 
## Background

The gaming industry has evolved tremendously since the beginning of the first commercial arcade game, Pong that was created in 1972. Since then, the gaming industry has expanded by creating multiple platforms that can hold different types of games ranging from different devices such as consoles, personal computers to handheld devices. On top of that, the quality, game map size and speed in which the games can run have also been improving throughout the years.

##### Before Year 2000
Before the year 2000, most games have largely been held on platform such as PC, Console and Arcade. During that time, games that were held on various platforms were big and bulky which were not as portable as it is because cellphones during that time were not as advanced as compared to the current smartphones we are using now. The most successful released of the handheld system was the Gameboy that was invented by Nintendo during 1989. There was also a large disparity between the quality of the games as during the period before 2000 as games were usually held in 2-dimension. 

##### 2001 to present (The online boom)
The rise of technology (Internet and Mobile) that led to a huge growth for the gaming industry. Since the invention of portable gaming consoles such as the playstation portable(PSP)/Vita, Nintendo switch, Mobile Phone(Smartphones) and the most recent announcement of Valve handheld steam console, the rapid growth of the gaming industry on handheld devices grew rapidly. Since then, the growth in gaming revenue hosted on PC, Arcade and Console has been on a gradual decline.
([*Source*](https://www.visualcapitalist.com/50-years-gaming-history-revenue-stream/))

###### Game Type
In the past, the game quality and players interaction were limited to the technology that was available. Thus the games usually requires the players to complete a storyline and/or compete with a computer character. Players can only compete with another players if they are within close proximity through link cable, own similar devices and game type such a Pokemon. With the advanced in technology, games has since transformed into massive multipler online network(MMORPG) and are moving towards virtual reality. 

#### Online interactive games
This advancement also led to the creation of games like DOTA, DOTA 2, GTAV, league of legends, World of warcraft just to name a few. During the period between 2003 to 2007, DOTA 1 was very popular in most of the computer cafe (aka Lan Shop) in Singapore. The popularity in DOTA could be due to the simplicity of the task but difficult on other aspect such as different skills/keys with different characters as well as competition against each other in teams. As more and more people start to own personal computers/laptops at home as well as the improvement in internet speed and connectivity, people started to gradually transit to home gaming. 

#### Gaming Industry Now
The gaming industry has evolved beyond just playing game to pass time. With the growth and advance in technology, there are many avenues players can look to create content and collect income. To add further, the rise of e-sports, online streaming and competitions are creating more opportunities for passionate players to convert to choosing gaming as a career. Currently Dota2 is still very popular among gamers and the price pool has been increasing every year (excluding 2020). ([*Source*](https://www.statista.com/statistics/807889/dota-2-tournament-prize-pool/#:~:text=The%20timeline%20presents%20the%20annual,figure%20in%20the%20previous%20year.))

Currently, Dota 2 leads the top games award price money with league of legend 3 placing lower. ([*Source*](https://www.esportsearnings.com/games)) The latest Dota 2 competition will be held on October 2022 in Singapore. This would definitely recreate the hyped over Dota 2 once again among users. 
 ([*Source*](https://mothership.sg/2022/05/the-international-singapore/?fbclid=IwAR0urNOFJnsi6IMkndgF5PPgHS1qVT5zTsjNFWkGks79CxOB4jcJ0XLhNX8))

## Dataset Selected

* [`dota_df.csv`](dota_df.csv): Dota data scraped from Subreddit
* [`lol_df.csv`](lol_df.csv): League of Legends data scraped from Subreddit

The dataset contains titles and comments that were posted by users which could provide useful insight in helping us to build a strong and reliable machine learning model with impactful features. 


## Conclusion and Recommendation
|Model|Best Score|Accuracy(test)|Sensitivity|Specificity
|---|---|---|---|---|
|Multinomial NB (Count Vector)|0.878|0.878|0.893|0.868 
|**Multinomial NB (TF-IDF)**|0.891|**0.894**|0.841|0.932
|Logistic Regression (Count Vector)|0.870|0.874|0.759|0.958
|Logistic Regression (TF-IDF)|0.869|0.865|0.724|0.966


In conclusion, 
- Multinomial NB (TF-IDF) model has the best accuracy among all the other models in terms of predicting which category the features belongs to. 

- The result would help segregate comments obtained from the main beta forum and channel to sub forum that enables players to have a more cohesive discussion among similar area of interest. With more players coming together to share methods and learn from each other in terms of strategy as well as forming online teams, this would ultimately lead to user growth in Twitch as well as the respective games. 

- As Twitch is deriving its revenue from successful game streaming as well as user growth, Twitch could venture future into determining sentimental analysis as well as detecting negative comments on a particular game(beyond Dota2 and LOL) in ensuring the continuous success of such games. 

- Twitch can also utilise the ability of our categorical models to determine the rising trends of different games type and could have the power to guide content creator as well as the community to venture and stream live videos of such games as a form of entertainments. 


### Limitations and next steps

The limitations to our model is that our models are only able to learn and differentiate from useful features as well as large amount of data. If users decided to increase non-game related chatters or input images/gif to tell their story, our model would not be able to succesfully categorised the features/trend. 

Players can also use alternate forums to hold their discussions which could lead to a low daily active users which can ultimately lead to low collection of data. This would limit our models as we may not have enough strong features to train our models to make accruate and reliable predictions.

**Possible improvements**
- We can look to collect data directly from our twitch streaming live chatbox instead of relying on reddit forums. By doing so, we could obtain live updates on the games, strategies, trends and even events that are occuring/occuring soon. This timely update would also help twitch to make adequate preparation in view of a sudden surge in daily active users. 



## Authors

- [@zacharykwek15](https://github.com/zacharykwek15/GA-projects)

