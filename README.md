# Sample Babel-Register setup for WebStorm

What was done to set this up:

* Install the following packages:
 
```bash
npm install --save babel-register
npm install --save babel-preset-es2015 babel-register
```

* Add a `.babelrc` file to indicate ES2015 presets

* Set up project to use ES6 (Preferences -> Languages & Frameworks -> JavaScript -> ECMAScript 6)

* Install Node 4.x, and configure the run configuration to use it. (Run -> Edit Configurations -> Node Interpreter)
    
    
What it does:

`index.js` is the entry point. It loads `babel-register`, and proceeds to load two modules which use ES6 features not available to Node 4.x

You can add breakpoints in either `a.js` or `b.js` to verify that it works.


The entire `./idea` folder is included in this repo for reference, but you'll probably need to adjust to your local config.


