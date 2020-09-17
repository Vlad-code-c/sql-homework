## Procesul de creare a unui utilizator in MSSMS

### Crearea unui login
Pentru a crea un login, selectam Security > Logins  
![New Login](/users/images/new_login.png)  

In urmatoarea fereastra introducem:
 - Login Name
 - Selectam SQL Server autentification
 - Selectam o parola
 - Apasam OK
  
![Credentials](/users/images/credentials.png)  

Login-ul e creat  
![Login](/users/images/login_is_created.png)  

Deasemenea, putem crea un login si cu comanda   
`CREATE LOGIN MyLogin WITH PASSWORD = '123'`


### Crearea unui utilizator
- Identificam baza de date pentru care dorim sa creem utilizatori
- Selectam folderul Security
- Click-dreapta > New > User...

![create_user](/users/images/create_user.png)  

In continuare introducem numele utilizatorului si numele login-ului creat anterior
Apasam OK
![credentials_user](/users/images/credentials_user.png)  


Utilizatorul este creat  
![user_is_created](/users/images/user_is_created.png)  


Deasemenea, putem crea un utilizator folosind comanda  
`create user <user-name> for login <login-name>`
