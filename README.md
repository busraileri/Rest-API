# Using Fake API (JSON-SERVER)

In this exercise, we will create a Fake REST API. The advantages of creating a Fake REST API include:

- Testing a frontend application that is already prepared.
- Creating a prototype for backend work that we plan to do.
- Making requests for different HTTP methods on an API platform like Postman.

## Setup Instructions

Initialize the Project:
  ```console
npm init
```

This command will create a package.json file.

Install json-server package with:

```console
npm i json-server
```
Download the example employees.json file from: employees.json. Place this file inside a directory named api in your project.

Update the scripts section in your package.json file as follows:

```json
"scripts": {
    "start:server": "json-server --watch api/employees.json"
  }
```

This allows you to start the FAKE API with the command:

```console
npm run start:server
```

Example Requests

```
GET ALL EMPLOYEES - GET : http://localhost:3000/employees
GET AN EMPLOYEE DETAILS - GET : http://localhost:3000/employees/:employee_id
EMPLOYEES - ROLES RELATION - GET : http://localhost:3000/employees?_expand=role
ADD AN EMPLOYEE - POST : http://localhost:3000/employees
UPDATE AN EMPLOYEE - PATCH(PUT) : http://localhost:3000/employees/:employee_id
DELETE AN EMPLOYEE - DELETE : http://localhost:3000/employees/:employee_id
```

## For More Information
 - ### [json-server](https://github.com/typicode/json-server)