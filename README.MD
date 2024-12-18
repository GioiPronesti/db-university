### MY SQL DB_UNIVERSITY ###

### 1. Selezionare tutti gli studenti nati nel 1990 ### 

```SQL
SELECT *
FROM `students`
WHERE YEAR(`date_of_birth`) = 1990
```
### 2. Selezionare tutti i corsi che valgono più di 10 crediti ###

```SQL
SELECT *
FROM `courses`
WHERE `cfu` > 10
```
### 3. Selezionare tutti gli studenti che hanno più di 30 anni ### 

```SQL
SELECT *
FROM `students`
WHERE YEAR(`date_of_birth`) < 1994
```
### 4. Selezionare tutti i corsi del primo semestre del primo anno di un qualsiasi corso di laurea ###

```SQL
SELECT `period`,`year` 
FROM `courses`
WHERE `year` = 1
```
### 5. Selezionare tutti gli appelli d'esame che avvengono nel pomeriggio (dopo le 14) del 20/06/2020 ###

```SQL
```

### 6. Selezionare tutti i corsi di laurea magistrale ###

```SQL
SELECT * 
FROM `degrees`
```

### 7. Da quanti dipartimenti è composta l'università ###

```SQL
SELECT COUNT(*) AS department_number 
FROM `departments`;
```

### 8. Quanti sono gli insegnanti che non hanno un numero di telefono? ###

```SQL
SELECT COUNT(*) AS teacher_not_number 
FROM `teachers`
WHERE `phone` IS NULL;
```