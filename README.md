# restapi
Boiler plate rest api using node.js, epress router and jsonwebtoken

### Usage:
You must have node.js/npm and mongoDb installed

In root :
```
npm install

```

Change config file to match your configuration

Then:
```
node server.js

```
It should print something like:

```
' Magic happens on port 8080 '

```

Very simple. The boiler contain a token generation and checkup logic 
(very basic) as middleware and provide basic routing structure.

Just start from there and you can vuild a restapi in hours.

##### PS: jsonwebtoken npm seem to be changed need to replace it in package.json and in server.js to use another jwt module
