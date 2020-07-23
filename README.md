# NBA Free Throws
## A study of whether the fans affect NBA free throws
You see it at every NBA game. When a player on the road team is shooting free throws, the fans behind the basket wave thundersticks to try to distract the shooter. But does it work?

We are going to look at how teams shoot free throws at home and on the road as well as how the road teams fare in each of the NBA arenas.

## Obtain the Data
The data from the 2018-19 season was scraped from NBA.com using the [nba_api API Client](https://github.com/swar/nba_api). There were 2,460 records that covered 1230 games, one record for each team fore each game. 

## Visualize the Data
First we will look at the histograms of all free throws attempted and made as well as the free throw percentage for each game.



The free thows attempted, free throws made, and free throw percentage all look relatively normal.

Next, we look at the boxplots. Free throws attempted and made can be shown on the same plot, but the free throw percentage will be looked at on a separate plot.

## Home vs Away
It is time to look at the home/away splits. We create a new column called Home and give it a boolean value based on the Matchup column. The Matchup column for the first game is GSW vs. OKC for GSW and GSW @ OKC for OKC. Therefore, if the fifth element is 'v', then the record is about the home team.

These histograms do look pretty similar, which makes it look like the fans do not make much of a difference. Let's break it down and look at each team and each venue to see if we can find places where the fans may make more of a difference.

## Metrics
We want to see if there is an advantage when it comes to free throw shooting. One way would be to check the free throw percentage of a team at home and compare it to the free throw percentage at a different venue. Then we can see if a certain venue shows a big difference.

For each venue, show the difference in percentage, possibly with a heat map.

For each team, show the difference in percentage in each venue.

