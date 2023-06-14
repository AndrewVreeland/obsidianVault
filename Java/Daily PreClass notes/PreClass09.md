[Related data in Spring (only read section “3. One-to-Many Relationship”)](https://www.baeldung.com/spring-data-rest-relationships)

1.  Name a few real life examples of “One To Many” relatioships.
	1. a teacher to stundetns, one teacher many students.
2.  Given two entities, one named Player and one named Team, if you wanted to create a one to many relationship with those entities which would be the one and which would be the many?
	1. the team would be the one and the players would be the many 
3.  Explain one to many relationships to a non-technical friend.
	1. another example could be you have one artist and many songs 
	

[Baeldung: Spring Integration Testing](https://www.baeldung.com/integration-testing-in-spring)


In order to test you will need many dependencies 
We'll need several Maven dependencies for running the integration tests First and foremost, we'll need the latest [junit-jupiter-engine](https://search.maven.org/classic/#search%7Cga%7C1%7Cg%3A%22org.junit.jupiter%22%20AND%20a%3A%22junit-jupiter-engine%22), [junit-jupiter-api](https://search.maven.org/classic/#search%7Cga%7C1%7Cg%3A%22org.junit.jupiter%22%20AND%20a%3A%22junit-jupiter-api%22), and [Spring test](https://search.maven.org/classic/#search%7Cgav%7C1%7Cg%3A%22org.springframework%22%20AND%20a%3A%22spring-test%22) dependencies:

```java
@Test
public void givenHomePageURI_whenMockMVC_thenReturnsIndexJSPViewName() {
    this.mockMvc.perform(get("/homePage")).andDo(print())
      .andExpect(view().name("index"));
}
```

Let's break it down:

-   _perform()_ method will call a GET request method, which returns the _ResultActions_. Using this result, we can have assertion expectations about the response, like its content, HTTP status, or header.
-   _andDo(print())_ will print the request and response. This is helpful to get a detailed view in case of an error.
-   _andExpect()_ will expect the provided argument. In our case, we're expecting “index” to be returned via _MockMvcResultMatchers.view()._


1.  Describe the difference between a unit test and an integration test.
	1. While unit tests always take results from a single unit, such as a function call, integration tests may aggregate results from various parts and sources.
2.  What is the object that provides support for Sprin MVC Testing?
	1. _MockMvc_ provides support for Spring MVC testing. **It encapsulates all web application beans and makes them available for testing.**
3.  What does the “perform()” method do in a Spring integration test?
	1.    _perform()_ method will call a GET request method, which returns the _ResultActions_. Using this result, we can have assertion expectations about the response, like its content, HTTP status, or header.

