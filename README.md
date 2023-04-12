# Store API

## This is a RESTful API built with Express and MongoDB. It allows the user to perform various actions on a database of store products that have been populated with JSON data. The user can perform the following actions:

    Sort the data using any of the properties such as company, name, rating either in ascending or descending order, etc.
    Get the data of only the properties they want to access.
    Get access to certain fields such as the company and name or rating scale and price, depending on the fields the user wants to access.
    Search for company names without typing the full company. As the user types the characters of the word they want to search for, the API fetches all data that contains those particular characters.
    Limit the number of data the API fetches.

## Getting Started

To get started with this API, you need to follow these steps:

    Clone this repository to your local machine
    Navigate to the project directory and run npm install to install all dependencies
    Run npm start to start the server
    Use a tool such as Postman to make requests to the API endpoints.

## API Endpoints
### Get all products

To get all the products, make a GET request to the /products endpoint.
Sort products

To sort the products, make a GET request to the /products/sort endpoint, and include the property you want to sort by and the order you want to sort in the query parameters. For example:


```
/products/sort?property=name&order=asc
```

Get specific fields

To get specific fields of the products, make a GET request to the /products/fields endpoint, and include the fields you want to get in the query parameters. For example:


```
/products/fields?fields=name,company
```

## Search for products

To search for products by company name, make a GET request to the /products/search endpoint and include the characters you want to search for in the query parameters. For example:

bash

/products/search?query=app

## Limit products

To limit the number of products returned, make a GET request to the /products/limit endpoint and include the number of products you want to get in the query parameters. For example:

```

/products/limit?limit=5
``` 

Conclusion

That's it! You can now use this API to interact with the store products database, sort the data, get specific fields, search for products, and limit the number of products returned. Feel free to modify the code to suit your needs.