<!-- Challenges: SQL Country Database
Save your queries in a file if you want to keep them for posterity.

WHERE
* What is the population of the US? (HINT: 278357000)

SELECT population, name 
FROM country
WHERE population > 278356000

"population"	"name"
1013662000	"India"
1277558000	"China"
278357000	"United States"

* What is the area of the US? (HINT: 9.36352e+06)

"surfacearea"	"name"
9.36352e+06	"United States"

* Which countries gained their independence before 1963?

"name"	"indepyear"
"China"	-1523
"Ethiopia"	-1000
"Japan"	-660
"Denmark"	800
"Sweden"	836
"France"	843
"San Marino"	885
"United Kingdom"	1066
"Portugal"	1143
"Andorra"	1278
"Thailand"	1350
"Spain"	1492
"Switzerland"	1499
"Netherlands"	1581
"Nepal"	1769
"United States"	1776
"Haiti"	1804
"Liechtenstein"	1806
"Colombia"	1810
"Chile"	1810
"Mexico"	1810
"Venezuela"	1811
"Paraguay"	1811
"Argentina"	1816
"Costa Rica"	1821
"Guatemala"	1821
"Peru"	1821
"Brazil"	1822
"Ecuador"	1822
"Bolivia"	1825
"Uruguay"	1828
"Greece"	1830
"Belgium"	1830
"Nicaragua"	1838
"Honduras"	1838
"El Salvador"	1841
"Dominican Republic"	1844
"Liberia"	1847
"Monaco"	1861
"Italy"	1861
"Canada"	1867
"Luxembourg"	1867
"Romania"	1878
"Australia"	1901
"Cuba"	1902
"Panama"	1903
"Norway"	1905
"Iran"	1906
"New Zealand"	1907
"Bulgaria"	1908
"South Africa"	1910
"Bhutan"	1910
"Albania"	1912
"Finland"	1917
"Hungary"	1918
"Poland"	1918
"Austria"	1918
"Yemen"	1918
"Yugoslavia"	1918
"Afghanistan"	1919
"Mongolia"	1921
"Ireland"	1921
"Egypt"	1922
"Turkey"	1923
"Holy See (Vatican City State)"	1929
"Iraq"	1932
"Saudi Arabia"	1932
"Syria"	1941
"Lebanon"	1941
"Iceland"	1944
"Indonesia"	1945
"Taiwan"	1945
"Vietnam"	1945
"Philippines"	1946
"Jordan"	1946
"Pakistan"	1947
"India"	1947
"South Korea"	1948
"Sri Lanka"	1948
"North Korea"	1948
"Myanmar"	1948
"Israel"	1948
"Oman"	1951
"Libyan Arab Jamahiriya"	1951
"Cambodia"	1953
"Laos"	1953
"Germany"	1955
"Morocco"	1956
"Tunisia"	1956
"Sudan"	1956
"Malaysia"	1957
"Ghana"	1957
"Guinea"	1958
"Chad"	1960
"Madagascar"	1960
"Mali"	1960
"Mauritania"	1960
"Congo, The Democratic Republic of the"	1960
"Congo"	1960
"Central African Republic"	1960
"Niger"	1960
"Nigeria"	1960
"Cameroon"	1960
"Cï¿½te dï¿½Ivoire"	1960
"Benin"	1960
"Senegal"	1960
"Somalia"	1960
"Cyprus"	1960
"Gabon"	1960
"Togo"	1960
"Burkina Faso"	1960
"Sierra Leone"	1961
"Kuwait"	1961
"Tanzania"	1961
"Uganda"	1962
"Burundi"	1962
"Trinidad and Tobago"	1962
"Samoa"	1962
"Rwanda"	1962
"Jamaica"	1962
"Algeria"	1962

* List the countries in Africa that have a population smaller than 30,000,000 and a life expectancy of more than 45? (HINT: 37 entries)

