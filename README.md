<h1 align="center">Student-Setup</h1>
<h3 align="center">Setup-ul presupune utilizarea sistemului de operare Windows</h3>

Pentru a rula si rezolva laboratoarele este obligatorie instalarea urmatoarelor programe si urmarea instructiunilor ce se regasesc in acest README.md. Pentru orice neclaritati in urmarea pasilor se recomanda intrebarea pe forumul Student-Setup de pe moodle.

Programele necesare sunt:
 - [MinGW](https://sourceforge.net/projects/mingw/) - set de programe ce emuleaza ecosistemul Linux pe Windows
 - [VS Code](https://code.visualstudio.com/) - editor de cod recomandat, ce permite folosirea unor extensii utile in dezvoltarea software

 Dupa instalarea MinGW se vor selecta urmatoarele pachete din interfata grafica a programului:
 <img src="./resources/minGW.jpg">
Dupa selectarea acestor pachete se va apasa pe butonul Instalation -> Apply Changes si se va astepta instalarea acestora.


Dupa instalarea acestor se vor edita variabilele de sistem (environment variables) si se vor adauga path-urile catre fiserele bin ale minGW.
Daca instalarea sa facut fara a modifica path-ul propus de installer atunci urmatoarele path-uri sunt cele dorite:
```
C:\MinGW\bin
C:\MinGW\msys\1.0\bin
```

<img src="./resources/envp2.jpg">
Path-urile de mai sus vor fi introduse in variabila de sistem Path prin selectarea variabilei Path si apasarea pe butonul Edit...
<img src="./resources/envp3.jpg">

