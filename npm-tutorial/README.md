#NPM - Node's package manager

##Checking the npm version
In order to check npm's version, type into the node repl:
```
$ npm --version
4.1.2
```

##Installing and upgrading NPM
npm comes pre - installed with node.
In order to update it, simply type into the node repl:
```
$ npm install npm -g
```

##Searching for npm modules
```
npm search <module-name>
```
Or, go to [NPM Registry](https://npmjs.com)

##Installing an npm module
```
$ npm install <module-name>
```
_Example:_
```
$ npm install express
```
The above command installs the module in a local node instance.
To install modules globally, add the _-g_ flag.
```
$ npm install express -g
```
_Note:_ NPM modules (If installed locally) should be installed in the directory of the node instance, or the npm module.

##Uninstall an npm module
```
$ npm uninstall <module-name>
```
_Example:_
```
$ npm uninstall express
```

##Updating a module
```
$ npm update <module-name>
```
_Example:_
```
$ npm update express
```

##Creating your own NPM module
###Creating an account in the NPM registry
1. Go to [NPM Registry](https://npmjs.com) and create an account
2. Remember the username and password

###Initializing your module
1. Create a directory with the name of the module you intend to create; for e.g. vatsal-module-1.
2. Navigate to the folder you've made.
3. Start the node/ npm REPL in the folder.
4. Type in `$ npm init`
5. The project will ask for various details like module name, version, etc.
6. Unless you want to change anything, keep the values default as mention between the parentheses.
7. Done! You've initialized your first node module!

###Writing your module
+ We will be writing a module which prints the current date and time.
+ After initializing your module, if not done already, navigate to the module's directory.
+ Create a file named index.js.
+ We are now telling the module what to do when started. Edit the scripts section in package.json to look like so:
```
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
	"start": "node index.js"
  },
```
+ Open and edit the index.js file to look like so:
```javascript
var date = new Date();	//Create new instance of Date object
console.log (date.getDate()  + "/" + // get Today's Date
			(date.getMonth() + 1) + "/" +	//get Today's Month and add 1 to it 
											//Done so, because Month is zero indexed
			(date.getYear - 100));
```

###Running the module
+ Navigate to the directory of your module
+ Type into the node REPL: `$ npm start`

###Publish your module
+ Change the version number to desired number in package.json. **Do not change anything else**.
+ Make sure you have an account on [NPM Registry](https://npmjs.com).
+ Type into the REPL:
```
$ npm login
```
+ Enter your credentials as required.
+ Type into the REPL:
```
$ npm publish
```
+ Hopefully, your module will get published successfully.
