# Web Scraping and Data Analysis

This was my first Python project. My main goal was to apply some of what I had been studying for a while. Today, I see that a lot could have been written better (I need to make time to revisit the project), even so, during its development I not only learned a lot, but also fell in love with programming and the area of data science. Thus, I hope you enjoy it!





General objectives:

Creation of a database with 10.000 most listened songs in the last century on Brazilian radios and their lyrics. We intent to get insights by visualizing the evolution scenario, looking for trends and factors that indicate a greater probability of success for a new song.


PART I - Retriving the Data:

In this part we made requests to retrieve a list of the 100 most listened songs on stations radios in Brazil for each year, from 1920 to 2020. 
Then, we treat the data with BeautifulSoup and Regex techniques to organize it in a DataFrame.
For that, we will use the website "https://maistocadas.mus.br/", this site offers static information about musics in Brazil.

With that list in hands, we will make requests to retrive the lyrics of all those songs from the website "https://www.letras.mus.br/". 
Again, we used BeautifulSoup and Regex techniques to organize our data into a final DataFrame

The final DataFrame, with the artist, song name, year, position of rank and full lyric can be fund in this repository with the name 'years_1920_2020' 

PART II - Treating the Data and Initial Analysis:

In this part we created a summary grouped by year, it contain relevant informations of our DataFrame, like informations about the language of the songs, scrap success rate, if the song had the participation of other artists, etc.
This summary allowed us to began analysing the retrieved data, creating visualizations that generated the first insights.


PART III - Lyrics Analisys:

In this part we used nlkt library, regex and text mining techniques to analyze the lyrics. 
We were able to find the most frequent words for portuguese and english songs, normalizing the values according to the total quantity of each year.

Finally, we were able to better understand the evolution of songs on Brazilian radios, and even get insights on how to increase the probability of a song appearing in the top 100 most listened songs in the coming years.
