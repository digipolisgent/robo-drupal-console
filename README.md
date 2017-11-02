# Robo Drupal Console Extension

Extension to execute Drupal Console commands in [Robo](http://robo.li/).

[![Latest Stable Version](https://poser.pugx.org/digipolisgent/robo-drupal-console/v/stable)](https://packagist.org/packages/digipolisgent/robo-drupal-console)
[![Latest Unstable Version](https://poser.pugx.org/digipolisgent/robo-drupal-console/v/unstable)](https://packagist.org/packages/digipolisgent/robo-drupal-console)
[![Total Downloads](https://poser.pugx.org/digipolisgent/robo-drupal-console/downloads)](https://packagist.org/packages/digipolisgent/robo-drupal-console)
[![PHP 7 ready](http://php7ready.timesplinter.ch/digipolisgent/robo-drupal-console/develop/badge.svg)](https://travis-ci.org/digipolisgent/robo-drupal-console)
[![License](https://poser.pugx.org/digipolisgent/robo-drupal-console/license)](https://packagist.org/packages/digipolisgent/robo-drupal-console)

[![Build Status](https://travis-ci.org/digipolisgent/robo-drupal-console.svg?branch=develop)](https://travis-ci.org/digipolisgent/robo-drupal-console)
[![Code Climate](https://codeclimate.com/github/digipolisgent/robo-drupal-console/badges/gpa.svg)](https://codeclimate.com/github/digipolisgent/robo-drupal-console)
[![Test Coverage](https://codeclimate.com/github/digipolisgent/robo-drupal-console/badges/coverage.svg)](https://codeclimate.com/github/digipolisgent/robo-drupal-console/coverage)

Created based on [Robo DrushStack](https://github.com/boedah/robo-drush). Runs
Drupal Console commands in stack. You can define global options for all
commands (like Drupal root and uri).

## Table of contents

- [Installation](#installation)
- [Usage](#usage)
- [Testing](#testing)
- [Examples](#examples)

## Installation

Add `"digipolisgent/robo-drupal-console": "~0.1"` to your composer.json:

```json
    {
        "require-dev": {
            "digipolisgent/robo-drupal-console": "~0.1"
        }
    }
```

and execute `composer update`.

OR

Issue `composer require --dev digipolisgent/robo-drupal-console:~0.1`

## Usage

Use the trait (according to your used version) in your RoboFile:

```php
class RoboFile extends \Robo\Tasks
{
    use DigipolisGent\Robo\Task\DrupalConsole\loadTasks;
}
```

## Testing

`composer test`

## Examples

### Site update

This executes pending database updates and reverts all features (from code to database):

### Site install
