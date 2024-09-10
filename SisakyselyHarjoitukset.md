#Sisäkysely harjoitukset

1. SELECT name FROM country WHERE iso_country in( SELECT iso_country FROM airport WHERE name LIKE 'Satsuma%');

2. SELECT name FROM airport WHERE iso_country in( SELECT iso_country FROM country WHERE name LIKE 'Monaco');

3. SELECT screen_name FROM game WHERE id in( SELECT game_id FROM goal_reached WHERE goal_id in( SELECT id FROM goal WHERE name = 'CLOUDS'));

4. SELECT name FROM country WHERE iso_country NOT in( SELECT iso_country FROM airport);

5. SELECT name FROM goal WHERE id NOT in( SELECT goal_id FROM goal_reached WHERE game_id in( SELECT id FROM game WHERE screen_name = 'Heini'));
