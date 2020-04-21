# PAN-CHAY-AT 
The Basic Shopify APP

This is the first step to build a Commercial Application by using Shopify Platform [shopify](https://www.shopify.dev/concepts/shopify-introduction).


## Overview

This is the basic version of an automated local search marketing platform for businesses and brands and gaussips. That Application build by GraphQL APIs in Node.js using ES6, Koa.js, react.js, next.js, firebase authentication and shopify polaris library. It Helps you stay productive by following best practices. Follows [latest Javascript syntax guide](http://www.ecma-international.org/ecma-262/6.0/).

### Authentication process

| Feature                                | Summary                                                                                                                                                                                                                                                     |
|----------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

| Authentication with Shopify-Partner-developper credentials.                  	 	 | Supports authentication using [SHOPIFY_API_KEY= '##########$$$$$***',    SHOPIFY_API_SECRET_KEY='@@#######################$$', API_VERSION='2019-10'](https://shopify.dev/tutorials/rotate-revoke-api-credentials).  ||

When authenticating merchants, Shopify redirects from the app authorization prompt back to the app. Our app needs an HTTPS address to be able to do this. Since the localhost:3000 isn’t a public address, we will use ngrok to create a secure tunnel from the public internet to the local machine. [HOST='https://@#$##example.ngrok.io']                | Restart the server using [nodemon](https://github.com/remy/nodemon) in real-time anytime an edit is made, with babel compilation and eslint.                                                                                                                                                                                                     
|Mainly GraphQL APIS are used for the better allignment of other libraries and packages of shopify, to achive the high performance.  [shopify_graphQLexploral](https://shopify.dev/tools/graphiql-admin-api) [graphQL the query language](https://graphql.org/)
| Run with ngrok and tests before any commit is made locally, making sure that only tested and quality code is committed
|Do server side rendering with Next.js [next.js](https://nextjs.org/docs)

- CORS support via [cors](https://github.com/koajs/cors)

## Getting Started

Clone the repo:
```sh
git clone current-repo
```

Install :
```js
npm install -g

npm install ngrok -g
```

Set environment (vars):
```sh
edit .env
```

Start server:
```sh
# Start server

# First Step
run in the terminal : ngrok http 3000 , 

and get the ngrok session status like [https://$$@1082d.ngrok.io]. Copy that ngrok value and paste it to at env file 'Host = https://$$@1082d.ngrok.io', paste the same value at 'APP url and Whitelisted redirection URL(s)'
 

# Second Step 
in another terminal run : npm run dev

then open this url with your ngrok value : https://YOURNGROKADDRESS.io/auth?shop=YOURTESTSTORE.myshopify.com

# Selectively set DEBUG env var to get logs
yarn start:debug
```
Refer [debug](https://www.npmjs.com/package/debug) to know how to selectively turn on logs.

```

#### API logging
Logs detailed info about each api request to console during development.


## Contributing

Contributions, questions and comments are all welcome and encouraged. For code contributions submit a pull request with unit test.

