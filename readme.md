# React Redux Starter Kit

[![Build Status](https://travis-ci.org/imjohsep/react-redux-starter-kit.svg?branch=master)](https://travis-ci.org/imjohsep/react-redux-starter-kit)
[![dependencies Status](https://david-dm.org/imjohsep/react-redux-starter-kit/status.svg)](https://david-dm.org/imjohsep/react-redux-starter-kit)
[![devDependencies Status](https://david-dm.org/imjohsep/react-redux-starter-kit/dev-status.svg)](https://david-dm.org/imjohsep/react-redux-starter-kit?type=dev)

## What is this

This is a super simple example project utilizing React, Redux, and Webpack.

### Includes

* [Hot Module Replacement](https://webpack.github.io/docs/hot-module-replacement.html): When possible, changes will be patched in to the running application.
* [Linting](http://eslint.org/): Javascript code will be passed through a configurable linter. Configure it. Love it.
* [CSS Modules](https://github.com/css-modules/css-modules): Stylesheets can loaded into Javascript and accessed through Object properties.
* [SASS](https://github.com/jtangelder/sass-loader): Because CSS is a hack and painful without a preprocessor.
* [File Loading](https://github.com/webpack/file-loader): Load images, fonts, etc.
* [Testing!](https://mochajs.org/): Because they make coding more rewarding.

## Commands

All pre-baked commands are defined in `package.json` and are run through `npm`.
You should look there to see what they are doing in case you need to make any modification.

| Command                            | Purpose                 |
|------------------------------------|-------------------------|
| `npm start`                        | starts the local server |
| `npm run clean`                    | deletes contents of dist directory |
| `npm run compile`                  | runs `clean` and compiles new build |
| `npm run compile:stats`            | runs `compile` and additionally outputs json stats file |
| `npm run check`                    | checks for updates to installed packages |
| `npm run test(:watch)`             | executes all tests, optionally watch for changes |
| `npm run test:coverage`            | executes tests and generates coverage report |
| `npm run test:unit(:watch)`        | executes unit tests |
| `npm run test:integration(:watch)` | executes integration tests |
| `npm run test:karma(:watch)`       | __@todo__ executes tests using the Karma test runner

## Getting Started

In general, there is a lot of business to take care of to make this repo your own.
This project attempts to reduce some of setup business to provide a clean slate for
your new project. Just follow the following steps to get started.

### Step 1. Clone the Repo

When you `git clone` this project be sure to add your project name on
the end of the command like so:

```sh
git clone https://github.com/imjohsep/react-redux-starter-kit.git <my_project_name>
```

You will also want to break from the current git directory with `sudo rm -r .git`.
Then just reinitialize git with `git init`.

### Step 2. Initializing the Package

Run `npm init` at the root of the project and overwrite the package.json
details that don't correspond to your new project.

Install all the dependencies:

```sh
npm install
```

#### Alternative Initialization

Run `yarn init` to reconfigure the package.json file. I prefer yarn to init
our package because it asks to override more of the package details than npm; in
addition to all of the performance improvements.

Once our package.json file is updated you can `yarn install` the dependencies listed
in the yarn.lock file.

### Step 4. Start the App

`npm start`

That's about it! This starterkit is ready to go. It is recommended you
grow accustomed with the HomeContainer and Home Components first. Then
work your way over to the Counter Container and Component, as these
more fully implement Redux action, reducers, and state.

## Optional

### Step 5. Switch the Favicon

Generate the complete range of images using this [site](http://www.favicomatic.com/).

Move all of the generated files into the `src/static/favicon` directory and replace
the link tags in the `src/index.html` file.

### Step 6. Setup Deployment

This project comes with a procfile and travis.yml files, so it is setup to deploy
to heroku with TravisCI. You can use those services to quickly and freely deploy
your project, but you will need to updat those configs. See the following for more information on that:

[Heroku Deployment on Travis](https://docs.travis-ci.com/user/deployment/heroku)