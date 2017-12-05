# PHP Composter PHPCS WPCS

### Check your PHP source code for compliance with WordPress coding standards before committing.

This Composer package will start to check your PHP files upon each commit to make sure they comply to the [WordPress Coding Standards](https://make.wordpress.org/core/handbook/best-practices/coding-standards/php/).

This is a [PHP Composter](https://github.com/php-composter/php-composter) Action.

Uses the wonderful [PHP CodeSniffer Project](https://github.com/squizlabs/PHP_CodeSniffer).

## Table Of Contents

* [Installation](#installation)
* [Basic Usage](#basic-usage)
* [Contributing](#contributing)

## Installation

Add the repository's URL as a repository to the `composer.json` file:
```
"repositories": [
  {
    "type": "vcs",
    "url": "https://github.com/php-composter/php-composter-phpcs-wpcs"
  }
],
```

Then j add as a development requirement to your `composer.json`, and it should work automagically:

```BASH
composer require --dev php-composter/php-composter-phpcs-wpcs
```

## Basic Usage

It should just work when you `git commit`.

## Internals

By default of the 5 different WordPress coding standards (`WordPress-VIP`, `WordPress`, `WordPress-Extra`, `WordPress-Docs` and `WordPress-Core`), this one uses the WordPress-Extra.

If you need to change it, currently you need to edit the Sniff file. Contributions on how to make this dynamic are welcome (.env file, different sniffs for each and choosing the appropriate hooks).

## Contributing

All feedback / bug reports / pull requests are welcome.
