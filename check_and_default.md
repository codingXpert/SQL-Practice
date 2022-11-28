


 ## AND , OR , NOT Clause

```sql
SELECT * FROM students 
WHERE age >= 18 AND age <= 23;
SELECT * FROM students;

SELECT * FROM students 
WHERE age >= 18 AND city = 'hazaribagh';
SELECT * FROM students;

SELECT * FROM students 
WHERE age >= 18 OR age <= 23;
SELECT * FROM students;

SELECT * FROM students 
WHERE NOT city = 'hazaribagh';
SELECT * FROM students;

SELECT * FROM students 
WHERE NOT city = 'hazaribagh' AND age <= 23;
SELECT * FROM students;

```