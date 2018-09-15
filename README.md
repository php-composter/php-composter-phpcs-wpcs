# PHP Composter PHPCS WPCS

### Check your PHP source code for compliance with WordPress Coding Standards before committing.

This Composer package will start to check your PHP files upon each commit to make sure they comply with the [WordPress Coding Standards](https://make.wordpress.org/core/handbook/best-practices/coding-standards/php/).

This is a [PHP Composter](https://github.com/php-composter/php-composter) Action.

Uses the wonderful [PHP CodeSniffer Project](https://github.com/squizlabs/PHP_CodeSniffer).

## Table Of Contents

* [Installation](#installation)
* [Basic Usage](#basic-usage)
* [Contributing](#contributing)

## Installation

Add the GitHub repository's URL as a package repository to the `composer.json` file:
```
"repositories": [
  {
    "type": "vcs",
    "url": "https://github.com/php-composter/php-composter-phpcs-wpcs"
  }
],
```

Then just add the package as a development requirement to your `composer.json`, and it should work automagically:

```BASH
composer require --dev php-composter/php-composter-phpcs-wpcs
```

## Basic Usage

It should just work when you `git commit`.

## Internals

WPCS provides 5 different coding standards (`WordPress-VIP`, `WordPress`,
`WordPress-Extra`, `WordPress-Docs` and `WordPress-Core`). By default this uses
`WordPress-Extra`. If you want to use another one of the standards, you can
specify it in your project's composer.json's `extra` key:
 ```json
  "extra": {
    "php-composter-phpcs-wpcs": {
      "standard": "WordPress-VIP"
    }
  }
```

## Contributing

All feedback / bug reports / pull requests are welcome.
