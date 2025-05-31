# Egalizator controlat cu comenzi vocale

tldr: am implementat filtrele cascadate si am gasit un script in python care face voice recognition. Pe parcurs daca este nevoie sa complic tema, pot pe parcurs sa fac eu ceva de la 0(spre exemplu calculor coeficientilor, script ul de python etc.). Voi avea doua
moduri de utilizare - basic(3 benzi, unde dau comenzi foarte simple, precum boost/cut la low/mid/hiw freqencies) si advanced(mai multe benzi, mai multe comenzi). O preblema in prezent este ca schimbarea numralului de filtre reseteza de tot parametrii.  
Partea originala la care m am gandit ar fi sa implementez un algoritmcare recalculeaza coeficientii, cand se realizeaza trecerea la advanced la basic(aici e mai greu), si de la basic la advanced, astfel incat sa se aproprie cat mai mult de cum se auzea inainte.


## (Instalare)
Pe langa MAX/MSP instalat, este nevoie de fisierele din prioect, MAX/MSP si python versiunea 3.12 si librariile pythonosc, sppechrecognition, myaudio, py.audio

## (Utilizare)
Deja existand casti unde este posibil sa modifici parametri eq-ului. Acest modul ar putea folosit de catre soferi drept un eq "hands free".


## (Istoric)

(13.05) ...

(3.06) ...

(X.06) ...

## (Link-uri)
https://www.youtube.com/watch?v=HitjKUix8WQ&t=42s&ab_channel=gmazel

# Dezvoltarea proiectului

Pentru început:

1. Creează-ți cont pe Github
2. Download și install [Github Desktop](https://desktop.github.com/)
3. Citește [acest ghid](https://charlesmartin.com.au/blog/2020/08/09/student-project-repository) și ține la îndemână [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet).

Apoi, procesul este următorul (inspirat de [aici](https://cs.anu.edu.au/courses/comp1720/deliverables/05-major-project/#submission-process)):

1. *fork* al acestui template către propriul tău cont de Github

![](assets/fork.gif)

_(dacă preferi cumva ca repo-ul să nu fie vizibil de către public, îl poți seta ca Private din Settings - "Change visibility". Atunci trebuie să mă adaugi drept colaborator, ca eu să am acces.)_

2. *clone* al repo-ului din Github Desktop pentru a-l downloada local

![](assets/clone.gif)

3. *commit* și *push* pe măsură ce lucrezi la proiect. Ultima versiune push-ată pe server înainte de deadline va conta pentru evaluare.

![](assets/commit.gif)

## Elemente obligatorii

1. Acest readme completat. Titlu, descriere, mod de utilizare, istoric, link-uri utile.

   Poți include și imagini și chiar [gif-uri animate](https://www.screentogif.com/), sau link-uri către materiale audio/video.
   
   Vezi [aici](https://charlesmartin.com.au/blog/2020/08/09/student-project-repository) mai multe sugestii.

2. [Declarația de originalitate](statement-of-originality.yml) completată. Tot ce nu este inclus acolo va fi considerat 100% contribuție proprie.

    *(formatul este adaptat de [aici](https://gitlab.cecs.anu.edu.au/comp1720/2018/comp1720-2018-major-project/-/blob/master/statement-of-originality.yml). Da, este un pic ironic să refolosim un doc [de altundeva](https://cs.anu.edu.au/courses/comp1720/resources/faq/#how-do-i-fill-out-my-statement-of-originality), dar menționăm sursa deci nu este plagiat!)*

3. Proiectul în sine. Tot codul trebuie să fie prezent, proiectul trebuie să poată rula conform instrucțiunilor din readme. Dacă e nevoie de asset-uri mari (sunete, video etc), [folosește Git LFS](https://git-lfs.github.com/) sau include link de download în instrucțiunile de instalare.

