# SQL Tehtävät  

## Tehtävä 1  

## Tehtävä 2  

## Tehtävä 3  

## Tehtävä 4  
SELECT * FROM Kurssisuoritus  
## Tehtävä 5  
SELECT kurssi FROM Kurssisuoritus  
## Tehtävä 6  
SELECT DISTINCT kurssi FROM Kurssisuoritus  
## Tehtävä 7  
SELECT * FROM Opiskelija WHERE nimi='Anna'  
## Tehtävä 8  
SELECT * FROM Kurssisuoritus WHERE opiskelija='999999'  
## Tehtävä 9  
SELECT DISTINCT pääaine FROM Opiskelija WHERE pääaine like '%tiede%'  
## Tehtävä 10  
SELECT nimi, päivämäärä, arvosana FROM Kurssi, Kurssisuoritus WHERE Kurssi.kurssitunnus = Kurssisuoritus.kurssi
## Tehtävä 11  
SELECT nimi, päivämäärä, arvosana FROM Opiskelija, Kurssisuoritus WHERE Opiskelija.opiskelijanumero = Kurssisuoritus.opiskelija
## Tehtävä 12  
SELECT Kurssi.nimi AS kurssi, Tehtävä.nimi AS tehtävä FROM Kurssi, Tehtävä, Kurssitehtävä WHERE  Kurssi.kurssitunnus = Kurssitehtävä.kurssi AND Kurssitehtävä.tehtävä = Tehtävä.tunnus
## Tehtävä 13  
SELECT Kurssi.nimi AS kurssi, Tehtävä.nimi AS tehtävä FROM Kurssi, Kurssitehtävä, Tehtävä, Tehtäväsuoritus, Opiskelija WHERE Opiskelija.nimi ='Anna' AND Kurssi.kurssitunnus = Kurssitehtävä.kurssi AND Tehtävä.tunnus = Kurssitehtävä.tehtävä AND Tehtäväsuoritus.tehtävä = Kurssitehtävä.tunnus  AND Tehtäväsuoritus.opiskelija = Opiskelija.opiskelijanumero
## Tehtävä 14  

## Tehtävä 15  

## Tehtävä 16  
SELECT kurssi AS kurssikoodi, COUNT(*) AS lukumäärä FROM Kurssisuoritus GROUP BY kurssi
## Tehtävä 17  
SELECT kurssi.nimi AS kurssi, COUNT(Kurssisuoritus.kurssi) AS lukumäärä FROM kurssi, kurssisuoritus WHERE kurssi.kurssitunnus = kurssisuoritus.kurssi GROUP BY kurssi.nimi
## Tehtävä 18  

## Tehtävä 19  

## Tehtävä 20  
