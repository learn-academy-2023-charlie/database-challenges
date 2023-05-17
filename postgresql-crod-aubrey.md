WHERE

##What is the population of the US? (HINT: 278357000)

SELECT population
FROM country 
WHERE name = 'United States'

##What is the area of the US? (HINT: 9.36352e+06)

SELECT country, surfacearea
From country
WHERE name = 'United States'

##Which countries gained their independence before 1963?

SELECT country, indepyear
From country
WHERE indepyear < 1963


##List the countries in Africa that have a population smaller than 30,000,000 and a life expectancy of more than 45? (HINT: 37 entries)

SELECT country, continent, population, lifeexpectancy
FROM country 
WHERE continent = 'Africa' AND population < 30000000 
AND lifeexpectancy > 45


##Which countries are something like a republic? (HINT: Are there 122 or 143?)

SELECT country, governmentform
FROM country
WHERE governmentform 
LIKE '%epublic'

There are 144 entries


##Which countries are some kind of republic and achieved independence after 1945? (HINT: 92 entries)

SELECT country, governmentform, indepyear
FROM country
WHERE governmentform 
LIKE '%epublic'
AND indepyear > 1945

##Which countries achieved independence after 1945 and are not some kind of republic? (HINT: 27 entries)

SELECT *
FROM country
WHERE governmentform
NOT LIKE('%epublic')
AND indepyear > 1945;