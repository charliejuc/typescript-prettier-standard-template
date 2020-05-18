# Typescript prettier-standard template
A simple template to initiate writing typescript code with linter and basic build commands.

Dependecies Installation:
```bash
yarn install

//OR

npm install
```

Available commands(package.json):
```JSON
"scripts": {
    "build": "npm-run-all clean tsc",
    "dev": "npm-run-all build --parallel tsc:watch nodemon",
    "lint": "prettier-standard --lint",
    "test": "npm-run-all lint",
    "tsc": "tsc",
    "tsc:watch": "tsc --watch",
    "clean": "rimraf dist",
    "format": "prettier-standard --format",
    "nodemon": "nodemon --watch dist",
    "start": "node dist/index.js"
}
```
