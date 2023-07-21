# REST

[How I explained REST to my brother](https://gist.github.com/brookr/5977550)

## Who is Roy Fielding?

> Roy Fielding is a computer scientist who played a significant role in the creation of the Hypertext Transfer Protocol (HTTP) and the development of Representational State Transfer (REST) architectural style. He is also one of the primary authors of the HTTP specification (RFC 2616).

## Why don’t the techniques that we use in this class work well when we need to be able to talk to all of the machines in the world?

The techniques used in a specific class or local environment might not work well when needing to communicate with all machines in the world due to the following reasons:

- *a. Scalability:* Techniques that work well in a small-scale environment may not scale efficiently to handle the vast number of machines and users on the internet.

- *b. Security:* The internet is a globally connected network with a diverse range of machines and users. Security becomes a crucial concern when communicating with machines worldwide, and the techniques used in a local environment may not be robust enough to handle the potential threats from a global scale.

- *c. Interoperability:* To communicate with machines worldwide, it is essential to follow widely accepted standards and protocols to ensure interoperability. Local techniques might not be compliant with global standards.

## What is the HTTP protocol that Fielding and his friends created?

> HTTP stands for Hypertext Transfer Protocol. It is an application layer protocol used for transmitting hypermedia documents, such as HTML, over the World Wide Web. It was created by Tim Berners-Lee and his team at CERN in the early 1990s, and Roy Fielding was one of the key contributors to the HTTP specification.

## What does a GET do?

> In HTTP, a GET request is a method used to retrieve data from a server. When a client (such as a web browser) sends a GET request to a server, it is asking the server to return a specific resource (identified by the URL) back to the client. The server responds with the requested resource as the payload of the HTTP response.

## What does a POST do?

> A POST request in HTTP is used to send data to the server to create a new resource. It typically includes the data to be sent in the body of the request. The server processes the data and, if successful, responds with a status code indicating the successful creation of the resource.

## What does PUT do?

> PUT is another HTTP method used for updating existing resources on the server. When a client sends a PUT request to a specific URL, it means the client wants to store or replace the resource at that URL with the new data included in the request body.

## What does PATCH do?

PATCH is an HTTP method used for making partial modifications to a resource. It is similar to PUT but is used when you want to apply changes to only a part of the resource, rather than replacing the entire resource. The PATCH request includes the specific modifications to be applied in the request body. This can be useful for updating specific fields of a resource without affecting the rest of the data.