"name"	"continent"	"population"	"lifeexpectancy"
"Benin"	"Africa"	6097000	50.2
"Burkina Faso"	"Africa"	11937000	46.7
"Burundi"	"Africa"	6695000	46.2
"Djibouti"	"Africa"	638000	50.8
"Eritrea"	"Africa"	3850000	55.8
"Gabon"	"Africa"	1226000	50.1
"Gambia"	"Africa"	1305000	53.2
"Ghana"	"Africa"	20212000	57.4
"Guinea"	"Africa"	7430000	45.6
"Guinea-Bissau"	"Africa"	1213000	49
"Cameroon"	"Africa"	15085000	54.8
"Cape Verde"	"Africa"	428000	68.9
"Comoros"	"Africa"	578000	60
"Congo"	"Africa"	2943000	47.4
"Lesotho"	"Africa"	2153000	50.8
"Liberia"	"Africa"	3154000	51
"Libyan Arab Jamahiriya"	"Africa"	5605000	75.5
"Western Sahara"	"Africa"	293000	49.8
"Madagascar"	"Africa"	15942000	55
"Mali"	"Africa"	11234000	46.7
"Morocco"	"Africa"	28351000	69.1
"Mauritania"	"Africa"	2670000	50.8
"Mauritius"	"Africa"	1158000	71
"Mayotte"	"Africa"	149000	59.5
"Cï¿½te dï¿½Ivoire"	"Africa"	14786000	45.2
"Equatorial Guinea"	"Africa"	453000	53.6
"Rï¿½union"	"Africa"	699000	72.7
"Saint Helena"	"Africa"	6000	76.8
"Sao Tome and Principe"	"Africa"	147000	65.3
"Senegal"	"Africa"	9481000	62.2
"Seychelles"	"Africa"	77000	70.4
"Sierra Leone"	"Africa"	4854000	45.3
"Somalia"	"Africa"	10097000	46.2
"Sudan"	"Africa"	29490000	56.6
"Togo"	"Africa"	4629000	54.7
"Chad"	"Africa"	7651000	50.5
"Tunisia"	"Africa"	9586000	73.7

* Which countries are something like a republic? (HINT: Are there 122 or 143?)

"name"	"governmentform"
"Albania"	"Republic"
"Algeria"	"Republic"
"Angola"	"Republic"
"Argentina"	"Federal Republic"
"Armenia"	"Republic"
"Azerbaijan"	"Federal Republic"
"Bangladesh"	"Republic"
"Benin"	"Republic"
"Bolivia"	"Republic"
"Bosnia and Herzegovina"	"Federal Republic"
"Botswana"	"Republic"
"Brazil"	"Federal Republic"
"Bulgaria"	"Republic"
"Burkina Faso"	"Republic"
"Burundi"	"Republic"
"Chile"	"Republic"
"Costa Rica"	"Republic"
"Djibouti"	"Republic"
"Dominica"	"Republic"
"Dominican Republic"	"Republic"
"Ecuador"	"Republic"
"Egypt"	"Republic"
"El Salvador"	"Republic"
"Eritrea"	"Republic"
"South Africa"	"Republic"
"Ethiopia"	"Republic"
"Fiji Islands"	"Republic"
"Philippines"	"Republic"
"Gabon"	"Republic"
"Gambia"	"Republic"
"Georgia"	"Republic"
"Ghana"	"Republic"
"Guatemala"	"Republic"
"Guinea"	"Republic"
"Guinea-Bissau"	"Republic"
"Guyana"	"Republic"
"Haiti"	"Republic"
"Honduras"	"Republic"
"Indonesia"	"Republic"
"India"	"Federal Republic"
"Iraq"	"Republic"
"Iran"	"Islamic Republic"
"Ireland"	"Republic"
"Iceland"	"Republic"
"Israel"	"Republic"
"Italy"	"Republic"
"Austria"	"Federal Republic"
"Yemen"	"Republic"
"Yugoslavia"	"Federal Republic"
"Cameroon"	"Republic"
"Cape Verde"	"Republic"
"Kazakstan"	"Republic"
"Kenya"	"Republic"
"Central African Republic"	"Republic"
"China"	"People'sRepublic"
"Kyrgyzstan"	"Republic"
"Kiribati"	"Republic"
"Colombia"	"Republic"
"Comoros"	"Republic"
"Congo"	"Republic"
"Congo, The Democratic Republic of the"	"Republic"
"North Korea"	"Socialistic Republic"
"South Korea"	"Republic"
"Greece"	"Republic"
"Croatia"	"Republic"
"Cuba"	"Socialistic Republic"
"Cyprus"	"Republic"
"Laos"	"Republic"
"Latvia"	"Republic"
"Lebanon"	"Republic"
"Liberia"	"Republic"
"Lithuania"	"Republic"
"Madagascar"	"Federal Republic"
"Macedonia"	"Republic"
"Malawi"	"Republic"
"Maldives"	"Republic"
"Mali"	"Republic"
"Malta"	"Republic"
"Marshall Islands"	"Republic"
"Mauritania"	"Republic"
"Mauritius"	"Republic"
"Mexico"	"Federal Republic"
"Micronesia, Federated States of"	"Federal Republic"
"Moldova"	"Republic"
"Mongolia"	"Republic"
"Mozambique"	"Republic"
"Myanmar"	"Republic"
"Namibia"	"Republic"
"Nauru"	"Republic"
"Nicaragua"	"Republic"
"Niger"	"Republic"
"Nigeria"	"Federal Republic"
"Cï¿½te dï¿½Ivoire"	"Republic"
"Pakistan"	"Republic"
"Palau"	"Republic"
"Panama"	"Republic"
"Paraguay"	"Republic"
"Peru"	"Republic"
"Portugal"	"Republic"
"Poland"	"Republic"
"Equatorial Guinea"	"Republic"
"France"	"Republic"
"Romania"	"Republic"
"Rwanda"	"Republic"
"Germany"	"Federal Republic"
"Zambia"	"Republic"
"San Marino"	"Republic"
"Sao Tome and Principe"	"Republic"
"Senegal"	"Republic"
"Seychelles"	"Republic"
"Sierra Leone"	"Republic"
"Singapore"	"Republic"
"Slovakia"	"Republic"
"Slovenia"	"Republic"
"Somalia"	"Republic"
"Sri Lanka"	"Republic"
"Sudan"	"Islamic Republic"
"Finland"	"Republic"
"Suriname"	"Republic"
"Syria"	"Republic"
"Tajikistan"	"Republic"
"Taiwan"	"Republic"
"Tanzania"	"Republic"
"Togo"	"Republic"
"Trinidad and Tobago"	"Republic"
"Chad"	"Republic"
"Czech Republic"	"Republic"
"Tunisia"	"Republic"
"Turkey"	"Republic"
"Turkmenistan"	"Republic"
"Uganda"	"Republic"
"Ukraine"	"Republic"
"Hungary"	"Republic"
"Uruguay"	"Republic"
"Uzbekistan"	"Republic"
"Belarus"	"Republic"
"Vanuatu"	"Republic"
"Venezuela"	"Federal Republic"
"Russian Federation"	"Federal Republic"
"Vietnam"	"Socialistic Republic"
"Estonia"	"Republic"
"United States"	"Federal Republic"
"Zimbabwe"	"Republic"

