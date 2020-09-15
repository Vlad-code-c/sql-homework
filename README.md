
## Tema pentru acasă

* ### Instrumente de instalare.  
  - Primul instrument necesar pentru instalarea sistemului de gestiune a bazelor de date *SSMS* este *serverul SQL*. Acesta este disponibil [aici](https://www.microsoft.com/en-us/sql-server/sql-server-downloads).  
  Acesta se va instala ca orice alta aplicatie pe calculator, alegand in prealabil locatia unde dorim sa o instalam.
  
  - In continuare, avem nevoie sa descarcam sgbd-ul propriu zis (in engleza SQL SERVER MANAGEMENT STUDIO -> SSMS), disponibil [aici](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver15&viewFallbackFrom=sql-server-2019).  
  La fel ca serverul, instalarea acestei aplicatii nu necesita explicatii, totul fiind simplu si comod.  
  
  - Dupa instalarea acestor doua aplicatii, in meniul Start vor aparea toate aplicatiile necesare pentru configurarea, lansarea si intretinerea serverului.
    
   ![Context Menu](/images/aplicatii_sgbd.png) 
   
   Pentru a incepe sa folosim sistemul de gesitune, vom lansa aplicatia  `Microsoft SQL server management studio 18`.  
   Dupa aparitia urmatoarei ferestre:  
   ![Connection window](/images/connection_window.png),  
   daca in campul Server Name se afla numele utilizatorului actual, apasam _Connect_. In caz contrar in campul Server Name apasam pe buttonul :arrow_down_small: -> `Browse for more...` -> `Database Engine` si selectam numele utilizatorului necesar.

* Instrumente de configurare.
` `
* Gestionarea rolurilor de utilizatori.
` `

* ### Securizarea bazei de date.
 Securitatea bazei de date este asigurata atat de catre structura acesteia, cat si de sistemul de gestiune pe care aceasta ruleaza. Sistemul de securitate al MSSS include urmatoarele elemnente principale:
  - Autentificarea
     In sistemul de gestiune MS SQL cuprinde doua subsisteme pentru conectarea la baza de date: `autentificarea Windows` - care este asigurata la nivel de sistem operational, si `securitatea SQL Server` - care necesita o autentificare suplimentara la server.
  - Rolurile
    Pentru a crea un utilizator nou, pot fi utilizate modul design sau modul prin comenzi sql.  
    Sintaxa comenzii sql este urmatoarea:  
    `CREATE LOGIN <login> WITH PASSWORD = <password>`  
    Pentru a crea un nou utilizator, utilizând Management Studio, din lista obiectelor serverului (Object Explorer) extindeţi ramura Security. După aceasta, tasta dreapta pe Logins şi alegeţi New Login. Se va deschide fereastra de dialog Login în care se completează datele necesare.
