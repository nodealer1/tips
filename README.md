# tips
Enroll Course:
https://sso.teachable.com/secure/164090/identity/sign_up

Bookmark:
https://github.com/in28minutes?tab=repositories


https://www.knowledgehut.com/interview-questions/spring-boot

https://github.com/rahulmoundekar/Spring-Boot-Interview-Questions

http://www.codespaghetti.com/spring-interview-questions/#introduction

https://www.interviewbit.com/microservices-interview-questions/


Microservices Interview Questions and Answers
Q. List down the advantages of Microservices Architecture.

Q. What are the best practices to design Microservices?

Q. How does HTTPS authentication works in Microservices?

Q. What is RabbitMQ?

Q. What is an idempotent in REST APIs?

In the context of REST APIs, when making multiple identical requests has the same effect as making a single request – then that REST API is called idempotent.

An idempotent HTTP method is an HTTP method that can be called many times without different outcomes. It would not matter if the method is called only once, or ten times over. The result should be the same. It essentially means that the result of a successfully performed request is independent of the number of times it is executed. For example, in arithmetic, adding zero to a number is idempotent operation.

Example:

    POST is NOT idempotent.
    GET, PUT, DELETE, HEAD, OPTIONS and TRACE are idempotent.

Q. What is Bounded Context?

Q. What is the use of PACT in Microservices architecture?

Q. What is the use of Container in Microservices?

Q. What is the role of Web, RESTful APIs in Microservices?

Q. What is OAuth?

Q. What is Conway’s law?

Q. What is a Consumer-Driven Contract (CDC)?

Q. What do you understand by Semantic monitoring in Microservices architecture?

Q. What is Canary Releasing?

Q. Why would we need Reports and Dashboards in Microservices?

Q. What is Semantic Versioning?

Q. What is the difference between Mean Time to Repair (MTTR) and Mean Time between failures (MTBF)?

Q. What is Confused Deputy Problem in security context?

Q. What are the important Cross-Functional Requirements to consider during the design of a Microservice?

Q. What is a Circuit Breaker pattern in the context of Microservice?

Q. What is Bulkhead design pattern?

Q. How can you scale a Database?

Q. What is Command Query Responsibility Segregation (CQRS) design pattern?

Q. What is CAP theorem?

Q. What do you mean by Eureka in the realm of Microservices?

Q. Can you integrate Zuul with other types of projects?

Q. Describe the circumstances under which you would use the Netflix Hystrix

Q. Shed light on Tasklet with reference to Spring Batch and Microservices

Q. What do you know about YAML in the realm of Microservices?

Q. Shed light on the various types of IT characteristics that are available in Microservices

Q. How to monitor multiple Microservices For Various Indicators Like Health?

Q. What are the possible ways for communication between microservices?

Q. What is exchange in message queue?

Q. What are the possible solutions for the case when one service is not available?

Q. What is the difference between synchronous and asynchronous communication?

Q. What are possible ways for implementing authentication in microservices?

Q. What is Eventual consistency?

Q. What is Cohesion and Coupling?

Q. What are different types of Tests for Microservices?

Q. What do you understand by Distributed Transaction in microservices?

## Spring Framework Annotations

|Sl.No| Annotation    | Description  |
|-----|---------------|--------------|
| 01. |@Autowired	  |Annotation @Autowired is used to inject object dependency implicitly for a **constructor, field or method**. This is known as “autowired by type” since the object to be injected is discovered by its type. The items declared @Autowired need not have to be public.|				
| 02. |@Configurable  |	Used on classes to inject properties of domain objects. Types whose properties are injected without being instantiated by Spring can be declared with @Configurable annotation.	|
| 03. |@Qualifier	  |It can be used to create more than one bean of the same type and wire only one of the types with a property. It provides greater control on the dependency injection process and can be used with @Autowired annotation.|
| 04. |@Required	  |Used to mark class members that are mandatory. The Spring auto-configuration fails if a particular property specified with this annotation cannot be injected.|
| 05.  |@ComponentScan|Make Spring scan the package for the @Configuration clases.|
| 06.  |@Configuration|It is used on classes that define beans.|
| 07.  |@Bean	      |It indicates that a method produces a bean which will be mananged by the Spring container.|			
| 08.  |@Lazy	      |Makes a @Bean or @Component to be initialized only if it is requested.|		
| 09.  |@Value	      |It is used to inject values into a bean’s attribute from a property file. @Value annotation indicates a default value expression for the field or parameter.|	
| 10.  |@Resource     |Annotation used to inject an object that is already in the Appl­ication Context. It searches the instance by name. It also works on setter methods.|
| 11.  |@Primary      |Annotation used when no name is provided telling Spring to inject an object of the annotated class first. Used along with @Comp­onent.|
| 12.  |@Component    |Generic stereotype annotation used to tell Spring to create an instance of the object in the Appl­ication Context. It's possible to define any name for the instance, the default is the class name as camel case.|
| 13.  |@Contr­oller   |Stereotype annotation for presen­tation layer.|
| 14.  |@Repos­itory   |Stereotype annotation for persis­tence layer. |
| 15.  |@Service      |Stereotype annotation for service layer.     |
| 16.  |@Conditional  |Annotation is used to load beans into Application Context only if the given condition is met.|


