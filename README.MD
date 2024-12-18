### MY SQL DB_UNIVERSITY ###

### 1 Selezionare tutti gli studenti nati nel 1990 ### 

```SQL
SELECT *
FROM `students`
WHERE YEAR(`date_of_birth`) = 1990
```
### 2 Selezionare tutti i corsi che valgono più di 10 crediti ###

```SQL
SELECT *
FROM `courses`
WHERE `cfu` > 10
```


