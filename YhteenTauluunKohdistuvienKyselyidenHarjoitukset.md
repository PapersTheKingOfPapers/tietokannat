#Yhteen tauluun kohdistuvien kyselyiden harjoitukset

1. SELECT * FROM goal
![image](https://github.com/user-attachments/assets/d65f79d3-d079-41e9-92a4-0a25d26cc585)

2. SELECT name airport_type FROM airport
   WHERE iso_country='FI'
![image](https://github.com/user-attachments/assets/1124bd10-d194-4cb6-b9fa-3bc94be7e5f7)

3. SELECT name FROM airport 
   WHERE iso_country='FI'
   ORDER BY name
![image](https://github.com/user-attachments/assets/c264d892-c2cb-447f-9c1a-7495f42e9bf3)

4. SELECT name, type FROM airport
   WHERE iso_country='FI'
   ORDER BY type, name
![image](https://github.com/user-attachments/assets/fcf06815-1c45-4b06-8767-5bc809c8ad20)

5. SELECT name FROM country
   WHERE name LIKE 'F%'
![image](https://github.com/user-attachments/assets/42f47757-85e5-434c-b68f-8e5172336cc5)

6. SELECT name FROM country
   WHERE name LIKE '%F%'
![image](https://github.com/user-attachments/assets/5b4159f4-427c-40ea-8326-6dffc7a07684)

7. SELECT location FROM game
   WHERE screen_name='Vesa'
![image](https://github.com/user-attachments/assets/d91f67c5-4f78-43c4-b0be-2bd4cc129fe6)

8. SELECT co2_consumed FROM game
   WHERE screen_name='Ilkka'
![image](https://github.com/user-attachments/assets/3feead67-1bb4-4b16-98b4-0ae81c1779b3)

9. SELECT DISTINCT co2_budget FROM game
![image](https://github.com/user-attachments/assets/d5e6cd74-d5ee-4373-b8a3-a7c0b61bf443)
