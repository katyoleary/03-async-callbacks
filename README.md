![CF](https://camo.githubusercontent.com/70edab54bba80edb7493cad3135e9606781cbb6b/687474703a2f2f692e696d6775722e636f6d2f377635415363382e706e67) 03: Asynchronous Callbacks
===

## Submission Instructions
* Work in a fork of this repository
* Work in a branch on your fork
* Write all of your code in a directory named `lab-` + `<your name>` **e.g.** `lab-susan`
* Open a pull request to this repository
* Submit on canvas a question and observation, how long you spent, and a link to your pull request

## Resources
* [fs module docs](https://nodejs.org/api/fs.html)

## Configuration
Configure the root of your repository with the following files and directories. Thoughfully name and organize any aditional configuration or module files.
* **README.md** - contains documentation
* **.gitignore** - contains a [robust](http://gitignore.io) `.gitignore` file
* **.eslintrc** - contains the course linter configuratoin
* **.eslintignore** - contains the course linter ignore configuration
* **package.json** - contains npm package config
  * create a `lint` script for running eslint
  * create a `test` script for running tests
* **lib/** - contains module definitions
* **data/** - contains the text files used by the program
* **\_\_test\_\_/** - contains unit tests

## Testing
##### File Reader Module Tests
* Use `describe` and `it` methods to define descriptive tests and increase readability
* Each `it` callback should aim to test a small, well defined, feature of a function
* Write tests to ensure that the reader function rejects errors with invalid file paths
* Write tests to ensure that the reader function correctly resolves mapped string data for an array of file paths

## Feature Tasks
##### File Reader Module
In the lib/ directory, create a `reader.js` module that exports a single function. The reader module should take an array of three file paths and `console.log` the first 8 bytes (in hex) of each file. You will need to create these files yourself and *be sure* to make their content and length different.  Regardless of file size, all three files should be read and logged in the order **one.txt**, **two.txt**, **three.txt**.

* The file reader module should have the function signature `(paths, callback) => undefined`
* On failure, the file reader module should invoke the callback with an error `callback(error)`
* On success, the file reader module should invoke the callback with `null` as the first parameter and the result as the second parameter - `callback(null, result)`

##  Documentation
In your `README.md` describe the exported values of the module you have defined. Your file reader function description should include it's airty (expected number of parameters), the expected data for each parameter (data-type and limitations), and it's behavior (for both valid and invalid use). Feel free to add any additional information to your `README.md` that seems relavent and useful.

