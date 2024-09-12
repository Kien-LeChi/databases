# Week 2

## Assignment 1
`SELECT * FROM goal;`

![screenshot](W3_E2_1.png)

## Assignment 2
`SELECT name, type FROM airport where iso_country = "FI";`

![screenshot](W3_E2_2.png)

## Assignment 3
`SELECT name FROM airport where iso_country = "FI" order by name asc;`

![screenshot](W3_E2_3.png)

## Assignment 4
`SELECT name, type FROM airport where iso_country = "FI" order by type asc, name asc;`

![screenshot](W3_E2_4.png)

## Assignment 5
`SELECT name FROM country where name like "F%";`

![W3_E2_5.png](W3_E2_5.png)

## Assignment 6
`SELECT name FROM country where name like "%F%";`

![W3_E2_6.png](W3_E2_6.png)

## Assignment 7
`SELECT location FROM game where screen_name = "Vesa";`

![W3_E2_7.png](W3_E2_7.png)

## Assignment 8
`SELECT co2_consumed FROM game where screen_name = "Ilkka";`

![W3_E2_8.png](W3_E2_8.png)

## Assignment 9
`SELECT co2_budget FROM game where id = '1';`

![W3_E2_9.png](W3_E2_9.png)

## Assignment 10
`SELECT screen_name, co2_budget, co2_consumed, @co2_left := co2_budget - co2_consumed as co2_left from game where screen_name = "Ilkka";`

![W3_E2_10.png](W3_E2_10.png)
