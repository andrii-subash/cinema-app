# CINEMA_APP


## *Description*

#### The application that provides basic features of a movie theater and implements authentication, authorization and input validation.

---
## *Features*

#### Non-authenticated:
- Register new user

#### All-authenticated users:
- Get list of all cinema halls 
- Get list of sessions for given movie and day

#### Only for role USER:

- Retrieve user's shopping cart
- Add a ticket of given movie session to the shopping cart
- Complete (create) order from shopping cart
- Get user's order history

#### Only for role ADMIN:

- Get user's info [Only for ADMIN]
- Add new movie
- Add new cinema hall
- Add new movie session
- Update movie session with given id
- Delete movie session with given id

Feel free to change sample values in request bodies or params and test the app using Postman or similar tool.

---
## *Technologies*

- JDK v.17
- TomCat v.9.0.75
- Maven  
- MySQL  v.8.0.22
- Hibernate 5.6.14.Final for relational DB connection.
- Spring v.5.3.20 for dependency injection.
- Spring MVC v.5.3.20 to create RESTful endpoints. 
- Spring Security v.5.6.10 to implement authorization and authentication.

---
## *Application run*

1. Clone this repository to your local machine using git clone.
2. Ensure that you have Java, Apache Tomcat and any relational DB management system (like MySQL) installed on your system.
3. Configure the database settings in src/main/resources/db.properties.
4. Build the application using mvn package.
5. In Tomcat configuration in field "Deployment directory" specify path to directory cinema-app, in field "Use classpath of module" specify this directory too, and specify "/" in "Context path"
6. Start Tomcat by running the startup.sh (or startup.bat on Windows) script in the bin/ directory of your Tomcat installation.
7. Use Postman or similar tool to test the endpoints.

