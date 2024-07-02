Nome esercizio: DB-SQL-2
Consegna:
Nuova repository, vi allego query GROUP BY e JOIN da risolvere.
Caricate il file con le query (formattate).
Buon divertimento


Query Con Group By 

1) "Contare quanti iscritti ci sono stati ogni anno"

SELECT YEAR(`enrolment_date`) AS 'anno',
COUNT(*) AS 'totale_iscritti'
FROM
    `students`
GROUP BY anno;

2. "Contare gli insegnanti che hanno l'ufficio nello stesso edificio"

SELECT
    `office_address` AS edificio,
    COUNT(`id`) AS totale_insegnanti
FROM
    `teachers`
GROUP BY
    edificio
ORDER BY
    edificio


3. "Calcolare la media dei voti di ogni appello d'esame"

SELECT
   `exam_id` AS esame,
   AVG(`vote`) AS media_voti
   FROM
   `exam_student`
   GROUP BY
   `exam_id`
   ORDER BY
   `exam_id` ASC;

4. "Contare quanti corsi di laurea ci sono per ogni dipartimento"

SELECT
    `department_id`,
    COUNT(`name`) AS totale_corsi
FROM
    `degrees`
GROUP BY
    `department_id` 