# Note

sample code for [Heroku Getting Started for Nodejs](https://devcenter.heroku.com/articles/getting-started-with-nodejs)

## config

* config vsc task for npm

## remote server
```command
heroku create
git push keroku master
heroku ps:scale web=1
```
and launch browser to generated URL
add argument to URL path
```command
heroku open
heroku open cool
```
## local server
* npm install
* start local server
```command
heroku local web 
```

## console
starts a remote connection to a one-off dyno
```command
heroku run node
heroku run bash
```
Uses port 5000, will not work behind proxy server.

## env
heroku local refers to the .env file when the server starts up.
heroku cloud use commands to config
```command
heroku config
heroku config:set TIMES=2
```

# node-js-getting-started

A barebones Node.js app using [Express 4](http://expressjs.com/).

This application supports the [Getting Started with Node on Heroku](https://devcenter.heroku.com/articles/getting-started-with-nodejs) article - check it out.

## Running Locally

Make sure you have [Node.js](http://nodejs.org/) and the [Heroku Toolbelt](https://toolbelt.heroku.com/) installed.

```sh
$ git clone git@github.com:heroku/node-js-getting-started.git # or clone your own fork
$ cd node-js-getting-started
$ npm install
$ npm start
```

Your app should now be running on [localhost:5000](http://localhost:5000/).

## Deploying to Heroku

```
$ heroku create
$ git push heroku master
$ heroku open
```
or

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

## Documentation

For more information about using Node.js on Heroku, see these Dev Center articles:

- [Getting Started with Node.js on Heroku](https://devcenter.heroku.com/articles/getting-started-with-nodejs)
- [Heroku Node.js Support](https://devcenter.heroku.com/articles/nodejs-support)
- [Node.js on Heroku](https://devcenter.heroku.com/categories/nodejs)
- [Best Practices for Node.js Development](https://devcenter.heroku.com/articles/node-best-practices)
- [Using WebSockets on Heroku with Node.js](https://devcenter.heroku.com/articles/node-websockets)
