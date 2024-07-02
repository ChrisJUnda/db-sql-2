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
3. "Calcolare la media dei voti di ogni appello d'esame"
4. "Contare quanti corsi di laurea ci sono per ogni dipartimento"