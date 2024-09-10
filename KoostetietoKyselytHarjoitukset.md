#Koostetieto kyselyt harjoitukset
![image](https://github.com/user-attachments/assets/a5d7794e-7dec-48d5-b2c6-766af09c4fef)


1. SELECT max(elevation_ft) FROM airport;

2. SELECT continent, count(*) FROM country GROUP BY continent;

3. SELECT game.screen_name, count(*) FROM goal INNER JOIN goal_reached ON goal_reached.goal_id = goal.id 
   INNER JOIN game ON game.id = goal_reached.game_id GROUP BY game.screen_name;

4. SELECT screen_name FROM game WHERE co2_consumed in (SELECT min(co2_consumed) FROM game);

5. SELECT country.name, count(*) FROM airport INNER JOIN country ON country.iso_country = airport.iso_country GROUP BY airport.iso_country ORDER BY count(*) DESC LIMIT 50;

6. SELECT country.name FROM airport INNER JOIN country ON country.iso_country = airport.iso_country GROUP BY airport.iso_country HAVING count(*) > 1000;

7. SELECT name FROM airport WHERE elevation_ft in (SELECT max(elevation_ft) FROM airport);

8. SELECT country.name FROM airport INNER JOIN country ON country.iso_country = airport.iso_country WHERE elevation_ft in (SELECT max(elevation_ft) FROM airport);

9. SELECT count(*) FROM goal WHERE id in( SELECT goal_id FROM goal_reached WHERE game_id in( SELECT id FROM game WHERE screen_name = 'Vesa'));

10. SELECT name FROM airport WHERE longitude_deg in (SELECT min(longitude_deg) FROM airport WHERE latitude_deg in (SELECT min(latitude_deg) FROM airport));