#### Spring-Boot Web Annotations

|Sl.No| Annotation            | Description  |
|-----|-----------------------|--------------|
| 01. |@SpringBootApplication |	This annotation is used to qualify the main class for a Spring Boot project. The class used with this annotation must be present in the base path. @SpringBootApplication scans for sub-packages by doing a component scan.|   			
| 02. |@EnableAutoConfiguration|Based on class path settings, property settings, new beans are added by Spring Boot by using this annotation.|					
| 03. |@Controller	           |Allows detection of component classes in the class path automatically and register bean definitions for the classes automatically.|					
| 04. |@RestController	       |Used in controllers that will behave as RESTful resources. @RestController is a convenience annotation that combines @Controller and @ResponseBody.	|				
| 05. |@ResponseBody	       |Makes Spring to convert the returned object to a response body. This is useful for classes exposed as RESTful resources.|				
| 06. |@RequestMapping	       |Used to map web requests to specific handler classes and methods, based on the URI.|
| 07. |@RequestParam	       |This annotation is used to bind request parameters to a method parameter in your controller.| 
| 08. |@PathVariable	       |This annotations binds the placeholder from the URI to the method parameter and can be used when the URI is dynamically created or the value of the URI itself acts as a parameter.	|	



#### Profile

|Sl.No| Annotation            | Description  |
|-----|-----------------------|--------------|
| 01. |spring.profiles.active |Property to be set in appl­ica­tio­n.p­rop­ert­ies in order to tell Spring what profiles are active.|
| 02. |@Profile("dev")       |Annotation used to define which profile can execute the annotated method.|


#### Aspect Annotations

|Sl.No| Annotation     |USE       | Description  |
|-----|----------------|----------|--------------|
| 01. |@Aspect         |Type      |Declares a class to be an aspect.|
| 02. |@After          |Method    |Declares a method to be called after a pointcut completes.|
| 03. |@AfterReturning |Method    |Declares a method to be called after a pointcut returns successfully.|
| 04. |@AfterThrowing  |Method    |Declares a method to be called after a pointcut throws an exception.|
| 05. |@Around         |Method    |Declares a method that will wrap the pointcut.|
| 06. |@Before         |Method    |Declares a method to be called before proceeding to the pointcut.|
| 07. |@DeclareParents |Static Field |Declares that matching types should be given new parents,that is, it introduces new functionality into matching types.|
| 08. |@Pointcut       |Method    |Declares an empty method as a pointcut placeholder method.|


#### Spring-Boot Testing Annotations

|Sl.No| Annotation            | Description  |
|-----|-----------------------|--------------|
| 01.  |@AfterTransaction	  |Annotation used to identify which method needs to be invoked after a transaction is completed.|
| 02.  |@BeforeTransaction	  |Used to identify the method to be invoked before a transaction starts executing.	|			
| 03.  |@ContextConfiguration |Declares the annotated classes which will be used to load the context for the test. The location of the configuration file has to be povided to Spring.|					
| 04.  |@DirtiesContext	      |This annotation indicates the test(s) modify or corrupt the SpringApplicationContext and that it should be closed. Hence, context is reloaded before the next test is executed.|					
| 05. |@ExpectedException	  |The test method is expected to throw a particular exception, else the test fails.|
| 06. |@WebAppConfiguration	  |Used to create web version of the application context.	|				
| 07. |@Repeat	              |Specifies the test method to be executed multiple times.	|				
| 08. |@Transactional 	      |Describes transaction attributes on a method or class.	|				
| 09. |@Rollback	          |Indicates if the transaction of a test method must be rolled back after the execution of the test completed.	|     			
| 10. |@Commit	              |Indicates that the transaction of a test method must be committed after the execution of the test completed.|     		
| 11. |@Timed	              |Indicates the time limit for the test method. If the test has not completed execution before the time expires, the test fails.|					
| 12. |@TestPropertySource	  |Annotation specifies the property sources for the test class.|					
| 13. |@Sql	                  |Annotation declares a test class/method to run SQL scripts against a database.|	


