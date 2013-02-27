use-require
===

Imagine the `require` command to import your files, without having to specify the full path


Setup
=
You need to specify where to find your libraries, as soon as your app starts:

`require('use-require').setup([ <TheDirectoryContainingYourCode> ]);`

for example:

`require('use-require').setup([ __dirname + '/code' ]);`

Usage
=
Once the module is setup, it creates a global function `use` which can be used to include your own modules. 

for example:

`var mylib = use('mylib');`

