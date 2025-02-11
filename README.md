# sql_project - Layan AlGhamdi

## 1. Retrieve all cinemas with a rating above 4
```sql
SELECT * FROM ksa WHERE rating > 4;
```
<img width="1081" alt="Screenshot 1446-08-12 at 11 48 55 AM" src="https://github.com/user-attachments/assets/2651e3b8-72eb-455b-b077-2af93ed5f436" />

## 2. Find the total number of cinemas in the dataset
```sql
SELECT COUNT(*) AS total_cinemas FROM ksa;
```
<img width="569" alt="Screenshot 1446-08-12 at 11 50 18 AM" src="https://github.com/user-attachments/assets/d88e7515-f1a9-4509-a3fb-3b055427622d" />

## 3. Retrieve cinemas where comments contain the word 'amazing'
```sql
SELECT * FROM ksa WHERE best_comment LIKE '%amazing%';
```
<img width="931" alt="Screenshot 1446-08-12 at 11 57 26 AM" src="https://github.com/user-attachments/assets/c20ef6fa-eea1-4ea5-bec1-03eab9f2ee03" />

## 4. Get the average rating of cinemas
``` sql
SELECT AVG(rating) AS avg_rating FROM ksa;
```
<img width="487" alt="Screenshot 1446-08-12 at 11 58 53 AM" src="https://github.com/user-attachments/assets/e75bfe62-7562-4d4d-8726-7dbd63f8ed51" />

## 5. Count how many cinemas belong to each genre
``` sql
SELECT genre, COUNT(*) FROM ksa GROUP BY genre;
```
<img width="533" alt="Screenshot 1446-08-12 at 12 00 44 PM" src="https://github.com/user-attachments/assets/96bba82b-2a6c-4085-9156-e4b27c3bf40f" />

## 6. List all unique locations in the dataset
``` sql
SELECT DISTINCT location FROM ksa;
```
<img width="512" alt="Screenshot 1446-08-12 at 12 01 44 PM" src="https://github.com/user-attachments/assets/2ddcc578-2095-4ffc-9956-1a54345bd374" />

## 7. Find the cinema with the lowest rating
``` sql
SELECT * FROM ksa ORDER BY rating ASC LIMIT 1;
```
<img width="737" alt="Screenshot 1446-08-12 at 12 03 20 PM" src="https://github.com/user-attachments/assets/d954b9cb-ab95-4ffa-a6b0-d87ca97d7fe4" />

## 8. Retrieve cinemas in a specific city (example: Jubail)
```sql
SELECT * FROM ksa WHERE location LIKE '%Jubail%';
```
<img width="992" alt="Screenshot 1446-08-12 at 12 04 58 PM" src="https://github.com/user-attachments/assets/67ea39be-7f0c-4534-aea0-0587468d66bd" />

## 9. Find cinemas that have the word 'theater' in their name
```sql
SELECT * FROM ksa WHERE name LIKE '%theater%';
```
<img width="972" alt="Screenshot 1446-08-12 at 12 06 25 PM" src="https://github.com/user-attachments/assets/9ed01366-23e1-4383-ac43-2a088c03249c" />

## 10. Find the most common rating in the dataset
```sql
SELECT rating, COUNT(*) FROM ksa GROUP BY rating ORDER BY COUNT(*) DESC LIMIT 1;
```
<img width="734" alt="Screenshot 1446-08-12 at 12 07 27 PM" src="https://github.com/user-attachments/assets/79882c73-a5cf-48b0-800c-e90deff2e38f" />




