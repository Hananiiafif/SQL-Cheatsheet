# SQL-Cheatsheet
Kumpulan Query SQL

## Select Function 
```Select query for all columns
SELECT * 
FROM mytable;
```
## Quueries With Constraits
```SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```
### Example
![hani](https://github.com/Hananiiafif/SQL-Cheatsheet/blob/main/Lesson%202.png)

## Quueries With Constraits Pt 2
### Example 
![hani](https://github.com/Hananiiafif/SQL-Cheatsheet/blob/main/Lesson%203.png)
```SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;
```

## Filtering and sorting Query results
### ini adalah Query untuk DISTINCT

```
SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);
```

### Ini adalah Query untuk ORDER BY

```
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC;
```

### Ini adalah Query untuk LIMIT
```
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;
```
## Simple SELECT Queries

### SELECT query
```
SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;
```
Question 
1. List all the Canadian cities and their populations
Answer 
SELECT city, population
FROM north_american_cities
WHERE country LIKE "Canada";

Question
2. Order all the cities in the United States by their latitude from north to south
Answer
SELECT city, latitude
FROM north_american_cities
WHERE country LIKE "United States"
ORDER BY latitude DESC;

Question 
3. List all the cities west of Chicago, ordered from west to east
Answer
SELECT city, longitude
FROM north_american_cities
WHERE longitude < "-88"
ORDER BY longitude ASC;

Question 
4. List the two largest cities in Mexico (by population)
Answer
SELECT city, population
FROM north_american_cities
WHERE country LIKE "Mexico"
ORDER BY population DESC
LIMIT 2;

Question
5. List the third and fourth largest cities (by population) in the United States and their population
Answer
SELECT city, population
FROM north_american_cities
WHERE country LIKE "United States"
ORDER by population DESC
LIMIT 2 OFFSET 2;
