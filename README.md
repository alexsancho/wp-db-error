# WP Dropin: Better db-error.php

[![Build Status](https://travis-ci.org/alexsancho/wp-db-error.svg?branch=master)](https://travis-ci.org/alexsancho/wp-db-error)

This `db-error.php` dropin enhances default "Database connection error page".

* It gives better connection error debugging for administrator when using wp-cli.
* It shows nice error message for end users.
* It returns `503 Service not available` status code instead of `200 OK`
* It shows database connection debugging to frontend when `WP_DEBUG` is used.

## Installation
You can copy `db-error.php` to your `wp-content` folder. Just plug&play.

OR you can use composer so that you can automatically update it too. Put these in your composer.json:
```json
{
    "require": {
        "alexsancho/wp-db-error": "^0.1"
    },
    "extra": {
        "dropin-paths": {
            "htdocs/wp-content/": ["type:wordpress-dropin"]
        }
    }
}
```
