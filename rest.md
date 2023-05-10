# RESTful Services

## 6 Constraints of REST

1. **Client-server architecture:** RESTful services are designed to be client-server based, meaning that the client and server are separate and independent components that communicate with each other using a standardized protocol. This constraint allows for better scalability and improved separation of concerns between the client and server.


1. **Stateless communication:** As mentioned earlier, RESTful services are designed to be stateless, meaning that the server does not store any client data or session information between requests. While this constraint allows for better scalability and improved performance, it can also make it more difficult to maintain application state between requests.


1. **Cacheability:** RESTful services should be designed to be cacheable, allowing clients and intermediaries to cache responses and reduce the number of requests made to the server. However, this constraint can also make it more difficult to implement dynamic, real-time services that require immediate updates.


1. **Layered architecture:** RESTful services should be designed to be layered, allowing for intermediaries such as proxies and gateways to be used to improve scalability and reliability. However, this constraint can also introduce additional latency and complexity into the system.


1. **Uniform interface:** RESTful services should use a uniform interface, allowing clients to interact with the service in a consistent and predictable manner. While this constraint allows for better interoperability and ease of use, it can also limit the flexibility and expressiveness of the API.


1. **Code on demand:** This is an optional constraint, which allows the server to send code to the client, allowing the client to execute the code. This constraint is rarely used in practice, as it can introduce security risks and complicate the design of the system.


## URI and URL

A URI is a general term that refers to any identifier for an online resource, a URL is a specific type of URI that includes the information needed to access a resource, such as the protocol (like http or https), the domain name (like google.com), and the path to the resource (like `/search?q=URI+vs+URL`).


## Statelessness

Statelessness refers to a communication between computers or servers where the server does not remember any information about the client between requests. This can simplify the server and make it more reliable and scalable, but may require clients to provide more information for each request.