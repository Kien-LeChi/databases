# Exercise 6

## Assignment 1

```sql
SELECT max(elevation_ft) FROM airport;
```
![W5E6_1.png](W5E6_1.png)

## Assignment 2
```sql
SELECT continent, count(*) from country
GROUP BY continent;
```
![W5E6_2.png](W5E6_2.png)

## Assignment 3
```sql
SELECT game.screen_name, COUNT(*) from goal_reached
LEFT JOIN game ON game_id = game.id
GROUP BY game.screen_name;
```
![W5E6_3.png](W5E6_3.png)

## Assignment 4
```sql
SELECT screen_name FROM game
WHERE co2_consumed IN (
    SELECT min(co2_consumed) FROM game
    );
```
![W5E6_4.png](W5E6_4.png)

## Assignment 5
```sql
SELECT country.name, count(*) FROM airport
LEFT JOIN country ON airport.iso_country = country.iso_country
GROUP BY airport.iso_country 
ORDER BY count(*) desc; 
```
![W5E6_5.png](W5E6_5.png)

## Assignment 6
```sql
SELECT country.name FROM airport
RIGHT JOIN country ON airport.iso_country = country.iso_country
GROUP BY airport.iso_country
HAVING count(airport.iso_country) >= 1000;
```
![W5E6_6.png](W5E6_6.png)
## Assignment 7
```sql
SELECT airport.name FROM airport
WHERE airport.elevation_ft IN (
    SELECT max(elevation_ft) FROM airport
    );
```
![W5E6_7.png](W5E6_7.png)
## Assignment 8
```sql
SELECT country.name FROM country
WHERE country.iso_country IN (
    SELECT airport.iso_country FROM airport
    WHERE airport.elevation_ft IN (
        SELECT max(elevation_ft) FROM airport
        )
    );
```
![W5E6_8.png](W5E6_8.png)
## Assignment 9
```sql
SELECT count(*) FROM goal_reached
WHERE goal_reached.game_id in (
    SELECT game.id FROM game
    WHERE game.screen_name = 'Vesa'
    );
```
![W5E6_9.png](W5E6_9.png)
## Assignment 10
```sql
SELECT name FROM airport
WHERE latitude_deg IN (
    SELECT min(latitude_deg) FROM airport
    );
```
![W5E6_10.png](W5E6_10.png)