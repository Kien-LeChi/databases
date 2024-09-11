# Week 2

## Assignment 1
`SELECT * from goal;`

![screenshot](W3_E2_1.png)

## Assignment 2
`SELECT name, type from airport where iso_country = "FI";`

![screenshot](W3_E2_2.png)

## Assignment 3
`select name from airport where iso_country = "FI" order by name asc;`

![screenshot](W3_E2_3.png)

## Assignment 4
`select name, type from airport where iso_country = "FI" order by type asc, name asc;`

![screenshot](W3_E2_4.png)

## Assignment 5
`select name from country where name like "F%";`

![W3_E2_5.png](W3_E2_5.png)

## Assignment 6
`select name from country where name like "%F%";`

![W3_E2_6.png](W3_E2_6.png)

## Assignment 7
`select location from game where screen_name = "Vesa";`

![W3_E2_7.png](W3_E2_7.png)

## Assignment 8
`select co2_consumed from game where screen_name = "Ilkka";`

![W3_E2_8.png](W3_E2_8.png)

## Assignment 9
`select co2_budget from game where id = '1';`

![W3_E2_9.png](W3_E2_9.png)

## Assignment 10
`select screen_name, co2_budget, co2_consumed, @co2_left := co2_budget - co2_consumed as co2_left from game where screen_name = "Ilkka";`

![W3_E2_10.png](W3_E2_10.png)
