METHOD 1 (easier):

make directory for package - PACKAGE_NAME
cd into PACKAGE_NAME
$ npm init
touch index.js file with module.exports 
$ npm link
cd into root
make directory "app folder"
cd into app folder
$ npm link PACKAGE_NAME
touch index.js file 
require the new package (using require syntax)
use the package for whatever it does (e.g. sayHello function)
$ node index.js


METHOD 2 (longer):

make directory for package - PACKAGE_NAME
cd into PACKAGE_NAME
$ npm init
touch index.js file with module.exports
run npm pack
move .tgz file to root
decompress .tgz file
cd into root
cd into the created folder (its called package) 
$ npm link
cd into root
make directory "app folder"
cd into app folder
$ npm link PACKAGE_NAME
touch index.js file 
require the new package (using require syntax)
use the package for whatever it does (e.g. sayHello function)
$ node index.js
