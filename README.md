Context.IO Laravel 4 Package
===========

Laravel 4 package built on top of the official PHP Library for Context.IO

Original Library: https://github.com/dominikgehl

Installation
------------

Include the package in your composer file

    "require": {
        "teddy/contextio-laravel": "dev-master"
    }
    

Run composer update

Set up your Context.IO key and secret in 'config/packages/contextio/config.php'

Add the service provider in you app.php config file in the 'providers' array

    'Teddy\Contextio\ContextioServiceProvider'

and add the alies also in the app.php config file in the 'aliases' array

    'ContextIO'			  => 'Teddy\Contextio\ContextIO'


Usage
-----

$ContextIO = new ContextIO();

$ContextIO->listAccounts();

