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
WHERE TIMESTAMPDIFF(YEAR, `date_of_birth`, CURDATE()) > 30
```
### 4. Selezionare tutti i corsi del primo semestre del primo anno di un qualsiasi corso di laurea ###

```SQL
SELECT `period`,`year` 
FROM `courses`
WHERE `year` = 1
AND `period` = 'I semestre'
```
### 5. Selezionare tutti gli appelli d'esame che avvengono nel pomeriggio (dopo le 14) del 20/06/2020 ###

```SQL
SELECT * , HOUR(`hour`)
FROM `exams`
WHERE `date` = '2020-06-20' AND 
HOUR(`hour`) >= 14
```

### 6. Selezionare tutti i corsi di laurea magistrale ###

```SQL
SELECT * 
FROM `degrees`
WHERE `level` = 'magistrale'
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

### 9. Inserire nella tabella degli studenti un nuovo record con i propri dati (per il campo degree_id, inserire un valore casuale) ###

```SQL
UPDATE `teachers`
SET `office_number` = '126'
WHERE `id` = 58
```

### 10. Cambiare il numero dell'ufficio del professor Pietro Rizzo in 126 ### 
```SQL

```


### 11. Eliminare dalla tabella studenti il record creato precedentemente al punto 9 ### 
```SQL

```