# Fledgeling

## Requirements

At least version 5.2.0 of npm. (npx comes with npm from this version on)

## Installation

Fledgeling uses [`npx`](https://medium.com/@maybekatz/introducing-npx-an-npm-package-runner-55f7d4bd282b) for building. This means that the devDependencies can be installed globally instead of running `npm i` in the project root.
This helps avoid having multiple copies of the required node_modules for every project.

For the global approach all that is needed is:
```
npm i -g npm-run-all pug-cli gaze-cli
npm start
```

For a normal local approach use:
```
npm i
npm start
```

## Development

`npm start` will build and watch source files and start up Browsersync as a development server with live reloading.

## Production

`npm build` will build the project to the `dist` directory.


## Methodology

Fledgeling is meant to be a fairly plain boilerplate that provides a solid starting point for static websites. It avoids bundling assets for use with http2 multiplexing and async loading.

## Coming soon

- Pug utility mixins for async / lazy loading of assets via loadjs.
- Production scripts for minimizing / uglifying css, js.
- Production script for making `.copat` versions of css / js files (using postCSS / babel)
- Image compression script.