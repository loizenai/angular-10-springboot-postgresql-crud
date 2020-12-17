SpringBoot + Angular 10 + PostgreSQL CRUD Example

https://loizenai.com/springboot-angular-10-postgresql-crud-restapi-example/

![SpringBoot + Angular 10 + PostgreSQL CRUD Example](https://loizenai.com/wp-content/uploads/2020/08/SpringBoot-Angular-10-PostgreSQL-CRUD-RestAPIs-Example.png)

In the tutorial, I introduce how to create an “SpringBoot + Angular 10 + PostgreSQL CRUD RestAPIs Example” with POST/GET/PUT/DELETE requests:

– Design overview system with an Architecture Diagram that includes: Angular 10 Client, SpringBoot RestAPIs, and PostgreSQL database.
– Implement Angular 10 CRUD Client with Angular built-in HttpClient to communicate with server side.
– Implement SpringBoot RestAPIs that gets data from PostgreSQL using Spring Data JPA and returns back data as Json format to requested Angular 10 Client.

## Overview Example – How to build SpringBoot Angular 10 PostgreSQL CRUD RestAPIs Example?

![SpringBoot + Angular 10 + PostgreSQL CRUD RestAPIs Example Application – Architecture](https://loizenai.com/wp-content/uploads/2020/08/SpringBoot-Angular-10-PostgreSQL-CRUD-RestAPIs-Example-Application-Architecture-Diagram.png)

- We build a backend SpringBoot CRUD RestAPIs with Spring Data JPA for POST/GET/PUT/DELETE data and store them in PostgreSQL database.
- We implement Angular 10 Application that use Angular HTTPClient to do CRUD requests(call/receive requests) with SpringBoot backend and display data on view.

## SPRINGBOOT DESIGN – FLOW: SPRINGBOOT – POSTGRESQL

![SPRINGBOOT DESIGN – FLOW: SPRINGBOOT – POSTGRESQL](https://loizenai.com/wp-content/uploads/2020/08/SpringBoot-PostgreSQL-CRUD-RestAPIs-Architecture-Diagram.png)

- For building RestAPIs in SpringBoot application, We use Spring MVC Web.
- For interacting with PostgreSQL, We use Spring Data JPA.
- We implement RestAPI’s URL in RestAPIController.java file to process bussiness logic.
- For manipulating PostgreSQL’s records, we define a JPA model for mapping field data and use a Spring Data JPA repository to do CRUD operation with PostgreSQL database.

## SpringBoot Project Structure

![SpringBoot Project Structure](https://loizenai.com/wp-content/uploads/2020/08/SpringBoot-CRUD-RestAPIs-Project-Structure.png)

- models package defines Customer model and Message response class.
- repository package defines Spring Data JPA repository class CustomerRepository to do CRUD operation with database.
- service package defines a middleware class CustomerServices between Controller and Repository.
- controller package defines a RestAPI Controller RestAPIController to handle POST/GET/PUT/DELETE request.

## ANGULAR 10 CRUD DESIGN – FLOW: ANGULAR – SPRINGBOOT RESTAPIS

![ANGULAR 10 CRUD DESIGN – FLOW: ANGULAR – SPRINGBOOT RESTAPIS](https://loizenai.com/wp-content/uploads/2020/08/Angular-10-CRUD-RestAPI-Application-Frontend-Architecture-Diagram.png)

Angular 10 CRUD Application is designed with 3 main layers:

- Service Layer is used to define Angular Common Services and HttpClient Services to interact with RestAPIs
- Component Layer is used to define Angular Components to show views in Browser for interacting with Users
- Router Layer is used to route URLs mapping with the corresponding Angular Components

## Angular 10 Project Structure

![Angular 10 Project Structure](https://loizenai.com/wp-content/uploads/2020/08/Angular-10-CRUD-Application-Project-Structure.png)

Angular 10 CRUD Application defines 3 components, 2 services, 1 routers, and 2 data models:

– Components:

add-customer component is used to add a new customer to system
list-customer component is used to show all customers on view pages, delete a customer and update a customer
message component is used to define a view to show logging message on browser
– Services:

customer.service.ts defines POST/GET/PUT/DELETE HTTP requests to SpringBoot RestAPIs with the built-in Angular HttpClient.
message.service.ts defines an array storage to log all messages when Angular CRUD App running

– Router: app-routing.module.ts defines how to map a corresponding Angular component with an URL.

– Models:

customer.ts defines the main data model of our application.
message.ts defines the response data model between SpringBoot and Angular application.

## Goal Project: Angular 10 + SpringBoot + PostgreSQL

– Add new Customer:

![Add new Customer](https://loizenai.com/wp-content/uploads/2020/08/Angular-10-CRUD-Application-Post-a-Data-to-Backend-SpringBoot.png)

– List All Customers:
![– List All Customers](https://loizenai.com/wp-content/uploads/2020/08/Angular-10-CRUD-Application-List-all-records-from-PostgreSQL-via-SpringBoot-server.png)

– Details a Customer:

![– Details a Customer:](https://loizenai.com/wp-content/uploads/2020/08/Angular-10-CRUD-App-get-a-Record-with-the-given-ID-from-PostgreSQL-via-SpringBoot-Server.png)

– Update a Customer:

![– Update a Customer:](https://loizenai.com/wp-content/uploads/2020/08/Angular-10-CRUD-Application-Update-a-data-with-a-given-id-to-PostgreSQL-via-SpringBoot-server.png)

– Delete a Customer:

![Delete a Customer](https://loizenai.com/wp-content/uploads/2020/08/Angular-CRUD-App-Delete-a-record-with-a-given-id-from-PostgreSQL-via-SpringBoot-backend.png)


– Check database records:

![Check database records](https://loizenai.com/wp-content/uploads/2020/08/Check-PostgreSQL-database-after-do-Angular-CRUD-requests.png)
## SpringBoot PostgreSQL RestAPIs – Backend Development

![SpringBoot PostgreSQL RestAPIs – Backend Development](https://loizenai.com/wp-content/uploads/2020/08/SpringBoot-PostgreSQL-CRUD-RestAPIs-Architecture-Diagram-1.png)

## Related post

- [Spring Boot Security JWT Authentication Example](https://loizenai.com/spring-boot-security-jwt-authentication-example-mysql-postgresql-spring-jpa-restapis/)
- [Angular Spring Boot JWT Authentication Example](https://loizenai.com/spring-boot-security-jwt-authentication-example-mysql-postgresql-spring-jpa-restapis/)
- [Angular Django CRUD RestAPIs Application Examples](https://loizenai.com/spring-boot-security-jwt-authentication-example-mysql-postgresql-spring-jpa-restapis/)
- [SpringBoot RestAPIs Upload Download Multiple CSV files to MySQL/PostgreSQL](https://loizenai.com/springboot-restapi-upload-download-multiple-csv-files-to-mysql-postgresql-database-with-ajax-restclient/)
