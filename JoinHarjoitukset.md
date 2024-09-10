#Join harjoitukset
![image](https://github.com/user-attachments/assets/b956c688-fae5-412f-bd2b-37458ddf7439)


1. SELECT country.name AS 'country name', airport.name AS 'airport name' FROM airport INNER JOIN country ON country.iso_country = airport.iso_country WHERE country.name='Finland' AND airport.scheduled_service='yes';

2. SELECT game.screen_name, airport.name FROM airport INNER JOIN game ON game.location = airport.ident;

3. SELECT game.screen_name, country.name FROM airport INNER JOIN game ON game.location = airport.ident INNER JOIN country ON country.iso_country = airport.iso_country;

4. SELECT airport.name, game.screen_name FROM airport LEFT JOIN game ON game.location = airport.ident WHERE airport.name LIKE '%Hels%';

5. SELECT goal.name, game.screen_name FROM goal LEFT JOIN goal_reached ON goal_reached.goal_id = goal.id LEFT JOIN game ON game.id = goal_reached.game_id;
