### SQL JOIN QUERY ###


###  1. Selezionare tutti gli studenti iscritti al Corso di Laurea in Economia  ###

```SQL
SELECT *
FROM `students` AS `s`
JOIN `degrees` as `d`
ON `d`.`id`= `s`.`id`
JOIN `courses` AS `c`
ON `c`.`degree_id` = `d`.`id`
WHERE `d`.`name` = 'Corso di Laurea in Economia' 
```
###  2. Selezionare tutti i Corsi di Laurea Magistrale del Dipartimento di Neuroscienze  ###
###  3. Selezionare tutti i corsi in cui insegna Fulvio Amato (id=44)  ###
###  4. Selezionare tutti gli studenti con i dati relativi al corso di laurea a cuisono iscritti e il relativo dipartimento, in ordine alfabetico per cognome e nome  ###
###  5. Selezionare tutti i corsi di laurea con i relativi corsi e insegnanti  ###
###  6. Selezionare tutti i docenti che insegnano nel Dipartimento di Matematica (54) ###
###  7. BONUS: Selezionare per ogni studente il numero di tentativi sostenuti per ogni esame, stampando anche il voto massimo. Successivamente, filtrare i tentativi con voto minimo 18.  ###