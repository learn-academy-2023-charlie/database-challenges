
Challenges: SQL Country Database
Save your queries in a file if you want to keep them for posterity.

WHERE
What is the population of the US? (HINT: 278357000)
<!-- SELECT code, name, population, gnp
FROM country
WHERE population > 1e+8
AND gnp > 1e+6;

SELECT name, population
FROM country
WHERE population
BETWEEN 278356000
AND 278357000; -->

What is the area of the US? (HINT: 9.36352e+06)

<!-- SELECT name, population, surfacearea
FROM country
WHERE population=278357000
AND surfacearea >= 9.36352e+06 -->

Which countries gained their independence before 1963?
<!-- 
SELECT name, indepyear
FROM country
WHERE indepyear <= 1963 -->

List the countries in Africa that have a population smaller than 30,000,000 and a life expectancy of more than 45? (HINT: 37 entries)
<!-- WITH africa_countries AS (
SELECT name,region, population, lifeexpectancy
FROM country
WHERE region='Africa'
AND population < 30000000
)
SELECT name, region, population, lifeexpectancy
FROM africa_countries
WHERE lifeexpectancy > 45; -->   work in progress


Which countries are something like a republic? (HINT: Are there 122 or 143?)
Which countries are some kind of republic and achieved independence after 1945? (HINT: 92 entries)
Which countries achieved independence after 1945 and are not some kind of republic? (HINT: 27 entries)



