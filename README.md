<h1 align="center">Student-Setup</h1>
<h3 align="center">Setup-ul presupune utilizarea sistemului de operare Windows</h3>

Pentru a rula si rezolva laboratoarele este obligatorie instalarea urmatoarelor programe si urmarea instructiunilor ce se regasesc in acest README.md. Pentru orice neclaritati in urmarea pasilor se recomanda intrebarea pe forumul Student-Setup de pe moodle.

Programele necesare sunt:
 - [MinGW](https://sourceforge.net/projects/mingw/) - set de programe ce emuleaza ecosistemul Linux pe Windows
 - [VS Code](https://code.visualstudio.com/) - editor de cod recomandat, ce permite folosirea unor extensii utile in dezvoltarea software

 Dupa instalarea MinGW se vor selecta urmatoarele pachete din interfata grafica a programului:
 <img src="./resources/minGW.jpg">
Dupa selectarea acestor pachete se va apasa pe butonul Instalation -> Apply Changes si se va astepta instalarea acestora.

Dupa instalarea acestor se vor edita variabilele de sistem (environment variables) si se vor adauga path-urile catre fiserele bin ale minGW. ( Pentru a accesa optiunea trebuie sa scrieti in meniul de start al Windows-ului 'env' si sa selecati optiunea de mai jos, accesarea meniului de start Windows se face prin apasarea pe butonul cu simbolul windows de la tastatura )
<img src="./resources/envp0.jpg">
Daca instalarea sa facut fara a modifica path-ul propus de installer atunci urmatoarele path-uri sunt cele dorite:

``` 
C:\MinGW\bin
C:\MinGW\msys\1.0\bin
```

<img src="./resources/envp2.jpg">
Path-urile de mai sus vor fi introduse in variabila de sistem Path prin selectarea variabilei Path si apasarea pe butonul Edit...
<img src="./resources/envp3.jpg">

Pentru a testa ca procesul a reusit scrieti in terminalul windows cmd comanda ```g++```, daca obtineti un mesaj similar cu cel de jos inseamna ca Windows-ul  reusit sa gaseasca programul ```g++``` dar ca nu a primit un fiiser pe care sa il compileze :

``` 
C:\Users\gabriel.rusu\Desktop\student-setup>g++
g++: fatal error: no input files
compilation terminated.
```

## FAQ:

### La ce ma ajuta acest setup ?

Acest setup are rolul de a va ajuta sa rulati testele unitare aferente fiecarui schelet de laborator.

### Ce este schelet-ul de laborator ?

In fiecare saptamana veti primi un nou schelet de laborator ce are ca scop introducerea studentilor in notiunile predate la curs intr-un mod practic.

Se numeste schelet de laborator deoarece voi va trebuii sa completati logica functiilor descrise in schelet fara a trebuii sa scrieti un program functional de la 0 in fiecare saptamana.

### Ce sunt testele unitare ?

Testele unitare sunt un set de teste ce au rolul de a apela functiile scrise de voi si de a determina daca acestea ruleaza corect.

In cazul in care s-a implementat ceva gresit testul va semnaliza acest lucru in consola

### Cum rulez scheletul ?

Odata descarcat scheletul laboratorului din saptamana respectiva deschideti un terminal in folder-ul sheletului de laborator si rulati comanda pentru a testa programul

``` 
make test
```

### Ce incarc pe moodle ?

Pe Moodle va trebuii incarcat doar folder-ul src ce contine tot codul sursa la care ati lucrat.

Se recomanda trimiterea folderului intr-o arhiva .rar/.zip
