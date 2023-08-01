# More CRUD

[CRUD Basics](https://medium.com/geekculture/crud-operations-explained-2a44096e9c88)

## Which HTTP method would you use to update a record through an API?

**HTTP PUT:**
The PUT method is used to update the entire resource with new data. When you make a PUT request to the API endpoint with the updated data, it replaces the entire resource with the new data provided. If some fields are not included in the PUT request, they may be removed or reset to default values.

**HTTP PATCH:**
The PATCH method is used to make partial updates to the resource. Unlike PUT, which replaces the entire resource, PATCH updates only the fields provided in the request, leaving other fields unchanged.

## Which REST methods require an ID parameter?

The following methods typically require an ID parameter:

**GET:**
The GET method is used to retrieve a specific resource or a collection of resources. When you want to fetch details about a single resource, you usually include the resource's ID as part of the URL.

As mentioned earlier, both PUT and PATCH methods require the resource's ID to specify which resource should be updated.

**DELETE:**
The DELETE method is used to remove a specific resource from the system. Like the other methods, you need to provide the resource's ID in the URL to specify which resource should be deleted.

**HEAD and OPTIONS** methods don't necessarily require an ID parameter, but they can be used to retrieve information about a specific resource if the server supports it. These methods are mainly used for preflight checks and to get metadata about a resource.

In summary, the HTTP methods that typically require an ID parameter in a RESTful API are GET (for specific resource retrieval), PUT, PATCH (for updates), and DELETE (for deletion).

[Speed Coding: Building a CRUD API](https://www.youtube.com/watch?v=EzNcBhSv1Wo)

## What’s the relationship between REST and CRUD?

> The relationship between REST (Representational State Transfer) and CRUD (Create, Read, Update, Delete) is that RESTful APIs often implement CRUD operations for resources. REST is an architectural style that defines a set of principles for designing networked applications, while CRUD represents the four basic functions that can be performed on resources in a system. RESTful APIs follow REST principles to create, read, update, and delete resources using standard HTTP methods (GET, POST, PUT, PATCH, DELETE).

## If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

- **Design Resource Model:**
Identify the resources that your API will manage. These can be entities like books, users, products, etc.
Define the attributes and relationships of each resource. This will form the basis of the data schema for your API.

- **Choose Base URL and Versioning:**
Decide on the base URL for your API, which will serve as the starting point for all endpoints. For example, https://api.example.com/v1.
Consider versioning your API in the URL (e.g., /v1/) to allow for future updates without breaking existing clients.

-**Define API Endpoints:**
Determine the URL structure for each CRUD operation on each resource.
Use HTTP methods (GET, POST, PUT, PATCH, DELETE) to represent the corresponding CRUD operation for each endpoint.

For example:
GET /v1/books - Retrieve a list of books.
POST /v1/books - Create a new book.
GET /v1/books/{id} - Retrieve details of a specific book by its ID.
PUT /v1/books/{id} - Update a book's information using its ID.
DELETE /v1/books/{id} - Delete a book by its ID.
Implement API Handlers:

- **Develop the server-side logic to handle each API endpoint.**
For each endpoint, define the corresponding functionality, such as reading from the database, creating new records, updating records, or deleting records.
Add Data Validation and Security:

- **Implement data validation to ensure that incoming requests contain the required fields and meet specific criteria.**
Enforce security measures to protect sensitive operations and data from unauthorized access. This may involve authentication and authorization mechanisms.
Additionally, when creating a RESTful API, it's essential to adhere to RESTful principles, such as statelessness, uniform interface, and using the appropriate HTTP status codes and response formats (e.g., JSON) for consistent communication. By following these steps and principles, you can design and develop a robust and scalable RESTful API that provides CRUD functionality for your resources.