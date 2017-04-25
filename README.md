# wordpress-boilerplate
[![Build Status](https://travis-ci.org/solsoft/wordpress-boilerplate.svg?branch=4.x)](https://travis-ci.org/solsoft/wordpress-boilerplate)
[![Dependency Status](https://www.versioneye.com/user/projects/58feac52710da23f86d4ff05/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/58feac52710da23f86d4ff05)
[![Packagist](https://img.shields.io/packagist/vpre/solsoft/wordpress-boilerplate.svg)](https://packagist.org/packages/solsoft/wordpress-boilerplate)
[![PHP 7 ready](https://php7ready.timesplinter.ch/solsoft/wordpress-boilerplate/4.x/badge.svg)](https://travis-ci.org/solsoft/wordpress-boilerplate)
[![License](https://poser.pugx.org/solsoft/wordpress-boilerplate/license)](https://github.com/solsoft/wordpress-boilerplate/blob/4.x/LICENSE)

Boilerplate for deploying new [WordPress](https://wordpress.org/) projects.  Based on [johnpbloch/wordpress-project](https://github.com/johnpbloch/wordpress-project) and [composer.rarst.net](https://http://composer.rarst.net/).  
Using [Composer](https://getcomposer.org/) and associated plugins, and the unofficial [wpackagist.org](https://wpackagist.org) repository.  
Packages are published and updated regularly at [Packagist](https://packagist.org/packages/solsoft/wordpress-boilerplate).  

## WordPress versions supported
- WordPress 4.7.x

## Development branches
- 4.x - development branch for the latest WordPress 4.7.x

## Usage
Before starting, consult the Composer reference for standard usage instructions.  
Use `composer create-project` to deploy a new project, specifying one branch.

```
composer create-project solsoft/wordpress-boilerplate:4.x-dev my-project --stability dev --no-interaction;
cd my-project;
composer update;
composer show;
composer run;
```

## Contributing
Clone the git repository pointing to one of the development branches.  
Merge requests should be submitted against these branches.

```
git clone -b 4.x git@github.com:solsoft/wordpress-boilerplate.git;
cd wordpress-boilerplate;
composer install;
composer update;
composer show;
composer run;
```

### Extras
The project can be reset by running `composer cleanup-project` to delete
the `vendor/`, `assets/` and `app/` directories and the `composer.lock` file.  
Optionally you may run `composer examples-deploy` to install example WordPress
Contributed libraries, plugins and themes example dependencies. These can
also be undeployed by running `composer examples-undeploy`. See more
information about this in the `composer.examples` directory.  

## Credits
See the [composer README](composer/README.md) for information about composer packages.  
Inspiration taken from [johnpbloch/wordpress-project](https://github.com/johnpbloch/wordpress-project) and [composer.rarst.net](https://http://composer.rarst.net/).

WordPress Boilerplate  
Copyright (C) 2017 SOL-Soft  
Luís Pedro Algarvio  

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
