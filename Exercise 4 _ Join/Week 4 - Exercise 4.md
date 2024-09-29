# Week 4

## Assignment 1

```sql
SELECT country.name as 'country name',
       airport.name as 'airport name' FROM country
INNER JOIN airport on country.iso_country = airport.iso_country
WHERE country.name = 'Finland' 
AND airport.scheduled_service = 'yes';
```

![W4E4_1.png](W4E4_1.png)

## Assignment 2
```sql
SELECT screen_name, name FROM game
JOIN airport ON location = ident;
```

![W4E4_2.png](W4E4_2.png)

## Assignment 3
```sql
SELECT screen_name, country.name FROM game
JOIN airport ON location = ident
JOIN country ON airport.iso_country = country.iso_country;
```

![W4E4_3.png](W4E4_3.png)

## Assignment 4
```sql
SELECT airport.name, screen_name FROM airport
LEFT JOIN game ON airport.ident = game.location
WHERE airport.name like "%Hels%";
```

![W4E4_4.png](W4E4_4.png)

## Assignment 5
```sql
SELECT goal.name, game.screen_name FROM goal
LEFT JOIN goal_reached ON goal.id = goal_reached.goal_id
LEFT JOIN game ON game_id = game.id;
```


![W4E4_5.png](W4E4_5.png)