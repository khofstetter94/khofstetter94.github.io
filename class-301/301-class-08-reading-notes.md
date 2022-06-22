# APIs

[API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

- **What does REST stand for?** - Representational State Transfer
- **REST APIs are designed around a ____.** - around resources
- **What is an identifier of a resource? Give an example.** - which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

        https://adventure-works.com/orders/1

- **What are the most common HTTP verbs?** - The most common operations are GET, POST, PUT, PATCH, and DELETE.
- **What should the URIs be based on?** -  URIs should be based on nouns (the resource) and not verbs (the operations on the resource).
- **Give an example of a good URI.** -

        https://adventure-works.com/orders

- **What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?** - A "chatty" web API exposes a large number of small resources. It is a bad thing.
- **What status code does a successful GET request return?** - HTTP status code 200 (OK).
- **What status code does an unsuccessful GET request return?** - 404 (Not Found).
- **What status code does a successful POST request return?** - HTTP status code 201 (Created).
- **What status code does a successful DELETE request return?** - HTTP status code 204 (No Content)

## Things I want to know more about

- The verbs POST, PUT, PATCH, and DELETE. How to make a web API less chatty.

[Return home](https://khofstetter94.github.io/reading-notes/)
