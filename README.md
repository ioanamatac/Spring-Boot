# Demo-Spring-Boot-Api
***


<a name="general info"></a>
<a name="technologies"></a>
<a name="installation"></a>
<a name="side information"></a>

## General Info

Maven Project [Spring Initializr](https://www.start.spring.io)


## Technologies

* Java  1.8
* Spring  2.3.2

## Installation
 
* git clone https://github.com/ioanamatac/demo_spring_boot_API.git
* maven install
* run as java application
* http://localhost:8080/essentielles

## Side Information

Dependencies:
* JPA
* Rest Repositories
* Rest Repositories HAL Browser
* H2 database

***

Model class and an interface: 
* Essentielle.java @Entity

* RestRepository.java @RepositoryRestResource

***
Resources file:
* application.properties :

```SQL 
spring.datasource.url=jdbc:h2:mem:Essentielles
```

* data.sql :

```SQL
INSERT INTO Essentielle(name, quantite, prix) VALUES ('Promenade En Foret', 30, 9.37);
INSERT INTO Essentielle(name, quantite, prix) VALUES ('Energie Positive', 30, 9.37);
INSERT INTO Essentielle(name, quantite, prix) VALUES ('Ylang Ylang', 5.10, 6.64);
INSERT INTO Essentielle(name, quantite, prix) VALUES ('Lemongrass Bio', 5.10, 6.64);
INSERT INTO Essentielle(name, quantite, prix) VALUES ('Cocooning', 30, 9.37);
INSERT INTO Essentielle(name, quantite, prix) VALUES ('Encens', 5, 9.41);

COMMIT;
```
***
 
 
 http://localhost:8080/browser/index.html#
 
***
 

API Documentation:
* POST /essentielles
* GET /essentielles/{essentielleId}
* PUT /essentielles/{essentielleId}
* DELETE /essentielles/{essentielleId}


