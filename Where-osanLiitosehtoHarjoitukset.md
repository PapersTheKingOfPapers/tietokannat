#Where-osan liitosehto harjoitukset
![image](https://github.com/user-attachments/assets/8c9a8dcc-ae8b-49b6-a9b9-7fc704df2283)


1. SELECT country.name AS 'country name', airport.name AS 'airport name' FROM country, airport WHERE
   country.iso_country = airport.iso_country AND country.name = 'Iceland';

2. SELECT airport.name AS 'airport name' FROM country, airport WHERE
   country.iso_country = airport.iso_country AND country.name = 'France'
   AND airport.type = 'large_airport';

3. SELECT country.name AS country_name, airport.name AS airport_name FROM country, airport WHERE
   country.iso_country = airport.iso_country AND country.continent = 'AN';

4. SELECT airport.elevation_ft FROM airport, game WHERE
   game.screen_name='Heini' AND airport.ident = game.location;

5. SELECT airport.elevation_ft * 0.3048 AS elevation_m FROM airport, game WHERE
   game.screen_name='Heini' AND airport.ident = game.location;

6. SELECT airport.name FROM airport, game WHERE
   game.screen_name='Ilkka' AND airport.ident = game.location;

7. SELECT country.name FROM country, airport, game WHERE
   game.screen_name='Ilkka' AND airport.ident = game.location AND airport.iso_country = country.iso_country;

8. SELECT goal.name FROM goal, goal_reached, game WHERE
   game.screen_name='Heini' AND goal_reached.game_id = game.id AND goal_reached.goal_id = goal.id;

9. SELECT airport.name FROM airport, goal, goal_reached, game WHERE
   game.screen_name='Ilkka' AND airport.ident = game.location AND goal_reached.game_id = game.id AND goal_reached.goal_id = goal.id AND goal.name = 'CLOUDS';

10. SELECT country.name FROM country, airport, goal, goal_reached, game WHERE
   game.screen_name='Ilkka' AND airport.ident = game.location AND goal_reached.game_id = game.id AND
   goal_reached.goal_id = goal.id AND goal.name = 'CLOUDS' AND country.iso_country = airport.iso_country;
