![gitline sample](https://github.com/blecher-at/gitline/blob/master/doc/gitline.png)

gitline - a git history to html renderer implemented in javascript (typescript).
===========

Idea is to have this on a central server or your local machine, to keep tabs on what your team is doing :)
needs a json file as input (generated with git2json)

Tries to be aware of your branching scheme. It will autodetect the category and assignment of branches and groups commits accordingly.

Future developments will include:
- include meaningful sample data
- show author and timestamp metadata
- include configuration dialog to configure your teams branching patterns (custom grouping/colors etc.)
- filtering functionality (by branches, author etc.)
- support other input formats like github-api
- statistics 

Buidling
------------------
- Install node.js
- Install typescript "npm install -g typescript"
- Install git2json (https://github.com/blecher-at/git2json/blob/master/README.md)
- run tsc to compile this

Creating Sample data
-----------
- run "git json > myfile.json" (in a cronjob presumably)
- point index.html to the json file.


Imports
-------
Programming Language: Typescript http://www.typescriptlang.org/

SVG Rendering: JSGL http://www.jsgl.org/

JQuery: https://jquery.org/
