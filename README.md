# CRUD RESTful-API

This is a python API that I developed, right now it contains a V1 and a V2, the V1 being a basic version. Users can authenticate and use 4 HTTP protocols to add/delete/see/update items and their price.

I used the following libraries to make this project:
- Flask
- Flask-RESTful
- Flask-JWT
- SQLite3

Everything was tested multiple times during development using Postman, these are the routes that the API uses:

```
/items to GET the list of items stored in the DB
/register to POST a user to the DB
/auth to POST a connection request, the API responds with a JWToken that you can use to access the methods that require to be connected
/item/<name> to GET/POST/PUT/DELETE an item, in order to POST and DELETE, a price must be given to the request in json format, for example {"price": 10.00}
```
## V1

The first version is a simple API that stores items and users in lists, these 4 HTTP protocols are implemented:

```
GET
POST 
DELETE
PUT
```

## V2

This version uses the SQLite3 library to store users and items in a DB