* Which countries are some kind of republic and achieved independence after 1945? (HINT: 92 entries)

"name"	"governmentform"	"indepyear"
"Algeria"	"Republic"	1962
"Angola"	"Republic"	1975
"Armenia"	"Republic"	1991
"Azerbaijan"	"Federal Republic"	1991
"Bangladesh"	"Republic"	1971
"Benin"	"Republic"	1960
"Bosnia and Herzegovina"	"Federal Republic"	1992
"Botswana"	"Republic"	1966
"Burkina Faso"	"Republic"	1960
"Burundi"	"Republic"	1962
"Djibouti"	"Republic"	1977
"Dominica"	"Republic"	1978
"Eritrea"	"Republic"	1993
"Fiji Islands"	"Republic"	1970
"Philippines"	"Republic"	1946
"Gabon"	"Republic"	1960
"Gambia"	"Republic"	1965
"Georgia"	"Republic"	1991
"Ghana"	"Republic"	1957
"Guinea"	"Republic"	1958
"Guinea-Bissau"	"Republic"	1974
"Guyana"	"Republic"	1966
"India"	"Federal Republic"	1947
"Israel"	"Republic"	1948
"Cameroon"	"Republic"	1960
"Cape Verde"	"Republic"	1975
"Kazakstan"	"Republic"	1991
"Kenya"	"Republic"	1963
"Central African Republic"	"Republic"	1960
"Kyrgyzstan"	"Republic"	1991
"Kiribati"	"Republic"	1979
"Comoros"	"Republic"	1975
"Congo"	"Republic"	1960
"Congo, The Democratic Republic of the"	"Republic"	1960
"North Korea"	"Socialistic Republic"	1948
"South Korea"	"Republic"	1948
"Croatia"	"Republic"	1991
"Cyprus"	"Republic"	1960
"Laos"	"Republic"	1953
"Latvia"	"Republic"	1991
"Lithuania"	"Republic"	1991
"Madagascar"	"Federal Republic"	1960
"Macedonia"	"Republic"	1991
"Malawi"	"Republic"	1964
"Maldives"	"Republic"	1965
"Mali"	"Republic"	1960
"Malta"	"Republic"	1964
"Marshall Islands"	"Republic"	1990
"Mauritania"	"Republic"	1960
"Mauritius"	"Republic"	1968
"Micronesia, Federated States of"	"Federal Republic"	1990
"Moldova"	"Republic"	1991
"Mozambique"	"Republic"	1975
"Myanmar"	"Republic"	1948
"Namibia"	"Republic"	1990
"Nauru"	"Republic"	1968
"Niger"	"Republic"	1960
"Nigeria"	"Federal Republic"	1960
"Cï¿½te dï¿½Ivoire"	"Republic"	1960
"Pakistan"	"Republic"	1947
"Palau"	"Republic"	1994
"Equatorial Guinea"	"Republic"	1968
"Rwanda"	"Republic"	1962
"Germany"	"Federal Republic"	1955
"Zambia"	"Republic"	1964
"Sao Tome and Principe"	"Republic"	1975
"Senegal"	"Republic"	1960
"Seychelles"	"Republic"	1976
"Sierra Leone"	"Republic"	1961
"Singapore"	"Republic"	1965
"Slovakia"	"Republic"	1993
"Slovenia"	"Republic"	1991
"Somalia"	"Republic"	1960
"Sri Lanka"	"Republic"	1948
"Sudan"	"Islamic Republic"	1956
"Suriname"	"Republic"	1975
"Tajikistan"	"Republic"	1991
"Tanzania"	"Republic"	1961
"Togo"	"Republic"	1960
"Trinidad and Tobago"	"Republic"	1962
"Chad"	"Republic"	1960
"Czech Republic"	"Republic"	1993
"Tunisia"	"Republic"	1956
"Turkmenistan"	"Republic"	1991
"Uganda"	"Republic"	1962
"Ukraine"	"Republic"	1991
"Uzbekistan"	"Republic"	1991
"Belarus"	"Republic"	1991
"Vanuatu"	"Republic"	1980
"Russian Federation"	"Federal Republic"	1991
"Estonia"	"Republic"	1991
"Zimbabwe"	"Republic"	1980

