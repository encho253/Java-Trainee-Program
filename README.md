# Java Trainee Program:

# ITERATION 1

## Servlet/JSP
- [Servlet/JSP Documentation](https://docs.oracle.com/javaee/6/tutorial/doc/bnafd.html)
- Servlet, Filter, Listeners + 3 scopes/contexts
- Annotations vs. `web.xml`
- WAR file structure
- Maven file structure for WAR packaging
- JSP, Tag Libraries, JSTL:
  - [JSP Documentation](https://docs.oracle.com/javaee/5/tutorial/doc/bnagx.html)
  - [Tag Libraries & JSTL](https://docs.oracle.com/javaee/5/tutorial/doc/bnakc.html)

## Maven
- [Maven Documentation](https://maven.apache.org/guides/getting-started/index.html)
- [Build Lifecycle](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html)
- [Standard Directory Layout](https://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html)
- [Dependency Mechanism](https://maven.apache.org/guides/introduction/introduction-to-dependency-mechanism.html)
- [Repositories](https://maven.apache.org/guides/introduction/introduction-to-repositories.html)
- [Plugins Configuration](https://maven.apache.org/guides/mini/guide-configuring-plugins.html)

## Web Technologies
- [URI - Uniform Resource Identifier](https://www.techtarget.com/whatis/definition/URI-Uniform-Resource-Identifier)
- [HTTP Overview](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview)

## Tasks
1. **Tomcat Setup:**
   - Download and set up the appropriate Tomcat version.
   - Add it as a server to Eclipse.
2. **Clone and Upgrade Servlet/JSP Demo:**
   - Clone the repository: [Servlet JSP Demo](https://github.com/hrabur/servlet-jsp-demo).
   - Fix and upgrade to the latest Servlet API.
   - Solve the tasks described on the index page.
3. **Create Hangman Application:**
   - Store ongoing games in memory using only Servlet API + JSP/JSTL for the view.

## Suggested Resources
- [Possible Literature](https://github.com/hrabur/web-programming-course/wiki)

## Tools
- **Eclipse:** [Download Eclipse](https://www.eclipse.org/downloads/download.php?file=/technology/epp/downloads/release/2024-06/R/eclipse-jee-2024-06-R-win32-x86_64.zip)
- **SonarLint:** Available from the Eclipse Marketplace
- **Google Java Format Eclipse Plugin:** [GitHub Repository](https://github.com/google/google-java-format#eclipse)
  - [Google Java Style Guide for Eclipse](https://github.com/google/styleguide/blob/gh-pages/eclipse-java-google-style.xml)
  - Enable format and other save actions
- **Tomcat:** [Download Tomcat](https://dlcdn.apache.org/tomcat/tomcat-10/v10.0.13/bin/apache-tomcat-10.0.13.zip)
- **DBeaver:** [Download DBeaver](https://dbeaver.io/files/dbeaver-ce-latest-win32.win32.x86_64.zip)
- **TortoiseGit:**
  - [Download TortoiseGit](https://download.tortoisegit.org/tgit/2.12.0.0/TortoiseGit-2.12.0.0-64bit.msi)
  - [Prerequisites](https://tortoisegit.org/support/faq/#prerequisites)
- **VS Code:** [Download VS Code](https://code.visualstudio.com/#)

# ITERATION 2
### Spring Core Topics Overview

1. **Spring Core**  
   - [Documentation](https://docs.spring.io/spring-framework/docs/current/spring-framework-reference/core.html#spring-core)
   - **Design Patterns Used in Spring:**
     - **Dependency Injection (DI) & Inversion of Control (IoC)**
     - **Proxy Pattern (Посредник)**

2. **Spring Beans and Their Life Cycle**  
   - [Documentation](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans)
   - **Ways to Turn POJO into a Spring Bean:**
     - Annotation
     - XML
     - Java Config, etc.
   - **Spring Application Context Life Cycle and Spring Bean Life Cycle**

3. **Dependency Injection Types Supported by Spring**  
   - [Documentation](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans-annotation-config)

4. **Resolving Missing Dependencies and Interface Implementations**  
   - [Documentation:](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans-autowired-annotation-primary)  
     [Primary Annotation](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans-autowired-annotation-primary)  
     [Qualifier Annotation](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans-autowired-annotation-qualifiers)  
     [Generics as Qualifiers](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans-generics-as-qualifiers)

5. **Java Configuration**  
   - [Documentation](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans-java)

6. **Classpath Scanning**  
   - [Documentation](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans-classpath-scanning)

7. **AOP in Spring**  
   - Covers both AspectJ and Spring AOP style approaches.

8. **Building a Pure Spring Core Application**  
   - Demonstrate dependency injection, AOP, classpath scanning, etc., without using Spring Boot.

9. **Unit Testing with JUnit 5, AssertJ, and Mockito**  
   - [JUnit 5 + AssertJ](https://assertj.github.io/doc/)  
   - [Mockito](https://site.mockito.org/)

- For configuring the Google Java Format Eclipse plugin with Java 16+, consult with Buddy on how to configure the `eclipse.ini` file.

# ITERATION 3
### Main Objectives

1. **Mastering Spring MVC**
   - Understand and implement core concepts: [Spring MVC Overview](https://docs.spring.io/spring-framework/docs/current/spring-framework-reference/web.html#spring-web)
   - Work with Annotated Controllers: [Annotated Controllers](https://docs.spring.io/spring-framework/docs/current/spring-framework-reference/web.html#mvc-controller)
   - Explore Handler Methods: [Handler Methods](https://docs.spring.io/spring-framework/docs/current/spring-framework-reference/web.html#mvc-ann-methods)
   - Learn Data Binding and Validation: [Bean Validation](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#validation-beanvalidation)
   - Implement Exception Handling and Controller Advice
   - Configure the DispatcherServlet for handling requests

### Secondary Objectives

1. **Integration Testing**
   - Set up and conduct integration testing using JUnit, Selenium, WebDriver, and the PageObject pattern.
   - Gain proficiency with XPath and CSS selectors.
   - Utilize the Spring MVC testing framework: [Spring MVC Test](https://docs.spring.io/spring-framework/docs/current/spring-framework-reference/testing.html#spring-mvc-test-framework)

### Practical Goals

1. **Refactoring and Testing**
   - Refactor a Servlet-based UI to use Spring MVC by configuring the DispatcherServlet.
   - Implement Exception Handling, Data Binding, and Validation.
   - Write UI integration tests using Selenium and WebDriver.
   - Replace the XML configurations


# ITERATION 4
### **Official Documentation**
- [Spring Boot Reference Guide](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/)
- [API Best Practices (PayPal API Standards)](https://github.com/levid-gc/paypal-api-standards/blob/master/api-style-guide.md)

---

## **Tasks Overview**

### **Primary Goal: Master Spring Boot**

1. **Getting Familiar with Spring Boot**
   - **Objective**: Understand the core features of Spring Boot.
   - [Spring Boot Features](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#features)
   
2. **Naming Conventions & Code Structure**
   - **Objective**: Organize code following best practices, focusing on packages per layer and per feature.
   - [Code Structuring Best Practices](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#using.structuring-your-code)

3. **Auto-Configuration**
   - **Objective**: Learn how Spring Boot automatically configures components to reduce boilerplate code.
   - [Auto-Configuration](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#using.auto-configuration)

4. **Embedded Container**
   - **Objective**: Understand how Spring Boot uses an embedded web server for running web applications.
   - [Embedded Container](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#features.developing-web-applications.embedded-container)

5. **Spring Boot and Spring MVC**
   - **Objective**: Learn how Spring Boot integrates with Spring MVC to build web applications.
   - [Spring MVC Integration](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#features.developing-web-applications.spring-mvc)

6. **Spring Boot Application Configuration**
   - **Objective**: Learn how to configure a Spring Boot application using external configuration files.
   - [External Configuration](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#features.external-config)
   - [Properties & Configuration](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#howto.properties-and-configuration)

---

### **Secondary Goal: Docker Integration**

1. **Understanding Docker**
   - **Objective**: Gain basic understanding of how Docker works for containerizing applications.
   - **Key Concepts**:
     - `docker pull`: Pull an image from a registry.
     - `docker run`: Run a container from an image.
     - `docker start/stop/restart`: Manage container lifecycle.

2. **Dockerfile Best Practices**
   - **Objective**: Learn how to create a Dockerfile for containerizing applications.
   - [Comparing Containerization Methods](https://cloud.google.com/blog/topics/developers-practitioners/comparing-containerization-methods-buildpacks-jib-and-dockerfile)

3. **Spring Boot & Docker**
   - **Objective**: Learn how Spring Boot integrates with Docker to create containerized applications.
   - [Spring Boot & Container Images](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#features.container-images)
   - [Testing with Docker (Testcontainers)](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#howto.testing.testcontainers)

---

### **Practical Task**

- **Objective**: Refactor an existing Hangman game project to use Spring Boot and Docker.
  
1. **Refactor Hangman Game with Spring Boot**
   - **Task**: Remove all manual configurations and replace them with Spring Boot’s auto-configuration and `application.yml`.

2. **Build a Docker Image**
   - **Task**: Create a Dockerfile, build a Docker image for the refactored application, and run the application from the Docker image.

---

### **Additional Resources**
- [API Best Practices (PayPal API Standards)](https://github.com/levid-gc/paypal-api-standards/blob/master/api-style-guide.md)

---

# Iteration 5

#### SQL
- **DDL (Data Definition Language)**
  1. Create table
  2. Alter table
  3. Drop table, etc.
  
- **DML (Data Manipulation Language)**
  1. **Select**:
     - Inner Join
     - Left Join
     - Right Join
     - Group By + Having
     - In Clause
  2. **Update**
  3. **Insert**

#### JPA/Hibernate
- **JPA Annotations:**
  - Mapping Bean to Entity using annotations
  - Implementing relationships: One-to-one, One-to-many, Many-to-many (Annotations, etc.)
  - Inheritance Strategies (3 strategies: JOINED, TABLE_PER_CLASS, SINGLE_TABLE)
  
- **DAO/Repository Pattern:**
  - Each Entity should have its own DAO.
  - **CrudDao**: Hand-crafted DAO with operations like `get()`, `listAll()`, `create()`, `delete()`, `update()`.
  - Using **EntityManager** to implement CRUD operations and specific queries.
  
- **Hibernate Criteria API**:
  - [Tutorial](https://www.tutorialspoint.com/hibernate/hibernate_criteria_queries.htm)
  
- **JPA Type-Safe Query API:**
  - [Tutorial](https://www.tutorialspoint.com/jpa/jpa_criteria_api.htm)
  - [JPA Metamodel](https://www.baeldung.com/hibernate-criteria-queries-metamodel)
  
- **HQL and JPQL**:
  - Outside the scope of this iteration; just for reference.

#### Spring Data
- **CRUD Operations:**
  - Simplify CRUD using conventions.
  
- **Custom Queries:**
  - Create custom queries using conventions.
  
- **Spring Data Specifications + JPA Criteria Query**:
  - [Guide](https://www.baeldung.com/spring-data-criteria-queries#specifications)
  
- **(Secondary Goal)**: DB Migrations with Flyway:
  - Schema versioning and migrations using Flyway.

---

### Practical Task

#### Project: Add Persistence Layer to the Hangman Game

1. **Database Implementation:**
   - Store ongoing and completed games in a **MariaDB** database (instead of in-memory storage).
   - Implement **GameRepository** using the **DAO Pattern** with a custom **CrudDao**.

2. **Game Statistics:**
   - Add a statistics table to store data for each completed game (One-to-One relation with Game entity).

3. **Ranking System:**
   - Create a separate ranking table with a **One-to-Many** relation to the statistics table.
   - Implement a **RankingService** to update rankings when a game ends.

4. **Spring Data Integration:**
   - Use Spring Data to manage **Stats** and **Rank** entities.
   - **Rank Page**: 
     - Display Top 10 players ever using Spring Data conventions.
     - Display Top 10 players in the last 30 days using **Spring Data Specifications**.

5. **Flyway Migrations:**
   - Initialize the database schema with Flyway.
   - Add mock data for statistics and rankings during the migration process.


# Iteration 6 - Web Services

### Main Goal

Web Services operate on a **stateless model** like the HTTP protocol, with two distinct sides:
- **Client (Consumer)**: the active, calling side
- **Server (Producer)**: the listening, responding side

Web Services, being machine-to-machine interfaces (unlike UI, which is human-to-machine), require:
- A **well-defined contract**: includes how to call the service, input parameters, expected outputs, etc.
- **Easy-to-parse structures**: standardized formats like XML or JSON.

There are two primary approaches to defining a web service:

#### 1. **Contract-First**
   - Commonly used for **SOAP** web services, where the contract is described in a **WSDL** file (an XML format).
   - In **REST** services, contracts are often provided in **OpenAPI** format (JSON), but documentation is often in English for easier understanding.

#### 2. **Code-First**
   - More common for **producers** (servers), where developers write code based on business requirements, and the contract or documentation is generated by a framework.

**Versioning and Backward Compatibility**  
Both **SOAP** and **REST** support versioning, and backward compatibility is crucial for evolving services. For better compatibility on the consumer side, consider using the **Tolerant Reader** pattern ([Martin Fowler’s Tolerant Reader](https://martinfowler.com/bliki/TolerantReader.html)).

### SOAP

- **SOAP Basics**: Learn the fundamentals of **SOAP, WSDL, and XSD**. Refer to [Guru99’s SOAP Tutorial](https://www.guru99.com/soap-simple-object-access-protocol.html).
- **JAX-WS and Apache CXF**: Explore JAX-WS, a Java API for SOAP, commonly implemented with **Apache CXF** ([Baeldung: JAX-WS](https://www.baeldung.com/jax-ws)).
- **JAXB**: Get familiar with JAXB, a Java framework for working with XML ([Oracle JAXB Documentation](https://docs.oracle.com/javase/tutorial/jaxb/intro/)).

### REST

- **REST Principles**: Study the principles of REST, including the HATEOAS maturity model and guidelines like **PayPal's API Standards** ([PayPal API Standards Guide](https://gitlab.sc.proxiad.bg/e.enevski/java-trainee-program/-/blob/main/paypal-api-standarts.md)).
- **OpenAPI and JSON Schema**: Review the OpenAPI standard and JSON Schema ([OpenAPI Documentation](https://oai.github.io/Documentation/start-here.html)).
- **Jackson and JSON-B**: For JSON parsing in Java, explore **Jackson** ([Jackson Databind](https://github.com/FasterXML/jackson-databind)) and **JSON-B** ([Baeldung: JSON-B](https://www.baeldung.com/java-json-binding-api)).

- **Swagger/OpenAPI with Springfox/Spring Docs**: Learn to use Swagger/OpenAPI for auto-documentation. Try integrating **Spring Docs** for REST APIs ([Spring Docs](https://springdoc.org/)).

---

### [Richardson Maturity Model](https://medium.com/@rojasjimenezjosea/rest-api-maturity-model-a3664747bf3b)

The **Richardson Maturity Model** categorizes RESTful services based on their adherence to REST principles, focusing on resources, HTTP verbs, and **HATEOAS** (Hypermedia as the Engine of Application State). Each level represents a step toward a more complete RESTful service:

- **Level 0: URI-Based Service**
  - **Description**: Single URI endpoint, often only uses **POST** requests for all actions.
  - **Example**: A service with a single endpoint, `/api/service`, where all actions (create, read, update, delete) occur through this single URL.

- **Level 1: Resource-Based Service**
  - **Description**: Introduces resources with individual URIs for different entities, but actions are not differentiated by HTTP verbs.
  - **Example**: Separate URIs like `/api/products` and `/api/orders`, but uses **POST** for all actions on these resources.

- **Level 2: HTTP Verbs**
  - **Description**: Differentiates actions on resources using HTTP verbs such as **GET**, **POST**, **PUT**, and **DELETE**.
  - **Example**: An endpoint like `GET /api/products/{id}` fetches details for a specific product, while `DELETE /api/products/{id}` deletes it.

- **Level 3: HATEOAS (Hypermedia Controls)**
  - **Description**: Implements HATEOAS by including hypermedia links in responses, allowing clients to dynamically discover and interact with available actions.

- **Detailed Example for HATEOAS (Level 3)**: For a `GET /api/products/1` endpoint:
  - **Level 2**: Returns the product details in JSON format:
    ```json
    {
      "id": 1,
      "name": "Product 1",
      "price": 10.99
    }
    ```
  - **Level 3**: In addition to the details, it includes hypermedia links to guide the client on possible actions, making the API more self-descriptive:
    ```json
    {
      "id": 1,
      "name": "Product 1",
      "price": 10.99,
      "links": [
        {
          "rel": "self",
          "href": "/api/products/1",
          "method": "GET",
          "description": "Retrieve this product"
        },
        {
          "rel": "update",
          "href": "/api/products/1",
          "method": "PUT",
          "description": "Update this product"
        },
        {
          "rel": "delete",
          "href": "/api/products/1",
          "method": "DELETE",
          "description": "Delete this product"
        }
      ]
    }
    ```

---

### Secondary Goal

**Writing Integration Tests**:
- **For SOAP**: Use the WSDL from the producer and generate a consumer using **wsimport** ([wsimport Maven Plugin](https://www.mojohaus.org/jaxws-maven-plugin/wsimport-mojo.html)), and test using **JUnit 5** and **AssertJ**.
- **For REST**: Use Swagger UI documentation and write integration tests with **JUnit 5**, **Spring WebClient** (deprecated, but included for reference), **Rest Assured** ([Rest Assured on GitHub](https://github.com/rest-assured/rest-assured)), and **AssertJ**.

---

### Practical Task

1. **SOAP Endpoint for Hangman Statistics**
   - Integrate **Apache CXF** with the Hangman app (use the latest **Spring Boot** with **JPA/Hibernate**).
   - Expose game statistics as a SOAP endpoint ([Apache CXF Spring Boot Starter Guide](http://cxf.apache.org/docs/springboot.html#SpringBoot-SpringBootCXFJAX-WSStarter)).
   - Look into CXF auto-configuration to understand its Spring integration.

2. **REST API for Hangman Game Functionality**
   - Follow [PayPal’s API Standards Guide](https://gitlab.sc.proxiad.bg/e.enevski/java-trainee-program/-/blob/main/paypal-api-standarts.md) for REST API design.
   - Integrate **Spring Docs** to auto-document the REST APIs ([Spring Docs](https://springdoc.org/)).

3. **Integration Tests for SOAP and REST APIs**
   - **SOAP Tests**: Write integration tests for the SOAP endpoint using JUnit 5 and AssertJ.
   - **REST Tests**: Write integration tests for REST endpoints, utilizing both **WebClient** and **Rest Assured** to practice various testing approaches.

---

4. ### Enhance an Existing REST Endpoint to Implement HATEOAS

**Objective**: Modify an existing RESTful endpoint to adhere to **Level 3** of the Richardson Maturity Model by including **HATEOAS** links in its responses. This will provide clients with hypermedia links for related actions on the resource.

**Task Details**:

1. **Identify the Endpoint to Enhance**  
   Select an existing endpoint (for example, `GET /api/orders/{id}`) that retrieves a resource, like an order.

2. **Modify Response Structure**  
   - Ensure that the existing endpoint's response includes **HATEOAS links** for guiding clients on possible next actions.
   - This enhances the client’s ability to interact with other related resources seamlessly.

3. **Add HATEOAS Links**  
   Add links based on actions the client may need to perform, such as:
   - `PUT /api/orders/{id}` to update the order.
   - `DELETE /api/orders/{id}` to cancel the order.
   - `GET /api/orders/{id}/status` to retrieve the current order status.
   - `POST /api/orders/{id}/items` to add items to the order.

4. **Implementation Steps**  
   - Utilize **Spring HATEOAS** or similar library to generate links in the response dynamically.
   - Ensure each link includes a **rel** attribute, such as `"update"`, `"delete"`, `"status"`, and `"add-item"`, indicating the link’s purpose.
   
5. **Example Enhanced Response**:
   ```json
   {
     "orderId": "12345",
     "orderDate": "2023-10-25",
     "status": "Pending",
     "total": 100.50,
     "_links": {
       "self": { "href": "/api/orders/12345" },
       "update": { "href": "/api/orders/12345", "method": "PUT" },
       "cancel": { "href": "/api/orders/12345", "method": "DELETE" },
       "status": { "href": "/api/orders/12345/status", "method": "GET" },
       "addItem": { "href": "/api/orders/12345/items", "method": "POST" }
     }
   }
   ```

6. **Testing**  
   - Write integration tests to validate the inclusion and accuracy of HATEOAS links in the modified endpoint.
   - Confirm that each link points to the correct endpoint and supports the designated HTTP method, ensuring consistent navigation for client applications. 

Updating an existing endpoint to follow Level 3 REST principles with HATEOAS will make the API more self-descriptive and user-friendly for client applications.

---

# Iteration 7 - JavaScript and ReactJS

### **Main Goal**

#### **JavaScript (ECMA 2017)**
- **let, const**  
- **Arrow Functions**  
  [MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions#syntax)  
- **Object Literals (Initializer)**  
  [MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#creating_new_objects)  
- **Coercion, Equals, Types, and Conditionals**  
  [Top JavaScript Interview Questions](https://dev.to/aershov24/top-26-javascript-interview-questions-i-wish-i-knew-26k1)  
- **Class Definitions**  
  [MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)  
- **Rest/Spread (Array and Objects)**  
  [Rest/Spread Properties in ECMAScript 2018](https://nitayneeman.com/posts/object-rest-and-spread-properties-in-ecmascript-2018/)  
- **Array as API**  
  [MDN Array Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)  
  - Methods: `map`, `filter`, `includes`, `some`, `every`, etc.  
- **Destructuring Assignment**  
  [MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)  
- **`this` Operator**  
  [MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)  
- **Fetch API**  
  [MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)  
- **JS Modules**  
  - `import`, `export`, `default export`  
- **NPM (Node Package Manager)**  
  - Similar to Maven but without packaging.  
  - Features: dependencies, registry (like Maven Central Repo), `package.json` (like `pom.xml`).  
- **Webpack**  
  - Role: Packaging tools for JavaScript.  
  - Key Features: plugins, configuration (`webpack.config.js`).  

---

#### **ReactJS**  
[ReactJS Tutorial](https://reactjs.org/tutorial/tutorial.html)  

1. **Core Concepts**  
   - Functional and Class Components  
   - Props and State  
   - Conditional Rendering  
   - Prop Propagation and Functions as Props  
   - React Hooks ([Documentation](https://reactjs.org/docs/hooks-intro.html))  
   - Render Props ([Documentation](https://reactjs.org/docs/render-props.html))  
   - Higher-Order Components (HOC) ([Documentation](https://reactjs.org/docs/higher-order-components.html))  

2. **Create React App**  
   - Role: Spring Initializer equivalent for ReactJS projects.  
   [Documentation](https://create-react-app.dev/)  

3. **React Packages**  
   - **SWR** ([Documentation](https://swr.vercel.app/))  
   - **React-Bootstrap** ([Documentation](https://react-bootstrap.github.io/))  
   - **React-Router** ([Documentation](https://reactrouter.com/docs/en/v6/getting-started/tutorial))  
   - **React-Intl** (i18n support)  
   - **React-Select**  

---

### **Additional Goal**
- **Storybook**  
  - UI styling and testing.  

---

### **Practical Goal**  
**Objective:** Replace all JSPs with ReactJS-based SPA.  

#### **Implementation Steps:**  
1. **Frontend Integration with Maven**  
   - Use `frontend-maven-plugin` for front-end build integration.  

2. **Development Setup**  
   - Start with `create-react-app` (avoid ejecting).  

3. **React Ecosystem**  
   - Use **Flexbox** for UI components. (Flexbox provides a simpler and more flexible approach for designing responsive layouts compared to   Bootstrap's grid system)
   - Use **React-Router** for navigation.  
   - Use **SWR** for data fetching.  

---

# Iteration 8 - Security with Apache Shiro, JWT, and Frontend Integration with React

---

#### **1. Overview**  
Enhance the security implementation in a Spring Boot application by integrating Apache Shiro with JWT for stateless authentication and enabling seamless integration with a React frontend. The focus includes:  
- Core Shiro concepts (authentication, authorization, and subject management).  
- Stateless authentication using JWT.  
- Integration with Spring Boot and React.  
- Managing user sessions and secure API access in the React frontend.  
- Role- and permission-based UI rendering in React.

---

#### **2. Security Features**  

1. **Authentication**  
   - Use Apache Shiro with JWT to implement stateless authentication.
   - JWTs are issued on successful login and included in the `Authorization` header for API requests.
   
2. **Authorization**  
   - Define roles and permissions.  
   - Enforce role-based and permission-based access control on backend endpoints.  

3. **JWT Integration**  
   - Include roles and permissions as claims in the JWT payload for frontend consumption.  
   - Secure APIs by validating JWTs and extracting claims to determine access levels.

4. **Frontend Integration with React**  
   - Use JWTs for managing user authentication and API access.  
   - Store JWT securely in browser storage (preferably `HttpOnly` cookies or local storage with secure practices).  
   - Decode the JWT to extract user roles and permissions for UI rendering.  

---

#### **3. Backend Implementation Details**  

1. **Shiro Configuration**  
   - Define a custom `Realm` for database integration.  
   - Use a JWT filter to validate and extract claims from incoming requests.  

2. **JWT Token Management**  
   - Include roles and permissions in the JWT for frontend validation.  

3. **API Endpoints**  
   - Implement endpoints for login, token refresh, and secure operations.  

---

#### **4. Frontend Implementation in React**  

1. **Login Process**  
   - Use an API call to the login endpoint to authenticate users and receive a JWT.  

2. **Token Management**  
   - Retrieve the JWT from storage for API requests and include it in the `Authorization` header.

3. **Decoding and Using JWT Claims**  
   - Decode the JWT to extract user roles and permissions for UI decisions.  

4. **Role- and Permission-Based UI Rendering**  
   - Implement conditional rendering in the UI based on user roles and permissions.  

5. **Handling Token Expiry**  
   - Monitor token expiration and refresh tokens as needed to maintain user sessions.

---

#### **5. References**  

1. **Apache Shiro Terminology:** [Shiro Terminology](https://shiro.apache.org/terminology.html)  
2. **Spring Boot Integration:** [Shiro and Spring Boot](https://shiro.apache.org/spring-boot.html).  
3. **JWT Documentation:** [JWT.io](https://jwt.io/).  

