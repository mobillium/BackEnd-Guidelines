# Project Folder Structure [WIP]

## Table of Content

* Overview
* Differences from Laravel's Standard Directory Structure
    * The `app\Http\Controllers\` directory
    * The `modules/` directory
* Example Project Tree

## Overview

Our project folder structure is very much to same as [Laravel's standard
directory structure](https://laravel.com/docs/8.x/structure). Additionally, we
have extra directory in the root directory. It is `modules/`, that contains all
modules as sub-directory used by main application (see [Modules](#modules)).

## Differences from Laravel's Standard Directory Structure

### The `app\Http\Controllers\` directory
We divide it into namepaces for various purposes. We have 3 namespace that are
absolutely necessary in every project. These are:

* `\App\Http\Controllers\Admin\`: Contains admin related controllers.
* `\App\Http\Controllers\Web\`: Contains public pages (homepage, privacy etc.)
  controllers.
* `\App\Http\Controllers\Api\`: Contains api related controllers.

### The `modules/` directory

WIP

## Example Project Tree
```txt
├── app
│   ├── Channels
│   ├── Console
│   │   └── Commands
│   ├── Events
│   ├── Exceptions
│   ├── Exports
│   ├── Helpers
│   ├── Http
│   │   ├── Controllers
│   │   │   ├── Admin
│   │   │   ├── Api
│   │   │   └── Web
│   │   ├── Middleware
│   │   ├── Requests
│   │   │   ├── Admin
│   │   │   ├── Api
│   │   │   └── Web
│   │   └── Resources
│   ├── Jobs
│   ├── Listeners
│   ├── Models
│   ├── Notifications
│   ├── Override
│   ├── Policies
│   ├── Providers
│   ├── Rules
│   ├── Services
│   └── Traits
├── bootstrap
├── config
├── coverage
├── database
│   ├── factories
│   ├── migrations
│   └── seeders
├── Modules
│   ├── Core
│   │   ├── resources
│   │   └── src
│   ├── Faq
│   │   ├── database
│   │   ├── resources
│   │   ├── routes
│   │   └── src
│   ├── Language
│   │   ├── database
│   │   ├── resources
│   │   ├── routes
│   │   └── src
│   ├── Translation
│   │   ├── database
│   │   ├── resources
│   │   ├── routes
│   │   └── src
│   └── Version
│       ├── database
│       ├── resources
│       ├── routes
│       └── src
├── public
├── resources
│   ├── lang
│   │   ├── en
│   │   └── tr
│   ├── sass
│   ├── stubs
│   └── views
├── routes
├── storage
└── tests
    ├── Feature
    └── Unit
```