* Which countries achieved independence after 1945 and are not some kind of republic? (HINT: 27 entries)

"name"	"governmentform"	"indepyear"
"Antigua and Barbuda"	"Constitutional Monarchy"	1981
"United Arab Emirates"	"Emirate Federation"	1971
"Bahamas"	"Constitutional Monarchy"	1973
"Bahrain"	"Monarchy (Emirate)"	1971
"Barbados"	"Constitutional Monarchy"	1966
"Belize"	"Constitutional Monarchy"	1981
"Brunei"	"Monarchy (Sultanate)"	1984
"Grenada"	"Constitutional Monarchy"	1974
"Jamaica"	"Constitutional Monarchy"	1962
"Jordan"	"Constitutional Monarchy"	1946
"Cambodia"	"Constitutional Monarchy"	1953
"Kuwait"	"Constitutional Monarchy (Emirate)"	1961
"Lesotho"	"Constitutional Monarchy"	1966
"Libyan Arab Jamahiriya"	"Socialistic State"	1951
"Malaysia"	"Constitutional Monarchy, Federation"	1957
"Morocco"	"Constitutional Monarchy"	1956
"Oman"	"Monarchy (Sultanate)"	1951
"Papua New Guinea"	"Constitutional Monarchy"	1975
"Qatar"	"Monarchy"	1971
"Saint Kitts and Nevis"	"Constitutional Monarchy"	1983
"Saint Lucia"	"Constitutional Monarchy"	1979
"Saint Vincent and the Grenadines"	"Constitutional Monarchy"	1979
"Solomon Islands"	"Constitutional Monarchy"	1978
"Samoa"	"Parlementary Monarchy"	1962
"Swaziland"	"Monarchy"	1968
"Tonga"	"Monarchy"	1970
"Tuvalu"	"Constitutional Monarchy"	1978

ORDER BY
* Which fifteen countries have the lowest life expectancy? (HINT: starts with Zambia, ends with Sierra Leonne)
* Which fifteen countries have the highest life expectancy? (HINT: starts with Andorra, ends with Spain)
* Which five countries have the lowest population density (density = population / surfacearea)? (HINT: starts with Greenland)
* Which countries have the highest population density?(HINT: starts with Macao)
* Which is the smallest country by area? (HINT: .4)
* Which is the smallest country by population? (HINT: 50)?
* Which is the biggest country by area? (HINT: 1.70754e+07)
* Which is the biggest country by population? (HINT: 1277558000)
* Who is the most influential head of state measured by population? (HINT: Jiang Zemin)

Subqueries: WITH
* Of the countries with the top 10 gnp, which has the smallest population? (HINT: Canada)
* Of the 10 least populated countries with permament residents (a non-zero population), which has the largest surfacearea? (HINT: Svalbard and Jan Mayen)

Aggregate Functions: GROUP BY
* Which region has the highest average gnp? (HINT: North America)
* Who is the most influential head of state measured by surface area? (HINT: Elisabeth II)
* What is the average life expectancy for all continents?
* What are the most common forms of government? (HINT: use count(*))
* How many countries are in North America?
* What is the total population of all continents?

Stretch Challenges
* Which countries have the letter ‘z’ in the name? How many?
* Of the smallest 10 countries by area, which has the biggest gnp? (HINT: Macao)
* Of the smallest 10 countries by population, which has the biggest per capita gnp?
* Of the biggest 10 countries by area, which has the biggest gnp?
* Of the biggest 10 countries by population, which has the biggest per capita gnp?
* What is the sum of surface area of the 10 biggest countries in the world? The 10 smallest?
* What year is this country database from? Cross reference various pieces of information to determine the age of this database. -->