##### Workflow and Tools 

|Sl.No| Category     |Tool                    | Description                         |
|-----|--------------|------------------------|-------------------------------------|
| 01. |Development	 |Spring Tool Suite (STS) |	STS is an Eclipse-based development environment that can be used to develop Spring applications easily.|
| 02. |Development	 |Eclipse	              |IDE used to develop Java applications. It has a plugin for develping Spring applications. Useful when working simultaneously on Spring and non-Spring based apps.|
| 03. |Development	 |IntelliJ IDEA	          |Provides a smooth environment and user experience for developing Spring applications. Provides a comprehensive view of the project forspeedy navigation, error highlighting, plugins for numerous purposes, code completion.|
| 04. |Unit Testing	  |JUnit	              |JUnit is a regression Testing Framework used to implement unit testing in Java with an enhanced speed and quality.|
| 05. |Unit testing	  |Mockito                |It is an open source mocking framework to create mock classes and interfaces providing realistic tests to predict the behaviour of the application.|
| 06. |Unit testing	  |JaCoCo                 |Provides support for code-coverage measurement and generates a detailed test report.|
| 07. |API Testing	  |JMeter                 |Apache’s JMeter is an open source testing tool which includes load, functional, regression and performance tests.|
| 08. |API Testing	  |Postman	              |Postman is a powerful tool used to test web services. It provides a feature to create test collections and can be used for API testing.|
| 09. |API Testing	  |REST-Assured	          |Makes API tesing in Java simple by providing behaviour driven development. It can integrate with any existing Java automation framework.|
| 10. |Monitoring	  |spring-boot-actuators  |Enables monitoring and managing Spring boot application by shipping production ready featues like health, metrics, HTTP tracing etc.|
| 11. |Monitoring	  |Micrometer	          |Micrometer is an application-neutral facade or abstraction for reporting application metrics which integrates with many monitoring systems, e.g., Graphite, New Relic and Statsd. Micrometer integrates with the metrics endpoint of spring-boot-actuators.|

<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>



Q1: Define Microservice Architecture  Related To: Software Architecture
 
Q2: Why Would You Opt For Microservices Architecture?  
 
Q3: List down the advantages of Microservices Architecture  
 
Q4: How does Microservice Architecture work?  
  
Q5: What are the features of Microservices?  
  
Q6: What is the difference between Monolithic, SOA and Microservices Architecture?  Related To: Software Architecture, SOA
  
Q7: What are main differences between Microservices and Monolithic Architecture?  
  
Q8: How can we perform Cross-Functional testing?  
  
Q9: What Are The Fundamentals Of Microservices Design?  
  
Q10: What are the challenges you face while working Microservice Architectures?  
 Q11: Whether do you find GraphQL the right fit for designing microservice architecture?  Related To: GraphQL
  
Q12: What are the standard patterns of orchestrating microservices?  
  
Q13: What is the difference between a proxy server and a reverse proxy server?  
  
Q14: What are smart endpoints and dumb pipes?  
  
Q15: What do you understand by Contract Testing?  
  
Q16: Can we create State Machines out of Microservices?  
  
Q17: What is Idempotence?  
  
Q18: What do you understand by Distributed Transaction?  
  
Q19: What is the role of an architect in Microservices architecture?  
  
Q20: What are the pros and cons of Microservice Architecture?  
  
Q21: What is Materialized View pattern and when will you use it?  
  
Q22: Mention some benefits and drawbacks of an API Gateway  
  
Q23: Explain what is the API Gateway pattern  Related To: API Design
  
Q24: How should the various services share a common DB Schema and code?  
  
Q25: Name the main differences between SOA and Microservices?  Related To: SOA
  
Q26: What does it mean that shifting to microservices creates a run-time problem?  
  
Q27: What is the difference between Cohesion and Coupling?  Related To: Software Architecture
  
Q28: What is a Consumer-Driven Contract (CDC)?  
  
Q29: What are Reactive Extensions in Microservices?  
  
Q30: What is the most accepted transaction strategy for microservices?  Related To: Software Architecture
  
Q31: What Did The Law Stated By Melvin Conway Implied?  
  
Q32: Why would one use sagas over 2PC and vice versa?   
  
Q33: How would you implement SSO for Microservice Architecture?  
  
Q34: Provide an example of "smart pipes" and "dumb endpoint"  
  

