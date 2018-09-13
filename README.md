<div align="center">
	<a href="https://github.com/webpack/webpack-cli">
		<img width="200" height="200" src="https://webpack.js.org/assets/icon-square-big.svg">
	</a>
</div>
<p align="center">
  A scaffolding tool for webpack.
</p>
<br>

[![npm](https://img.shields.io/npm/v/webpack-cli.svg)](https://www.npmjs.com/package/webpack-cli)
[![Build Status](https://travis-ci.org/webpack/webpack-cli.svg)](https://travis-ci.org/webpack/webpack-cli)
[![Build status](https://ci.appveyor.com/api/projects/status/c2a37nlrfv9mg64f?svg=true)](https://ci.appveyor.com/project/ev1stensberg/webpack-cli)
[![Dependency Status](https://david-dm.org/webpack/webpack-cli.svg)](https://david-dm.org/webpack/webpack-cli)
[![Code Climate](https://codeclimate.com/github/webpack/webpack-cli/badges/gpa.svg)](https://codeclimate.com/github/webpack/webpack-cli)
[![chat on gitter](https://badges.gitter.im/webpack/webpack.svg)](https://gitter.im/webpack/webpack)
[![Greenkeeper badge](https://badges.greenkeeper.io/webpack/webpack-cli.svg)](https://greenkeeper.io/)
[![Install Size](https://packagephobia.now.sh/badge?p=webpack-cli)](https://packagephobia.now.sh/result?p=webpack-cli)

# Webpack CLI

* [About](#about)
* [Getting Started](#getting-started)
* [How It Works](#how-it-works)
* Commands
  - [`webpack-cli init`](./packages/init/README.md#webpack-cli-init)
  - [`webpack-cli add`](./packages/add/README.md#webpack-cli-add)
  - [`webpack-cli info`](./packages/info/README.md#webpack-cli-info)
  - [`webpack-cli migrate`](./packages/migrate/README.md#webpack-cli-migrate)
  - [`webpack-cli remove`](./packages/remove/README.md#webpack-cli-remove)
  - [`webpack-cli generate-plugin`](./packages/generate-plugin/README.md#webpack-cli-generate-plugin)
  - [`webpack-cli generate-loader`](./packages/generate-loader/README.md#webpack-cli-generate-loader)
  - [`webpack-cli serve`](./packages/serve/README.md#webpack-cli-serve)
  - [`webpack-cli update`](./packages/update/README.md#webpack-cli-update)
* [webpack.config.js](https://webpack.js.org/concepts/configuration/)
* [Contributing and Internal Documentation](#contributing-and-internal-documentation)

## About

Webpack CLI is a CLI tool for providing a flexible set of commands for developers to increase speed when setting up a custom webpack project. As of webpack v4, webpack is not expecting a configuration file but in many cases, developers want to create a more custom webpack configuration based on their use-cases and needs. Exactly all of these cases with webpack CLI we are providing a set of tools so improve the setup of custom webpack configuration. 

### How to install

When you have followed the [Getting Started](https://webpack.js.org/guides/getting-started/) guide of webpack then webpack CLI is already installed!

Otherwise `npm install --save-dev webpack-cli` will install it. 

### Commands

In order to simplify many common tasks when using webpack in your projects, webpack CLI provides different commands according to their use-cases.

webpack CLI is organized as a [multi-package repository](https://github.com/lerna/lerna) and every command is developed in the `packages` Folder.

## Getting started

When you have followed the [Getting Started](https://webpack.js.org/guides/getting-started/) guide of webpack then webpack CLI is already installed! Otherwise you would need to install webpack CLI and the packages you want to use. If we want to use the `init` functionality to create a new `webpack.config.js` configuration file:

```sh
npm i webpack-cli @webpack-cli/init
npx webpack-cli init
```

After asking multiple questions related to your project and as a result create a webpack.config.js based on your selected answers. 

## How it works

With v3 of webpack CLI we introduced a scaffolding as an integral part of it. The idea is that creating complex webpack configuration for different use-cases can be difficult and we want to make it easy for everyone to be able to create and share their solutions. For this purpose `webpack-scaffold` was created. It is a utility suite for creating these addons. It contains functions that could be of use for creating an addon yourself.

For a much more comprehensive guide, we recommend reading our [Scaffolding](./SCAFFOLDING.md) documentation or checkout the example project [How do I compose a webpack-addon?](https://github.com/ev1stensberg/webpack-addons-demo).

## Contributing and Internal Documentation

The webpack family welcomes any contributor, small or big. We are happy to elaborate, guide you through the source code and find issues you might want to work on! To get started have a look at our [documentation on contributing](CONTRIBUTING.md).

