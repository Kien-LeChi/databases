`# Week 2

## Assignment 1
`SELECT country.name AS 'country name',`
`airport.name AS 'airport name'` <br>
`FROM country, airport` <br>
`WHERE country.iso_country = airport.iso_country` <br>
`AND country.name = 'Iceland';` <br>

![W3E3_1.png](W3E3_1.png)

## Assignment 2
`SELECT airport.name AS 'airport name'` <br>
`FROM airport, country` <br>
`WHERE type = "large_airport"` <br>
`AND airport.iso_country = country.iso_country` <br>
`AND country.name = "France";` <br>

![W3E3_2.png](W3E3_2.png)

## Assignment 3
`SELECT country.name AS 'country name',` <br>
`airport.name AS 'airport name'` <br>
`FROM country, airport` <br>
`WHERE country.iso_country = airport.iso_country;` <br>
`AND country.continent = 'AN';` <br>

![W3E3_3.png](W3E3_3.png)

## Assignment 4
`SELECT elevation_ft FROM game, airport` <br>
`WHERE game.screen_name = 'Heini'` <br>
`AND airport.ident = game.location;` <br>

![W3E3_4.png](W3E3_4.png)

## Assignment 5
`SELECT @elevation_m := airport.elevation_ft * 0.3048 as elevation_m` <br>
`FROM game, airport` <br>
`WHERE game.screen_name = "Heini"` <br>
`AND airport.ident = game.location;`

![W3E3_5.png](W3E3_5.png)

## Assignment 6
`SELECT name FROM airport, game` <br>
`WHERE game.screen_name = "Ilkka"` <br>
`AND game.location = airport.ident;`

![W3E3_6.png](W3E3_6.png)

## Assignment 7
`SELECT country.name FROM game, airport, country` <br>
`WHERE game.screen_name = "Ilkka"` <br>
`AND game.location = airport.ident` <br>
`AND airport.iso_country = country.iso_country;`

![W3E3_7.png](W3E3_7.png)

## Assignment 8
`SELECT goal.name FROM game, goal, goal_reached` <br>
`WHERE game.screen_name = "Heini"` <br>
`AND game.id = goal_reached.game_id` <br>
`AND goal_reached.goal_id = goal.id;` <br>

![W3E3_8.png](W3E3_8.png)

## Assignment 9
`SELECT airport.name FROM game, goal, goal_reached, airport` <br>
`WHERE game.screen_name = "Ilkka"` <br>
`AND game.id = goal_reached.game_id` <br>
`AND goal_reached.goal_id = goal.id` <br>
`AND goal.name = "Clouds"` <br>
`AND game.location = airport.ident;`

![W3E3_9.png](W3E3_9.png)

## Assignment 10
`SELECT country.name FROM game, goal,`
`goal_reached, airport, country` <br>
`WHERE game.screen_name = "Ilkka"` <br>
`AND game.id = goal_reached.game_id` <br>
`AND goal_reached.goal_id = goal.id` <br>
`AND goal.name = "Clouds"` <br>
`AND game.location = airport.ident` <br>
`AND airport.iso_country = country.iso_country;` 

![W3E3_10.png](W3E3_10.png)