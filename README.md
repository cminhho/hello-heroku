How to Deploy a Node.js App to Heroku
# Getting Started
- Go ahead and go to Heroku.com and create your free account.
- Tools needed: Node and npm, Heroku Toolbet, Git bash
- Login into Heroku: $ heroku login

# Creating a Simple Node Application
	- Creating a your application: use a git repo
	- Update package.json
{
  "name": "hello-heroku",
  "scripts": {
    "start": "node server.js"
  },
  "dependencies": {}
}
	- Install npm package and bower dependencies
	- Next up is our server.js file.
	- Run: $ node server.js
### Deploy your node app
	- Create the remote repo: $ heroku create
	- Rename your application: $ heroku apps:rename hello-heroku --app <your app name>
### Deploying code: $ git push heroku master
### View your application in browser
	- $ heroku open
	- Go ahead and visit that in browser: http://hello-heroku.herokuapp.com

# Using a Current Heroku App
	- Download the Heroku Toolbelt
	- Login: $heroku login
	- Add your public key: heroku keys:add
	- Pull down your current application: $ heroku git:clone -a app-name
	- Make your improvements
	- Git add and commit your$  changes
	- Push back to heroku: $ git push heroku master

# References
	- https://scotch.io/tutorials/how-to-deploy-a-node-js-app-to-heroku
