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
