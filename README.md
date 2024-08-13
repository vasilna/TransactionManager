# TransactionManager backend
Simple spring boot project for transactions and accounts with basic JWT authentication which support two roles

# How to run:

1. Open backend folder with Intelij

2. Open workbench or other Mysql visual tool for database architect.

3. Create schema called transactionmanager

4. Create query, type `use transactionmanager` and execute query

5. Create query for every file in folder database, copy all the content, paste it and execute the query

7. When you executed all of the files in database folder go to `src/main/resources/application.properties` and open it

8. Change `spring.datasource.username=?` and `spring.datasource.password=?` where `?` is your Local Mysql Connection username in the first case and you Local Mysql Connection password in the second case

9. Go back to your project and run it

10. If you want to test functionalities via swagger type `http://localhost:8080/swagger-ui/index.html#/` and start testing

11 When you try to test it will prompt you to enter your username and password. Type `vasko` for username and `nasko` for password and enjoy

# Functionalities

1. You can add or remove account or search account by its id or name

2. You can create a transaction between two accounts but you have to fill fields in json and after that to execute

3. You can list all transactions of a given source account

3. You can see transactions of an account listed in a pdf, excel file or to return in zip format

4. You can search account with one or two mistakes in the name with searchEngine functionality

5. Account searching uses cache proxy so if account is loaded it will return it to you much faster

6. You can register user, login and logout

7. The security is with httpBasic login and with jdbc authentication, the encryption of the password is with BcryptPasswordEncoder

8. There are different roles and every one of them can have list of authorities.
