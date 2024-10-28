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
ini adalah Query untuk DISTINCT
```SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);
```

Ini adalah Query untuk ORDER BY
```SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC;
```

