<<<<<<< HEAD
![license](https://img.shields.io/github/license/pattern-lab/patternlab-php.svg)
[![Packagist](https://img.shields.io/packagist/v/pattern-lab/edition-mustache-standard.svg)](https://packagist.org/packages/pattern-lab/edition-mustache-standard) [![Gitter](https://img.shields.io/gitter/room/pattern-lab/php.svg)](https://gitter.im/pattern-lab/php)

# Pattern Lab Standard Edition for Mustache

The Pattern Lab Standard Edition for Mustache is the evolution of Pattern Lab 1. Pattern Lab is still, at its core, a prototyping tool focused on encouraging communication between content creators, designers, devs, and clients. It combines platform-agnostic assets, like the [Mustache](http://mustache.github.io/)-based patterns, with a PHP-based "builder." Pattern Lab 2 introduces [the beginnings of an ecosystem](http://patternlab.io/docs/advanced-ecosystem-overview.html) that will allow teams to mix, match and extend Pattern Lab to meet their specific needs. It will also make it easier for the Pattern Lab team to push out new features. Pattern Lab Standard Edition for Mustache is just [one of the four PHP-based Editions currently available](http://patternlab.io/docs/installation.html).

## Demo

You can play with a demo of the front-end of Pattern Lab at [demo.patternlab.io](http://demo.patternlab.io).

## Requirements

To use the basic features of Pattern Lab to compile patterns, you must have **PHP 5.4+** installed. On Mac OS X Pattern Lab should work "out of the box." If you're on Windows you can [download PHP from PHP.net](http://windows.php.net/download/). Pattern Lab comes with its own built-in web server.

Pattern Lab uses [Composer](https://getcomposer.org/) to manage project dependencies. It's required if you want to install Pattern Lab using Composer's `create-project` command or if you want to upgrade Pattern Lab in the future.

## Installing

There are two methods for downloading and installing the Standard Edition for Mustache:

* Download a pre-built project
* Create a project based on this Edition with Composer

### Download a pre-built project

The fastest way to get started with Pattern Lab's Standard Edition for Mustache is to download the latest pre-built version from the [releases page](https://github.com/pattern-lab/patternlab-php/releases/latest).

### Use Composer to create a project

Pattern Lab uses [Composer](https://getcomposer.org/) to manage project dependencies.

#### 1. Install Composer

Please follow the directions for [installing Composer](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx) on the Composer website. We recommend you [install it globally](https://getcomposer.org/doc/00-intro.md#globally).

#### 2. Install the Standard Edition for Mustache

Use Composer's [`create-project` command](https://getcomposer.org/doc/03-cli.md#create-project) to install the Standard Edition for Mustache into a location of your choosing. To create a project do the following:

1. In a terminal window navigate to where you want to install Pattern Lab
2. Type `composer create-project pattern-lab/edition-mustache-standard patternlab2-example && cd $_`

This will install the Standard Edition for Mustache into a directory called `patternlab2-example` in your install location. When prompted choose the "demo" StarterKit. You will be automatically dropped into the project directory after the process is finished.

**Note:** If you clone or download this repository and use `composer install` to install the project dependencies you'll need to type the following to install the demo StarterKit:

    composer install-demo

Otherwise you'll have a very bare set-up of Pattern Lab.

## Get Up and Running

After installing do the following to start and view Pattern Lab:

1. In a terminal window navigate to the root of your project if you aren't there already
2. Type `php core/console --server --with-watch`

You should now be able to open [http://localhost:8080](http://localhost:8080) to see your generated site. Any changes you make in `./source/` will automatically rebuild your site and reload your browser.

As you get more comfortable with Pattern Lab you can [integrate it with a Gulp or Grunt workflow](http://patternlab.io/docs/advanced-integration-with-grunt.html) and drop some of the native Pattern Lab features like automatic browser reload. You can also check out [the list of plugins](http://patternlab.io/download.html).

## More Documentation

Obviously Pattern Lab is deeper than the install process. [Check out the documentation](https://patternlab.io/docs/) to learn about how to use patterns, how to modify the data used to populate those patterns, and about some advanced features.

## Migrating from Pattern Lab 1 to Pattern Lab 2

Pattern Lab 2 was a complete rewrite and reorganization of Pattern Lab 1. [Learn about the changes](http://patternlab.io/docs/changes-1-to-2.html). After installing the Standard Edition for Mustache do the following to migrate from Pattern Lab 1 to Pattern Lab 2:

1. Copy `./source` from your old project to your new install
2. Copy `./source/_patterns/00-atoms/00-meta/_00-head.mustache` to `./source/_meta/_00-head.mustache`
3. Copy `./source/_patterns/00-atoms/00-meta/_01-foot.mustache` to `./source/_meta/_00-foot.mustache`
4. Copy `./source/_data/annotations.js` to `./source/_annotations/annotations.js`

Everything else should work without changes.

## Need Pattern Lab 1?

The [source code for Pattern Lab 1](https://github.com/pattern-lab/patternlab-php/releases/tag/v1.1.0) is still available for download.

## Packaged Components

The Standard Edition for Mustache installs the following components:

* `pattern-lab/core`: [GitHub](https://github.com/pattern-lab/patternlab-php-core), [Packagist](https://packagist.org/packages/pattern-lab/core)
* `pattern-lab/patternengine-mustache`: [documentation](https://github.com/pattern-lab/patternengine-php-mustache#mustache-patternengine-for-pattern-lab-php), [GitHub](https://github.com/pattern-lab/patternengine-php-mustache), [Packagist](https://packagist.org/packages/pattern-lab/patternengine-mustache)
* `pattern-lab/plugin-reload`: [GitHub](https://github.com/pattern-lab/plugin-php-reload), [Packagist](https://packagist.org/packages/pattern-lab/plugin-reload)
* `pattern-lab/styleguidekit-assets-default`: [GitHub](https://github.com/pattern-lab/styleguidekit-assets-default), [Packagist](https://packagist.org/packages/pattern-lab/styleguidekit-assets-default)
* `pattern-lab/styleguidekit-mustache-default`: [GitHub](https://github.com/pattern-lab/styleguidekit-mustache-default), [Packagist](https://packagist.org/packages/pattern-lab/styleguidekit-mustache-default)

## List All of the Available Commands and Their Options

To list all available commands type:

    php core/console --help

To list the options for a particular command type:

    php core/console --help --[command]
=======
<p align="center">
  <img src='/patternlab.png' height="300" alt="Pattern Lab Logo" />
</p>

# Pattern Lab

This monorepo contains the core of Pattern Lab / Node and all related engines, UI kits, plugins and utilities. Pattern Lab helps you and your team build thoughtful, pattern-driven user interfaces using atomic design principles.

If you'd like to see what a front-end project built with Pattern Lab looks like, check out this [online demo of Pattern Lab output](http://demo.patternlab.io/).

[![Build Status](https://travis-ci.org/pattern-lab/patternlab-node.svg?branch=master)](https://travis-ci.org/pattern-lab/patternlab-node)
![current release](https://img.shields.io/npm/v/@pattern-lab/core.svg)
![license](https://img.shields.io/github/license/pattern-lab/patternlab-node.svg)
[![Coverage Status](https://coveralls.io/repos/github/pattern-lab/patternlab-node/badge.svg?branch=master)](https://coveralls.io/github/pattern-lab/patternlab-node?branch=master)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
[![node (scoped)](https://img.shields.io/node/v/@pattern-lab/patternlab-node.svg)]()
[![Join the chat at Gitter](https://badges.gitter.im/pattern-lab/node.svg)](https://gitter.im/pattern-lab/node)

## Using Pattern Lab

Refer to the [core usage guidelines](https://github.com/pattern-lab/patternlab-node/blob/master/packages/core/README.md#usage)

### Installation

Installation is still in flux due to the monorepo transition. Bear with us as we figure this out. Our intent is to ship the Pattern Lab Node CLI soon which will help new and existing users.

_In the meantime..._

if you already have an Edition tracking 3.X alphas, you can update using the [standard instructions](https://github.com/pattern-lab/patternlab-node/wiki/Upgrading#3x-instructions).

if you don't mind pulling down everything and playing with it locally, clone this repo and follow the instructions for [developing locally](https://github.com/pattern-lab/patternlab-node/blob/master/.github/CONTRIBUTING.md#developing-locally).

if you don't yet have a 3.X compatible Edition and want to try something a bit messier (and unsupported for now), you could attempt this [workaround](https://github.com/pattern-lab/patternlab-node/issues/813).

## Ecosystem

![Pattern Lab Ecosystem](http://patternlab.io/assets/pattern-lab-2-image_18-large-opt.png)

Core, and Editions, are part of the [Pattern Lab Ecosystem](http://patternlab.io/docs/advanced-ecosystem-overview.html). With this architecture, we encourage people to write and maintain their own Editions, Starterkits, and even PatternEngines.

## Support for Pattern Lab

Pattern Lab / Node wouldn't be what it is today without the support of the community. It will always be free and open source. Continued development is made possible in part from the support of [these wonderful project supporters](https://github.com/pattern-lab/patternlab-node/wiki/Thanks). If you want to learn more about supporting the project, visit the [Pattern Lab / Node Patreon page](https://www.patreon.com/patternlab).

**:100: Thanks for support from the following:**

* **[Brad Frost](http://bradfrost.com/)**
* [Marcos Peebles](https://twitter.com/marcospeebles)
* [Susan Simkins](https://twitter.com/susanmsimkins)
* [Wilfred Nas](https://twitter.com/wnas)

## Contributing

Refer to the [contribution guidelines](https://github.com/pattern-lab/patternlab-node/blob/master/.github/CONTRIBUTING.md).
>>>>>>> ab8fbc432b45baee56de5517ff3c93ffeae274a9
