# Node-TypeScript-Gulp-VsCode-Boilerplate

This is a Boilerplate project to start simple NodeJS 
projects. It supports TypeScript 2.0, since I like a 
strongly typed language support. It transpiles using 
Gulp and supports debugging in VsCode.

## Packages
All packages and type definitions are retieved using 
npm. Lodash is included, as it can be used in most 
applications. I consider it a basic library. The 
package.json is as follows:

{
  "name": "boilerplate",
  "version": "1.0.0",
  "description": "A ode-TypeScript-Gulp-VsCode-Boilerplate project",
  "main": "app.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "Toto",
  "license": "ISC",
  "devDependencies": {
    "@types/lodash": "^4.14.38",
    "@types/node": "^6.0.46",
    "del": "^2.2.2",
    "gulp": "^3.9.1",
    "gulp-sourcemaps": "^2.1.1",
    "gulp-tslint": "^6.1.2",
    "gulp-typescript": "^3.0.2",
    "nodemon": "^1.11.0",
    "path": "^0.12.7",
    "tslint": "^3.15.1",
    "typescript": "^2.0.3"
  },
  "dependencies": {
    "lodash": "^4.16.4"
  }
}

