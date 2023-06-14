[Spring Security overview](https://spring.io/guides/topicals/spring-security-architecture/)

1.  What does it mean to authenticate a user?
	1. to verify the users identity
2.  What does it mean to authorize a user?
	1. to give access to the autheticated user
3.  What are the three possible outcomes of the AuthenticationManager’s authenticate() method?
	1.   Return an `Authentication` (normally with `authenticated=true`) if it can verify that the input represents a valid principal.
    
	2.  Throw an `AuthenticationException` if it believes that the input represents an invalid principal.
    
	3.   Return `null` if it cannot decide.

[Spring Auth cheat sheet](https://github.com/codefellows/seattle-java-401d2/blob/master/SpringAuthCheatSheet.md)

1.  Review the cheatsheet above!