# How to Deploy a Node.js App to Heroku
- See demo: https://hello-heroku-node.herokuapp.com/

## Getting Started
- Go ahead and go to [Heroku.com](Heroku.com) and create your free account.
- Tools needed: [Node.js](http://nodejs.org/) and npm, [Heroku Toolbelt](https://toolbelt.heroku.com/), Git bash

## Creating a Simple Node Application

```sh
$ git clone git@github.com:heroku/hello-heroku.git # or clone your own fork
$ cd hello-heroku
$ npm install
$ node server.js
```

Your app should now be running on [localhost:8080](http://localhost:8080/).

## Deploy your node app

```
$ heroku login
$ heroku create
$ heroku apps:rename hello-heroku --app <your app name>
$ git push heroku master
$ heroku open
```

## Using a Current Heroku App

```
- Login: $heroku login
- Add your public key: heroku keys:add
- Pull down your current application: $ heroku git:clone -a app-name
- Make your improvements
- Git add and commit your$  changes
- Push back to heroku: $ git push heroku master
```

## References
- https://devcenter.heroku.com/articles/getting-started-with-nodejs
- https://scotch.io/tutorials/how-to-deploy-a-node-js-app-to-heroku
