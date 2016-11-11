# Node-TypeScript-Gulp-VsCode-Boilerplate

This is a Boilerplate project to start simple NodeJS 
projects. It supports TypeScript 2.0, since I like a 
strongly typed language support. It transpiles using 
Gulp and supports debugging in VsCode.

## Basic usage
Just start coding your app in app/app.ts. It is defined 
as the entrypoint of the application. To start transpiling
.ts files into .js files just open a command prompt in the
root folder and type 'gulp'. Alternatively you can run it 
as a task in VsCode. Just open the command line with CRTL-P
and type 'task' followed by a space. Choose 'default' from 
the dropdown.

## Packages
All packages and type definitions are retieved using 
npm. Lodash is included, as it can be used in most 
applications. I consider it a basic library. The 
package.json is as follows:

```package.json
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
```
## Gulp Tasks
Gulp is basically used as a transpiling system for the 
TypeScript files. The default task runs a watcher, which 
Lints and transpiles the .ts files. The generated sourcemaps
and .ja files are placed directly beside the .ts files.
There is also a task to clean the project of the enerated
files. 

## TypeScript Options
For some reason it does not transpile, when target is not 
set to 'es6'.

```tsconfig.json
{
    "compilerOptions": {
        "module":"commonjs",
        "sourceMap": false,
        "noEmitOnError": true,
        "target": "es6"
    },
    "exclude": [
        "node_modules/"
    ]
}
```

