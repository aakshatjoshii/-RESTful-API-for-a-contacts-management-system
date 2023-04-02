# RESTful-API-for-contacts-management-system

## Project OverView

This is a Node.js-based RESTful API built using the Express.js framework and MongoDB database. The API allows users to perform CRUD (create, read, update, delete) operations on contacts.

## Getting Started
To get started with this project, follow the steps below:

1. Clone the repository using the following command: 

```bash
git clone https://github.com/aakshatjoshii/-RESTful-API-for-a-contacts-management-system.git
```

2. Install the dependencies listed in package.json file with the following command:

```
nm install
```

3. Create a .env file in the root directory of the project and add the following environment variables:

```bash
PORT=5001
CONNECTION_STRING= mongodb+srv://admin:admin@cluster0.yl7jggw.mongodb.net/mycontacts-backend?retryWrites=true&w=majority
```

4. Coonect to mongo DB locally and Start the server using the following command:

```
npm start
```
## API Endpoints

The following API endpoints are available:

* GET /api/contacts

This endpoint returns a list of all contacts.

Query Parameters:

page (optional): the page number to retrieve, defaults to 1.
limit (optional): the number of items to retrieve per page, defaults to 10.
name (optional): the name of the contact to filter by.
GET /contacts/:id
This endpoint returns a single contact with the given id.

* POST /api/contacts

This endpoint creates a new contact.

Request Body:

```perl
{
  "name": "Akshat",
  "email": "akshat@gmail.com",
  "phone": "9876543210",
}
```
* PUT /api/contacts/:id

This endpoint updates the contact with the given id.

Request Body:

```perl
{
  "name": "Akshat Joshi",
  "email": "akshat123@gmail.com",
  "phone": "9876543210"
}
```

* DELETE /api/contacts/:id

This endpoint deletes the contact with the given id.

## Testing
To run the unit tests for the API endpoints, use the command npm start. Test the api endpoints using Postman or thunder client [VS code plugin].


## Credits
This project was created by Aakshat Joshi.




