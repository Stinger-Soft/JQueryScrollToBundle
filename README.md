# JQueryScrollToBundle
jquery-scrollTo Bundle for Symfony

## Current Version

jquery-scrollTo v2.1.2 - https://github.com/flesler/jquery.scrollTo

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/jquery-scrollto-bundle": "~2.1.2"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Stinger\JQueryScrollToBundle\StingerJQueryScrollToBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/jquery-scrollto-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

### Usage

Add the css and js file where needed:

``` html
{% javascripts
	'bundles/stingerjqueryscrollto/js/jquery.scrollTo.min.js'
%}
	<script src="{{ asset_url }}" ></script>
{% endjavascripts %}
```


# Licenses

Refer to the source code of the included files for license information

# References

1. https://github.com/flesler/jquery.scrollTo
2. http://symfony.com

