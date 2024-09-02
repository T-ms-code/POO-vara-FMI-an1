# Aplicatie (online) de gestionare a unui magazin de imbracaminte sportiva. Aplicatia prezinta o interfata atat pentru cumparatori, cat si pentru vanzatori.

## Cerințe obligatorii 

Nerespectarea duce la nepunctarea proiectului

- programul va fi scris în C++
- programul va avea un meniu interactiv (doar pentru ilustrarea funcționalității)
- programul nu are erori de compilare
- programul nu are warning-uri (folosind -Wall)
- existența a minim un punct din fiecare cerință
- fară variabile globale
- datele membre private/protected
- fara headere specifice unui sistem de operare (<windows.h>)
- teste unitare pentru cerințele implementate (unde se poate, dacă nu apar probleme cu setup-ul de teste 😅)
- folosirea a funcționalităților limbajului fără sens
- folosirea a funcționlităților limbajului cu scopul de a încălca "legal" o altă regulă
    - folosirea excesivă a claselor friend
    - folosirea excesviă a elementelor statice  

## Tema 1

#### Cerințe
- [X] definirea a minim **2-3 clase** care sa interactioneze in cadrul temei alese (fie prin compunere, agregare sau doar sa apeleze metodele celeilalte intr-un mod logic) (5p)
  - pentru o clasă:
    - [X] constructori de inițializare
    - [X] constructor supraîncărcat
    - [X] constructori de copiere
    - [X] `operator=` de copiere
    - [X] destructor
    - [X] `operator<<` pentru afișare (std::ostream)
    - [X] `operator>>` pentru citire (std::istream)
    - [X] alt operator supraîncărcat ca funcție membră
    - [X] alt operator supraîncărcat ca funcție non-membră
  - pentru celelalte clase se va definii doar ce e nevoie
- [X] implementarea a minim 3 funcții membru publice pentru funcționalități specifice temei alese, dintre care cel puțin 1-2 funcții mai complexe (3p)
- nu doar citiri/afișări sau adăugat/șters elemente într-un/dintr-un vector 
- [X] scenariu de utilizare a claselor definite (1p):
  - crearea de obiecte și apelarea tuturor funcțiilor membru publice în main
  - vor fi adăugate în fișierul `tastatura.txt` DOAR exemple de date de intrare de la tastatură (dacă există); dacă aveți nevoie de date din fișiere, creați alte fișiere separat
- [X] opțiune pentru citirea și afișarea a n obiecte (1p)

### Tema 2

#### Cerințe
- [0] separarea codului din clase în `.h` (sau `.hpp`) și `.cpp` [(0.5p)](https://github.com/Ionnier/poo/tree/main/proiect/P01#separarea-implement%C4%83rii-metodelor-din-clase)
  * fiecare clasa un fișier separat (sau cum considerați mai corect, însă codul să fie cât mai modular)
- [X] cât mai multe `const` [(0.5p)](https://github.com/Ionnier/poo/tree/main/labs/L04#reminder-const-everywhere)
- [X] moșteniri [(5p)](https://github.com/Ionnier/poo/tree/main/labs/L04#exemplu):
  - [X] minim o clasă de bază și **2 clase derivate**
  - [X] încercați să derivați o clasă creată anterior
    - dacă nu reușiți
      - creați o altă clasă care poate fi integrată cu clasele anterioare
      - menționați de ce nu ați reușit și ce ați încercat
  - [X] ilustrați [upcast](https://github.com/Ionnier/poo/tree/main/labs/L04#solu%C8%9Bie-func%C8%9Bii-virtuale-late-binding)-ul și [downcast](https://github.com/Ionnier/poo/tree/main/labs/L04#smarter-downcast-dynamic-cast)-ul folosind funcții virtuale și pointeri la clasa de bază
    - aceasta va fi făcută prin **2-3** metode specifice temei alese
    - funcțiile pentru citire / afișare sau destructorul nu sunt incluse deși o să trebuiască să le implementați 
  - [X] apelarea constructorului din clasa de bază din [constructori din derivate](https://github.com/Ionnier/poo/tree/main/labs/L04#comportamentul-constructorului-la-derivare)
  - [X] suprascris [cc](https://github.com/Ionnier/poo/tree/main/labs/L04#comportamentul-constructorului-de-copiere-la-derivare)/op= pentru copieri/atribuiri corecte
  - [X] destructor [virtual](https://github.com/Ionnier/poo/tree/main/labs/L04#solu%C8%9Bie-func%C8%9Bii-virtuale-late-binding)
- [X] funcții și atribute `static` (în clase) [(1p)](https://github.com/Ionnier/poo/tree/main/labs/L04#static)
- [X] excepții [(1p)](https://github.com/Ionnier/poo/tree/main/labs/L04#exception-handling)
  - porniți de la `std::exception`
  - ilustrați propagarea excepțiilor
  - ilustrati upcasting-ul în blocurile catch
  - minim folosit într-un loc în care tratarea erorilor în modurile clasice este mai dificilă
- [X] folosirea unei clase abstracte (fie la exceptii, fie la moșteniri) [(0.5p)](https://github.com/Ionnier/poo/tree/main/labs/L04#clase-abstracte)
- [X] actualizarea meniului & scenariului de utilizare [(0.5p)](https://github.com/Ionnier/oop-template-t1/blob/main/main.cpp#L16)
- [X] citirea și afișarea a n obiecte [(0.5p)](https://github.com/Ionnier/oop-template-t1/blob/main/main.cpp#L13)
  - poate fi combinat cu demonstrarea upcasting-ului & downcast-ului printr-un vector către o clasă de bază
  - poate fi făcut oriunde (dacă aveți deja o clasă cu un vector, de exemplu o clasă Coș cu un vector<Produs>)
- [0] existența unui pull request către branch-ul în care lucrați ce include adăugarea unei noi derivate ce evidențiază că modificările aduse sunt minimale (0.5p)
  - derivata nu poate fi una ștearsă și rescrisă
  - derivata va avea date membre noi + o modificare de comportament pe una dintre funcțiile virtuale

### Tema 3

#### Cerințe
 - Clase template (2p)
   - [0] crearea unei ierarhii de clase template cu minim 2 clase
   - [0] ilustrarea RTTI pe clase template
   - [0] instanțieri cu logică a claselor create
 - STL (2p)
   - [0] utilizarea a două structuri (containere) diferite (fără vector)
   - [X] utilizarea a unui algoritm cu funcție lambda (de exemplu, sort, transform)
 - Design Patterns (2p)
   - [0] utilizarea a două șabloane de proiectare
 - Prezentare (4p)
   - [X] răspunsuri la întrebări din cod / generale C++
   - [X] explicarea a unei alte structuri sau a altui algoritm neutilizat (STL)
   - [X] explicarea a altor două șabloane de proiectare


## Recomandare Tema

* rezolvați tema 1 cu niște itemi generali ca să puteți extinde tema cu ușurință la următoarele teme.
  - coș de cumpărături + produse
  - sistem de validare a documentelor + documente de identitate
  - sistem de gestionare a biletelor + bilet 
* funcționalitatea creată să folosească metode ale obiectului generic 
* ar fi bine ca relația de agregare să fie făcută cu un obiect general în stilul celor de mai sus ^
* branch-uri + commit-uri punctuale
