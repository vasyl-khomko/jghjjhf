# :warning: Unmaintained

This project has been **archived** and is considered **outdated** and **unmaintained**.

With the massive rise of the CLI tools by each major JavaScript Web frameworks, it was become irrelevant to pursue the quest of being a competitive project scaffolder for modern Web project.

We officialy advise to use the coresponding CLI tools for the framework you use:

- [create-react-app](https://github.com/facebook/create-react-app) for [React](https://reactjs.org/)
- [Vue CLI](https://cli.vuejs.org/) for [Vue.js](https://vuejs.org/)
- [Angular CLI](https://cli.angular.io/) for [Angular](https://angular.io/)

Of course, we have some regrets regarding our users, Yeoman users and some goals we had with Fountain (like giving important tool choices to users, harmonizing projects configurations between frameworks...) but still, you can use official CLI tools with confidence as they are great project which went further for development experience and Web optimization.

# Fountain Webapp Generator
[![Build Status](https://travis-ci.org/FountainJS/generator-fountain-webapp.svg?branch=master)](https://travis-ci.org/FountainJS/generator-fountain-webapp) [![codecov](https://codecov.io/gh/FountainJS/generator-fountain-webapp/branch/master/graph/badge.svg)](https://codecov.io/gh/FountainJS/generator-fountain-webapp) [![Slack](http://slackin.fountainjs.io/badge.svg)](http://slackin.fountainjs.io/) [![OpenCollective Backers](https://opencollective.com/fountainjs/backers/badge.svg?color=blue)](#backers) [![OpenCollective Sponsors](https://opencollective.com/fountainjs/sponsors/badge.svg?color=blue)](#sponsors)

> This Yeoman generator allows you to start any Webapp with the best Developer Experience out of the box!

> No matter what framework or module management you want to use, we got you covered with a cutting edge working configuration.

> We use [Gulp 4](http://gulpjs.com/) as a task manager but we'll ask you questions about:
- Framework: React, Angular 2, Angular 1, Vue 2
- Modules management: Webpack, SystemJS, none
- JS preprocessor: Babel, TypeScript, none
- CSS preprocessor: Sass, Stylus, Less, none

This generator is the entry point of the Yeoman Fountain generators for webapps. It can be considered as the v2 of [generator-gulp-angular](https://github.com/Swiip/generator-gulp-angular).

## Generator Fountain Webapp structure

To take profit of the best of the Yeoman infrastructure, we heavily relies on the composability natures of the generators.

Thereby, each needs of your future application will be addressed by a dedicated Yeoman generator (each will be used depending of the options you selected or not).

More informations in [DESIGN.md](http://fountainjs.io/doc/design).


### Web framework layer
This generators can be used directly to bypass the framework question.

[![React](http://fountainjs.io/assets/imgs/react.png)](https://github.com/FountainJS/generator-fountain-react) [![Angular 1](http://fountainjs.io/assets/imgs/angular1.png)](https://github.com/FountainJS/generator-fountain-angular1) [![Angular 2](http://fountainjs.io/assets/imgs/angular2.png)](https://github.com/FountainJS/generator-fountain-angular2) [![Vue 2](http://fountainjs.io/assets/imgs/vue.png)](https://github.com/FountainJS/generator-fountain-vue)

### Web tooling layer
[![Gulp](http://fountainjs.io/assets/imgs/gulp.png)](https://github.com/FountainJS/generator-fountain-gulp) [![ESLint](http://fountainjs.io/assets/imgs/eslint.png)](https://github.com/FountainJS/generator-fountain-eslint) [![BrowserSync](http://fountainjs.io/assets/imgs/browsersync.png)](https://github.com/FountainJS/generator-fountain-browsersync) [![Karma](http://fountainjs.io/assets/imgs/karma.png)](https://github.com/FountainJS/generator-fountain-karma)

### Module management layer
[![Webpack](http://fountainjs.io/assets/imgs/webpack.png)](https://github.com/FountainJS/generator-fountain-webpack) [![SystemJS](http://fountainjs.io/assets/imgs/systemjs.png)](https://github.com/FountainJS/generator-fountain-systemjs) [![Bower](http://fountainjs.io/assets/imgs/bower.png)](https://github.com/FountainJS/generator-fountain-inject)


### Usage

### Requirement Node 6+ && NPM 3+
This generator is targeted to be used with Node >= 6.0.0 and NPM => 3.0.0. You can check your version number with the command
```
node --version && npm --version
```

### Install

##### Install required tools `yo`:
```
npm install -g yo
```

##### Install `generator-fountain-webapp`:
```
npm install -g generator-fountain-webapp
```


### Run

##### Create a new directory, and go into:
```
mkdir my-new-project && cd my-new-project
```

##### Run `yo fountain-webapp`, and select desired technologies:
```
yo fountain-webapp
```
#### Use NPM scripts

- `npm run build` to build an optimized version of your application in /dist
- `npm run serve` to launch a browser sync server on your source files
- `npm run serve:dist` to launch a server on your optimized application
- `npm run test` to launch your unit tests with Karma
- `npm run test:auto` to launch your unit tests with Karma in watch mode


#### Or Gulp tasks

If you have [`gulp-cli`](https://www.npmjs.com/package/gulp-cli) installed in global packages you can use equivalent:

- `gulp` or `gulp build`
- `gulp serve`
- `gulp serve:dist`
- `gulp test`
- `gulp test:auto`

**If you don't have [`gulp-cli`](https://www.npmjs.com/package/gulp-cli) installed in global, you should have this error:**
> /usr/local/lib/node_modules/gulp/bin/gulp.js:121 gulpInst.start.apply(gulpInst, toRun); TypeError: Cannot read property 'apply' of undefined

### Sub-generators

If you want to access sub-generators, you have to globally install one of the following generators:
- [generator-fountain-react](https://github.com/FountainJS/generator-fountain-react)
- [generator-fountain-angular2](https://github.com/FountainJS/generator-fountain-angular2)
- [generator-fountain-angular1](https://github.com/FountainJS/generator-fountain-angular1)
- [generator-fountain-vue](https://github.com/FountainJS/generator-fountain-vue)

### [Start development](http://fountainjs.io/doc/usage/#use-npm-scripts)

***

## Backers

Support us with a monthly donation and help us continue our activities.
[![Backers](https://opencollective.com/fountainjs/backers.svg)](https://opencollective.com/fountainjs#support)

## Sponsors

Become a sponsor and get your logo on our website fountainjs.io and on our README on Github with a link to your site.
[![Sponsors](https://opencollective.com/fountainjs/sponsors.svg)](https://opencollective.com/fountainjs#support)

## [Changelog](https://github.com/FountainJS/generator-fountain-webapp/releases)


## [Contributing](http://fountainjs.io/doc/contributing)
