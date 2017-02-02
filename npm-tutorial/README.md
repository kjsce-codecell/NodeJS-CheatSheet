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
<<<<<<< HEAD

##Creating you own NPM module
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

###Publish your module
=======
>>>>>>> b06f47f27a1735e6349b62cfefe038b551f3e900
