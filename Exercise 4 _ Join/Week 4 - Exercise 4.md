# Week 4

## Assignment 1
`SELECT country.name as 'country name',` <br>
       `airport.name as 'airport name'` <br>
`FROM country` <br>
`INNER JOIN airport on country.iso_country = airport.iso_country` <br>
`WHERE country.name = 'Finland'` <br>
`AND airport.scheduled_service = 'yes';` <br>

![W4E4_1.png](W4E4_1.png)

## Assignment 2
`SELECT screen_name, name FROM game` <br>
`JOIN airport ON location = ident;`

![W4E4_2.png](W4E4_2.png)

## Assignment 3

`SELECT screen_name, country.name FROM game` <br>
`JOIN airport ON location = ident` <br>
`JOIN country ON airport.iso_country = country.iso_country;`

![W4E4_3.png](W4E4_3.png)

## Assignment 4

`SELECT airport.name, screen_name FROM airport` <br>
`LEFT JOIN game ON airport.ident = game.location` <br>
`WHERE airport.name like "%Hels%";`

![W4E4_4.png](W4E4_4.png)

## Assignment 5

`SELECT goal.name, game.screen_name FROM goal` <br>
`LEFT JOIN goal_reached ON goal.id = goal_reached.goal_id` <br>
`LEFT JOIN game ON game_id = game.id;`

![W4E4_5.png](W4E4_5.png)