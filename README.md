# restapi example
Boiler plate of a REST API using node.js, Express router and jsonwebtoken

### Usage:
You must have node.js/npm and MongoDB installed

As root :
```
npm install
```

Change config file to match your configuration.

Then:

```
node server.js
```

It should print something like:

```
' Listening port 8080 '
```

Very simple. The boiler contain a token generation and checkup logic 
(very basic) as middleware and provide basic routing structure.

Just start from there and you can vuild a restapi in hours.

##### PS: jsonwebtoken npm seem to be changed need to replace it in package.json and in server.js to use another jwt module

## MongoDB setup

```
./mongo
> use test
> db.inventory.insertMany([{"name": "example", "password": "example", "admin": true}])
> db.inventory.find({})
```

## Use cURL
```
curl --data-ascii '{ "name":"example", "password":"example" }' http://localhost:8080/api/authenticate
```

