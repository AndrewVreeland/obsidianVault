## Reading

[Spring App Basics](https://spring.io/guides/gs/serving-web-content/)

1.  What role do the @Controller classes play in a Spring MVC application?
	1.  The controller handles http requests
2.  Explain to a non-technical friend what a GET request is.
	1.  a get requested is like asking for food at a restaraunt and the waiter coming back with that food. If you ask for something that is not on the menu then you get an error and the waiter wont be able to bring you that food
3.  What annotation should be placed on your Spring Boot application class?
	1. import org.springframework.web.bind.annotation.GetMapping;
	2. import org.springframework.web.bind.annotation.RequestParam;
	3. [`@Controller`](http://docs.spring.io/spring/docs/current/javadoc-api/org/springframework/stereotype/Controller.html) annotation.

[Spring MVC and Thymeleaf](https://www.thymeleaf.org/doc/articles/springmvcaccessdata.html)

1.  What method allows for a variable defined in Java (in your Spring Controller) to be dispalyed in HTML with the help of Thymeleaf?
	1. To display a variable defined in a Spring Controller in HTML using Thymeleaf, you can use the `th:text` attribute in your HTML template.
2.  Explain the role of a @Controller class in a Spring MVC application.
	1. `@Controller` classes are responsible for preparing a model map with data and selecting a view to be rendered.
3.  What is a model attribute refered to in Thymeleaf?
	1. The equivalent term in Thymeleaf language is _context variables_.