### SQL GROUP BY QUERY ###

###  1. Contare quanti iscritti ci sono stati ogni anno  ###

```SQL
SELECT COUNT(*)
FROM `students`
GROUP BY (`enrolment_date`)
```
###  2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio  ###

```SQL
SELECT COUNT(id) , `office_address`
FROM `teachers`
GROUP BY `office_address` 
```
###  3. Calcolare la media dei voti di ogni appello d'esame  ###

```SQL
SELECT `exam_id` , AVG(`vote`) AS `avg_vote_for_exam` 
FROM `exam_student`
GROUP BY `exam_id`
```
###  4. Contare quanti corsi di laurea ci sono per ogni dipartimento  ###

```SQL
SELECT COUNT(`d`.`name`) AS `count_course_department`, `d`.`department_id`
FROM `degrees` AS `d` 
GROUP BY  `d`.`department_id`
```