# Web Scrapping and Analysis - FMOVIES.TO

# Introduction 

This is a web crawling and analysis project. [Fmovies](fmovies.to/home) is a website to stream movies and tv shows online for free. For this project, first 50 pages of the most-watched section of this website has been crawled and analysed. 
The data was fetched on Tuesday, July 14,2020. 

## Libraries Used:
For web crawling and parsing the Requests and  Beautiful soup packages were used. 

## File Structures

There are three files each for crawling, tidying and analysing sections respectively. 

# Analysis


## Genre Portions 

Movies |  Tvs
:-------------------------:|:-------------------------:
![img](https://github.com/nibukdk/web-scrapping-fmovie.to/blob/master/Imgs/genre_n_movies.png) | ![img](https://github.com/nibukdk/web-scrapping-fmovie.to/blob/master/Imgs/genre_n_tvs.png) 


From the pie chart most of the movies have genre Drama, Action, Comedy.. and so on in that order, while we should remember, mostly a movie has multiple genre. In TV screens most of the shows are Drama,Comedy and Action, while we should remember, mostly a show has multiple genre.

## Genre Ranks

Movies |  Tvs
:-------------------------:|:-------------------------:
![img](https://github.com/nibukdk/web-scrapping-fmovie.to/blob/master/Imgs/views_n_genres_mv.png) | ![img](https://github.com/nibukdk/web-scrapping-fmovie.to/blob/master/Imgs/views_n_genres_tv.png) 

### Movies
Its seems among **Action, Adventures,Sci-Fi, Fantasy** are the genres that are very popular in general. Moreover, **Comedy** is like a potato, bleding in anywhere. Genres like **Drama, Romance** top the chart amons least watched, while **Documentary, war** does not seems to crowd favorite as these genres attract only a certain group of people.But at the end of the day, either be movies or tvs, their popularity depends on many other factors like story, plot, cast, marketing, producers, star casts and so on.


### TVS

From plot, on contrary to Movies, **Drama** is very popular genre in small screens followed by **Crime** in second and then **Action** in the third most watched genre. **Documentary** is still not popluar here as well. **Horror** shows take equal stance in fmovies.


## IMDB Vs. Top 30 and Bottom 30 Movies

Top 30 |  Bottom 30
:-------------------------:|:-------------------------:
![img](https://github.com/nibukdk/web-scrapping-fmovie.to/blob/master/Imgs/imdb_vs_30_most_watched_mv.png) | ![img](https://github.com/nibukdk/web-scrapping-fmovie.to/blob/master/Imgs/imdb_vs_30_least_watched_mv.png) 

As we can see form both charts, Its clear that IMDB in general does effect the watch count. Most watched movies do have high IMDB ratins. But the Bottom thirty some movies are there which still have very high ratings like "Eternal sunshine of spotless mind",8.3 imdb. 


## Ranking Each Year By most movies watched


![img](https://github.com/nibukdk/web-scrapping-fmovie.to/blob/master/Imgs/yr_rank_most_watched_mv.png)

**Coding Logic:** *Lets Rank the year using pd.Rank with "min" being the highest rank. 
We know that lower the value higher the rank, however, plotting will show opposite.Lets subtract all values by 60 as max value being 42. By doing so smallest rank becomes highest and gets biggest size in plot.*


Year 1991 is ranked highest, while 1996 is lowest which is 42.


## Movies Released Per Year

![img](https://github.com/nibukdk/web-scrapping-fmovie.to/blob/master/Imgs/Movie_releases_per_yr.png)

While the time I created this plot if July 15,2020,  fmovies, has the movies from 1971-2020. The number of movies is increasing from 2012, while 2019 being the year with most movies.

**Note:** *These movies are all from the most-watched list from just first 50 pages of fmovies.to, not all the movies in inventory.*
