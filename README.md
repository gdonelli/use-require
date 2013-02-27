use-require
===

Import your node files without specifying their full path


Setup
=
You need to specify where to find your libraries, as soon as your app starts:

require('use-require').setup([ <TheDirectoryContainingYourCode> ]);

for example:
require('use-require').setup([ __dirname + '/code' ]);

Usage
=
Once the module is setup, it creates a global function `use` which can be used in to include your own modules. 

for example:
var mylib = use('mylib');

