pyDocker
========

 Python package documenter.

 pyDocker is a simple package documentor that uses python to process packages into json data.
 and angular js templates for the front-end documentation app.

 pyDocker is currently in an alpha stage so things can drastically change in future versions.

###Features

1. python to json intermediate conversion.
2. seperation of data and logic layers.
2. dynamic frontend can be edited as per new requirements.
3. support for help pages written in markdown.

##Intergations

1. Python 2.6+
2. Angular JS
3. google prettify
4. MarkdownConverter.js

## Getting Started

check that the pyDocker package is accessible by python through the sys.path
pyDocker requires a python file to be placed in the package that you want to document, there is no specific naming requirement but for keeping to standards you should name it makeDocs.py, a sample config file will help you get started.

whenever u want to update your docmentation to the code changes, you can run it file to generate the documentation again, all settings are on overwrite, for automation purposes it is recommended that you either use CRON or GRUNT to run this file on the specified intervals or changes.

###Options

 * deprecatedList : if you want to make a list of all deprecated functions in the package.
 * listImports : if u want to list all the imports in a module or package
 * docformat : currently has a custom docstring parser, but future release will be md and rst supported.
 * output : currently output is a json intermediate, future support for static htm is planned
 * loadMode : (local/webserver) : this option is important for the frontend as ajax requests are not possible on       local html files, therefore this implements a hack to load the json files.


## License

(C) Savio Fernandes 2014, released under an MIT license
