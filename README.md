# Microservices Design Patterns
- Saga Design Patterns

This pattern is used maintain data consistency across distributed services. It can be used as 2PC is expensive and doesn't scale. A saga is a sequence of requests. Each request execute instructions and publishes a message or event to trigger the next request in the saga. If a any request fails then the saga executes a series of compensating transactions that undo the changes that were made by the preceding all requests.

 ![Saga example](diagram/saga%20patterns.png)


### References
https://microservices.io/

https://www.youtube.com/watch?v=xDuwrtwYHu8&t=1576s
