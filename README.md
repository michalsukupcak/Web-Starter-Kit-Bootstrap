## PLEASE NOTE
> AS OF 29.7.2017 THIS REPOSITORY IS NO LONGER MAINTAINED

![Web Starter Kit + Bootstrap](http://s30.postimg.org/7u2nj3c81/web_starter_kit_bootstrap.png)

## Overview

Web Starter Kit with Bootstrap is a modified version of Google's [Web Starter Kit](https://developers.google.com/web/starter-kit) that has the default Style Guide replaced with [Bootstrap](https://github.com/twbs/bootstrap). Aim of the project is to allow developers access to all the powerful building tools WSK has on offer while letting them work with their favorite front-end framework, Bootstrap.

- Web Starter Kit: 0.6.1
- jQuery: 2.2.1
- Bootstrap: 3.3.6
- Font-Awesome: 4.5.0

## Quickstart

Check out README.MD for WSK for detailed explanation of what is going on here. You can (and should) use following commands:
- ```npm install``` - run as first thing after cloning repo as it downloads and installs all necessary dependencies such as build tools (gulp, lib-sass)
- ```gulp serve``` - run a local web server (localhost:3000) with a live and automatically updated preview of your application
- ```gulp``` - create production-ready build (dist)

## Update jQuery/Bootstrap/Font-Awesome ##

Simply download new version of jQuery, Bootstrap and Font-Awesome using ```bower install```. This creates ```/bower_components``` folder with latest versions of all 3 libraries/frameworks. Then simply replace following files:

| Original file                             | New file                                                                                       | Comment                                       |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------- | --------------------------------------------- |
| ```/app/fonts/**```                       | ```/bower_components/bootstrap/dist/fonts/**```, ```/bower_components/font-awesome/fonts/**``` | Delete all font files and copy new font files |
| ```/app/scripts/bootstrap.min.js```       | ```/bower_components/bootstrap/dist/js/bootstrap.min.js```                                     | Replace original file with new file            |
| ```/app/scripts/jquery.min.js```          | ```/bower_components/jquery/dist/jquery.min.js```                                              | Replace original file with new file            |
| ```/app/styles/bootstrap.min.css```       | ```/bower_components/bootstrap/dist/css/bootstrap.min.css```                                   | Replace original file with new file            |
| ```/app/styles/bootstrap-theme.min.css``` | ```/bower_components/bootstrap/dist/css/bootstrap-theme.min.css```                             | Replace original file with new file            |
| ```/app/styles/font-awesome.min.css```    | ````/bower_components/font-awesome/css/font-awesome.min.css```                                 | Replace original file with new file            |

Then simply remove ```/bower_components``` folder as it is no longer required.
