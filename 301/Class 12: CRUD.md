# CRUD

[Status codes based on REST methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

## In your own words, describe what each group of status code represents:

Status codes are three-digit numbers that are part of the HTTP response sent by a server to a client after a request is made. Each group of status codes represents a different category of response, conveying specific information about the request's success or failure.

- *100’s* = **Informational responses.** These codes indicate that the server has received the request and is continuing to process it. They are typically used to inform the client about the server's intermediate status.
- *200’s* = **Success responses.** These codes indicate that the server has successfully processed the request and is providing the requested information or action.
- *300’s* = **Redirection responses.** These codes indicate that further action needs to be taken by the client to complete the request. They often provide information about new locations or alternative resources.
- *400’s* = **Client error responses.** These codes indicate that the server could not fulfill the client's request due to an error on the client's side.
- *500’s* = **Server error responses.** These codes indicate that the server encountered an error while trying to process the request.

## What is a status code 202?

> **Status code 202 (Accepted):** This status code indicates that the request has been accepted for processing but not yet completed. It means that the server has received the request and will process it asynchronously.

## What is a status code 308?

> **Status code 308 (Permanent Redirect):** This status code is used to indicate that the requested resource has been permanently moved to a different location. The client should update its bookmarks or links to use the new URL provided in the response.

## What code would you use if an update didn’t return data to a client?

> If an update didn't return data to a client: In this scenario, you could use status code 204 (No Content). It indicates that the request was successfully processed, but there is no additional data to send in the response.

## What code would you use if a resource used to exist but no longer does?

> If a resource used to exist but no longer does: In this case, you could use status code 410 (Gone). It indicates that the requested resource is no longer available on the server and has been intentionally removed.

## What is the ‘Forbidden’ status code?

> **'Forbidden' status code:** The 'Forbidden' status code is 403. It indicates that the server understood the request, but the server refuses to authorise it. This status is similar to 401 (Unauthorised), but indicates that the client must authenticate itself to get access, and even after authentication, access is not allowed.

[Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 min](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

## Why do we need to pull our MongoDB database string out of our server and put it into our .env?

> Storing sensitive information, such as database connection strings, in the server code directly can be risky. If this information is exposed accidentally, it could lead to unauthorised access to the database, data breaches, or other security issues. By placing the MongoDB database string into a .env file, it is kept separate from the main codebase and is not exposed publicly. The .env file is typically not committed to version control, ensuring that sensitive information remains confidential and accessible only to authorized users who have access to the server environment.

## What is middleware?

Middleware is a concept in software development, particularly in web applications, where it acts as a bridge between the incoming request and outgoing response. In the context of web servers and frameworks, middleware functions intercept HTTP requests before they reach the final handler, allowing developers to perform various tasks such as authentication, logging, data parsing, and error handling. Middleware functions can modify the request or response objects, terminate the request-response cycle, or pass control to the next middleware in the chain.

## What does app.use(express.json()) do?

This code is used with the Express.js framework in Node.js applications to parse incoming JSON data. When a request with a JSON payload is received by the server, the express.json() middleware parses the JSON data and makes it available in the req.body object, allowing developers to access the data easily in their route handlers.

## What does the /:id mean in a route?

In the context of defining routes in web applications, the "/:id" represents a route parameter. It is a placeholder for a dynamic value that will be passed as part of the URL when the client makes a request. For example, if the route is defined as "/users/:id", then accessing "/users/123" would match this route, and the value "123" would be available as req.params.id in the route handler.

## What is the difference between PUT and PATCH?

**PUT:** The HTTP PUT method is used to update or replace an entire resource at a specific URL. When making a PUT request, the client sends the entire representation of the resource, and the server replaces the resource with the new representation. If the resource does not exist, PUT can create a new one.

**PATCH:** The HTTP PATCH method is used to apply partial modifications to a resource. It is more focused on updating specific fields or properties of a resource, rather than replacing the entire resource. The client sends only the changes (or the delta) to the server, and the server applies those changes to the existing resource.

## How do you make a default value in a schema?

> In databases and schema design, you can define default values for certain fields in a schema. If a document or record is created without specifying a value for a particular field, the default value will be automatically assigned to that field. This ensures that the field always has a value, even if it is not explicitly provided during the data creation process.

## What does a 500 error status code mean?

> The 500 status code is a server error response that indicates that an unexpected condition was encountered on the server, and the server was unable to fulfill the client's request. It is a generic error message that could be caused by various issues on the server, such as a bug in the server-side code, database connectivity problems, or other internal server errors.

## What is the difference between a status 200 and a status 201?

**Status 200 (OK):** This status code indicates that the server successfully processed the client's request, and everything is okay. It is the standard response for successful HTTP requests.

**Status 201 (Created):** This status code is used to indicate that a new resource has been successfully created as a result of the client's request. It is often sent in response to successful POST requests when a new resource is added to the server. The response should include a Location header with the URL of the newly created resource.