D3 Capital Cities Force-Directed Graph
======================================

About
-----
This project is an example of using D3 to generate a force-directed graph

Usage
-----
```bash
npm start
```

will start an HTTP server with the demo running.

Each node represents a country.  Hovering over the node will give a tooltip with the country name.

Building
--------
You can build the project using:
```bash
$ npm run build
```
This will create `dist/bundle.min.js` which is a self-executing Javascript bundle which can be used in non-ES2015-compliant browsers.  This is probably what you want to do upon release if you are writing a library for general use.

For a specific webapp, it is better to run:
```bash
$ npm run bundle
```
Which will create `public/js/main.bundle.js`.  This means that all code and JSPM dependencies will be bundled into a single Javascript file which will be requested as soon as one of the dependencies is required.  **Once you have done this it will keep using this bundle**.  That means that any changes to the original source will **not** be reflected in the website, until you run `npm run bundle` again, or alternatively remove it with `npm run clean`.

Author
------
[Guy Griffiths](https://github.com/guygriffiths)


