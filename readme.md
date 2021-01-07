# Demo-Spring-Boot-Api
Generate a Maven Project with Java and Spring Boot: [Spring Initializr](https://www.start.spring.io)
* versions: pom.xml :)
***

Dependencies:
* JPA
* Rest Repositories
* Rest Repositories HAL Browser
* H2 database
***
Generate: 
* Essentielle.java
@Entity
* RestRepository @RepositoryRestResource
***
localhost:8080//essentielles
***
Resources:
* application.properties:
```spring.datasource.url=jdbc:h2:mem:Essentielles```
* data.sql:
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

API Documentation:
* POST /essentielles
* GET /essentielles/{essentielleId}
* PUT /essentielles/{essentielleId}
* DELETE /essentielles/{essentielleId}

