# APIs

## What does REST stand for?

> REST stands for Representational State Transfer.

## REST APIs are designed around a ____.

> REST APIs are designed around resources.

## What is an identifier of a resource? Give an example.

> An identifier of a resource is called a Uniform Resource Identifier (URI). An example of a URI is:
https://api.example.com/users/123

## What are the most common HTTP verbs?

The most common HTTP verbs (methods) used in RESTful APIs are:

- **GET:** Used to retrieve a representation of a resource.
- **POST:** Used to create a new resource.
- **PUT:** Used to update an existing resource.
- **DELETE:** Used to remove a resource.
- **PATCH:** Used to apply a partial update to a resource.

## What should the URIs be based on?

> URIs should be based on the concept of resources and should be designed to be descriptive and intuitive. They should represent the entities and actions in the system.

## Give an example of a good URI.

> Example of a good URI for retrieving information about a specific book:
https://api.example.com/books/978-3-16-148410-0

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

> Having a 'chatty' web API means that the API requires multiple requests to perform a single operation. This is generally considered a bad thing because it can lead to increased network overhead and decreased performance. It's more efficient to design APIs that can perform multiple related actions in a single request.

## What status code does a successful GET request return?

> A successful GET request returns the status code 200 OK.

## What status code does an unsuccessful GET request return?

> An unsuccessful GET request may return various status codes, but commonly it returns 404 Not Found, indicating that the requested resource does not exist.

## What status code does a successful POST request return?

> A successful POST request returns the status code 201 Created, indicating that the request has been fulfilled, and a new resource is created as a result.

## What status code does a successful DELETE request return?

> A successful DELETE request returns the status code 204 No Content, indicating that the request has been successfully processed, but there is no additional content to send in the response.

[RegExr - Pay particular attention to the cheatsheet](https://regexr.com/)
[Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285
)
[Regex 101](https://regex101.com/)