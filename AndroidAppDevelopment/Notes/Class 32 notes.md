[Intro to Serverless](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)

[AWS Amplify](https://aws.amazon.com/amplify/)

[GraphQL Intro (just read the first few paragraphs, up until the query code)](https://docs.amplify.aws/cli/graphql/data-modeling/)

## Questions

1. What makes an API RESTful?
	 - Client-Server Architecture: API follows a client-server model over HTTP.
	- Stateless: Server does not maintain client state between requests.
	- Uniform Interface: API uses standard HTTP methods (GET, POST, PUT, DELETE) and URLs to interact with resources.
	- Resource-Based: API is based on identifiable resources accessed through URIs.
	- Representation-Oriented: Resources are represented in agreed formats (e.g., JSON or XML).
	- State Transfer: Resource state is transferred between client and server through representations.
	- Cacheable: Responses can be cached for improved performance.
	- Layered System: API can be designed with multiple layers for various functionalities.
1. What is the benefit of using GraphQL? Any downsides?
	**Benefits of GraphQL**:

- **Efficient Data Loading**: With GraphQL, the client specifies exactly what data it needs, which can reduce the amount of data transferred over the network.
    
- **Single Request-Response Cycle**: Instead of making several requests to different endpoints (as in REST), with GraphQL you can gather all the data your app needs in a single request.
    
- **Type Safety**: The schema that GraphQL uses is a strong type system which helps to ensure that the API is type-safe.
    
- **Real-time Data with Subscriptions**: GraphQL includes the concept of subscriptions for real-time data updates in its core specification.
    

**Downsides of GraphQL**:

- **Complexity**: GraphQL is more complex to understand and implement compared to REST.
    
- **Performance Issues with Large Queries**: In GraphQL, a client could request a lot of nested data in a single query, potentially leading to performance issues.
    
- **Caching**: Caching in GraphQL can be complex to implement because unlike REST, it doesn’t use HTTP caching mechanisms by default.
    
- **Over-fetching, Under-fetching**: While GraphQL is designed to avoid these problems, improper design can still lead to similar issues if the queries are not designed and optimized properly.
2. Describe “serverless” to a new 301 Code Fellows student.
	1. A server rack is typically how a company would store and manage all of their data in the past. You would store all of your data in one place and access it from that rack. Where serverless comes into play is instead of managing your own rack you outsource to a company like AWS. Now AWS doesnt just store your data in one rack they store your data across hundreds or thousands of racks at random where you only use up as much data as you need. so if a rack is 1000 TB of data and you only need 1TB of data you wont have to pay for a full rack you just pay to store your 1 TB. 