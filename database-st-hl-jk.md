QUESTION 1.

SELECT code, name, population, gnp
FROM country
WHERE population > 1e+8
AND gnp > 1e+6;

SELECT name, population
FROM country
WHERE population
BETWEEN 278356000
AND 278357000;

