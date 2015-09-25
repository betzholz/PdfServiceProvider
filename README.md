PdfServiceProvider
==================

A Pdf Service Provider for [Silex][2], based on [ZendPdf][1] library.

[![Build Status](https://secure.travis-ci.org/erivello/PdfServiceProvider.png?branch=master)](http://travis-ci.org/erivello/PdfServiceProvider)

Installation
------------

Installation is very easy, it makes use of [Composer][3].

### Install Composer

Run this in your command line:

``` bash
$ curl -s http://getcomposer.org/installer | php
```

Or [download composer.phar][4] into the project root.

### Add PdfServiceProvider to your composer.json

    "require": {
        "php": "> 5.3.3",
        "betzholz/pdf-service-provider": "dev-master"
    }

### Install Dependencies

Run the following command:

``` bash
$ php composer.phar install
```

Now PdfServiceProvider is installed into your vendor directory.

Registering
-----------

    $app->register(new Erivello\Silex\PdfServiceProvider());


Usage
--------

You can access the PdfServiceProvider by calling ``$app['pdf.generator']``.


Tests
-----

``` bash
$ php composer.phar install && phpunit
```

License
-------

The PdfServiceProvider is licensed under the MIT license.

[1]: http://framework.zend.com/manual/1.12/en/zend.pdf.html
[2]: http://silex.sensiolabs.org/
[3]: http://getcomposer.org/
[4]: http://getcomposer.org/composer.phar
