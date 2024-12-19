### SQL GROUP BY QUERY ###

###  1. Contare quanti iscritti ci sono stati ogni anno  ###
```SQL
SELECT COUNT(*)
FROM `students`
GROUP BY (`enrolment_date`)
```
###  2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio  ###
###  3. Calcolare la media dei voti di ogni appello d'esame  ###
###  4. Contare quanti corsi di laurea ci sono per ogni dipartimento  ###