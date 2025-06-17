# Egalizator controlat cu comenzi vocale

Am implementat filtrele cascadate si am gasit un script in Python care realizeaza voice recognition. Pe parcurs, daca este nevoie sa complic tema, pot implementa de la zero anumite componente (spre exemplu: calculul coeficientilor, scriptul de voice recognition etc.).

Voi avea doua moduri de utilizare:

SIMPLE — 3 benzi, cu comenzi simple (boost/cut pe low/mid/high frequencies)

Advanced — mai multe benzi si alte comenzi.

O problema intampinata in prezent este ca schimbarea numarului de filtre reseteaza toti parametrii.
Partea originala la care m-am gandit ar fi sa implementez un algoritm care recalculeaza coeficientii atunci cand se face trecerea de la Advanced la Basic (mai dificil) si de la Basic la Advanced, astfel incat sunetul sa ramana cat mai apropiat de cel anterior. Deoarece am intampinat dificultati la acest algoritm, am decis sa implementez functionalitatea VOLUME SMART CONTROL.




## (Instalare)
Pe langa MAX/MSP instalat, este nevoie de fisierele din prioect, MAX/MSP si python versiunea 3.12 si librariile pythonosc, sppechrecognition, myaudio, py.audio

## (Utilizare)
Deja exista casti unde este posibil sa modifici parametrii EQ-ului. Acest modul ar putea fi folosit de catre soferi drept un EQ "hands free".
De asemenea, comenzile pot fi date si prin intermediul unor meniuri de tip drop-down.

Utilizatorul mai intai trebuie sa porneasca muzica folosind comanda "START MUSIC". Dupa, va trebui sa selecteze dintre SIMPLE, ADVANCED sau RANDOM. La modul SIMPLE, avem pop, rock si EDM. La ADVANCED avem comenzi mai tehnice: low boost, mid boost si high boost. In ADVANCED va trebui sa dam si comanda SETTINGS, care va intra in partea de VOLUME SMART CONTROL — nivelul va fi scazut in timp ce vorbitorul da comanda. Acest state este trigger-uit si de comanda "HEY MAX". Acestea sunt principalele comenzi.


## (Istoric)

(11.04) - cercetare tema proiect  

(25.04) - am inceput sa lucrez la schematic + testare voice recognition 

(10.05) - implementare filtre 

(27.05) - ajustare a scopurilor (am renuntat pe moment la ideea cu recalcularea coeficientior, posibila imbunatatire pe viitor)

(10.06) - minor bugfixes + presentation mode


## Posibile imbunatatiri
- implementarea recalcularii coeficientilor
- imbunatatire algoritm de speech detection 
- 



## (Link-uri)
https://www.youtube.com/watch?v=HitjKUix8WQ&t=42s&ab_channel=gmazel


