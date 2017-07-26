<p align="center">
  <a href="http://materializecss.com/">
    <img src="http://materializecss.com/res/materialize.svg" width="150">
  </a>

  <h3 align="center">MaterializeCSS</h3>

  <p align="center">
    Materialize, a CSS Framework based on material design.
    <br>
    <a href="http://materializecss.com/"><strong>-- Browse the docs --</strong></a>
    <br>
    <br>
    <a href="https://travis-ci.org/Dogfalo/materialize">
      <img src="https://travis-ci.org/Dogfalo/materialize.svg?branch=master" alt="Travis CI badge">
    </a>
    <a href="https://badge.fury.io/js/materialize-css">
      <img src="https://badge.fury.io/js/materialize-css.svg" alt="npm version badge">
    </a>
    <a href="https://cdnjs.com/libraries/materialize">
      <img src="https://img.shields.io/cdnjs/v/materialize.svg" alt="CDNJS version badge">
    </a>
    <a href="https://david-dm.org/Dogfalo/materialize">
      <img src="https://david-dm.org/Dogfalo/materialize/status.svg" alt="dependencies Status badge">
      </a>
    <a href="https://david-dm.org/Dogfalo/materialize#info=devDependencies">
      <img src="https://david-dm.org/Dogfalo/materialize/dev-status.svg" alt="devDependency Status badge">
    </a>
    <a href="https://gitter.im/Dogfalo/materialize">
      <img src="https://badges.gitter.im/Join%20Chat.svg" alt="Gitter badge">
    </a>
    <br>
    * These badges are for the original Materialize, not the AMD-compatible version
</p>

## Note for AMD-compatible version

**Notice that this is NOT the offical AMD-compatible version, and I won't keep updating it with latest commit (just stable release), so just use `dist/js/materialize.js`.**

This modified version is tested and passed on [curl.js](https://github.com/cujojs/curl), I'm not sure that it would compatible with other AMD module.

After required it at the first time, please do `Waves.displayEffect()` to show waves, like this:

```js
require(['jquery']).next(['materialize'], function(Materialize){
    // add it when you required Materialize at the first time
    Waves.displayEffect();

    // do more things with Materialize here
});
```

For modified parts, see original issue here: https://github.com/Dogfalo/materialize/issues/634#issuecomment-183846293

## Table of Contents
- [Quickstart](#quickstart)
- [Documentation](#documentation)
- [Supported Browsers](#supported-browsers)
- [Changelog](#changelog)
- [Testing](#testing)
- [Contributing](#contributing)
- [Copyright and license](#copyright-and-license)

## Quickstart:
Read the [getting started guide](http://materializecss.com/getting-started.html) for more information on how to use materialize.

- [Download the latest release](https://github.com/ccloli/materialize/releases/latest) of materialize directly from GitHub.
- Clone the repo: `git clone https://github.com/ccloli/materialize.git`, `cd materialize` then `git checkout AMD-fix`.
- ~~Include the files via [cdnjs](https://cdnjs.com/libraries/materialize). More [here](http://materializecss.com/getting-started.html).~~
- Install with [npm](https://www.npmjs.com): `npm install github:ccloli/materialize#AMD-fix` (or replace `AMD-fix` to any modified version with `-amd` suffix like `v0.100.1-amd`).
- Install with [Bower](https://bower.io): `bower install https://github.com/ccloli/materialize.git#AMD-fix` (or replace `AMD-fix` to any modified version with `-amd` suffix like `v0.100.1-amd`).
- ~~Install with [Atmosphere](https://atmospherejs.com): `meteor add materialize:materialize`.~~ (Not sure if it works, try cloning the repo then try this [StackOverflow](https://stackoverflow.com/a/29579559))

## Documentation
The documentation can be found at <http://materializecss.com>. To run the documentation locally on your machine, you need [Node.js](https://nodejs.org/en/) installed on your computer.

### Running documentation locally
Run these commands to set up the documentation:

```bash
git clone https://github.com/ccloli/materialize
cd materialize
git checkout AMD-fix
npm install
```

Then run `grunt monitor` to compile the documentation. When it finishes, open a new browser window and navigate to `localhost:8000`. We use [BrowserSync](https://www.browsersync.io/) to display the documentation.

### Documentation for previous releases
Previous releases and their documentation are available for [download](https://github.com/ccloli/materialize/releases).

## Supported Browsers:
Materialize is compatible with:

- Chrome 35+
- Firefox 31+
- Safari 7+
- Opera
- Edge
- IE 10+

## Changelog
For changelogs, check out [the Releases section of materialize](https://github.com/Dogfalo/materialize/releases) or the [CHANGELOG.md](CHANGELOG.md).

## Testing
We use Jasmine as our testing framework and we're trying to write a robust test suite for our components. If you want to help, [here's a starting guide on how to write tests in Jasmine](CONTRIBUTING.md#jasmine-testing-guide).

## Contributing
Check out the [CONTRIBUTING document](CONTRIBUTING.md) in the root of the repository to learn how you can contribute. You can also browse the [help-wanted](https://github.com/Dogfalo/materialize/labels/help-wanted) tag in our issue tracker to find things to do.

## Copyright and license
Code copyright 2017 Materialize. Code released under the MIT license.
