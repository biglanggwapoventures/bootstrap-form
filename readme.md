# CORE-SYSTEM BOOTSTRAP FORM (Upgraded)

[![Packagist](https://img.shields.io/packagist/l/core-system/bootstrap-form.svg?maxAge=2592000)](https://packagist.org/packages/core-system/bootstrap-form)
[![GitHub release](https://img.shields.io/github/release/core-system/bootstrap-form.svg?maxAge=2592000)](https://packagist.org/packages/core-system/bootstrap-form)

This is a standalone part of `core-system` application for Laravel 5 Framework. 

> [CORE-SYSTEM](http://www.core-system.cz) is Laravel 5 based application 

CORE-SYSTEM Bootstrap Form contains `laravel-collective/html` extension for simple Twitter Bootstrap 3 form generation and and request validation error handling.
 
## Summary

- [Requirements and dependencies](#requirements-and-dependencies)
- [Installation](#installation)
- [Usage](#usage)
 
## Licence

GPL-3.0+

## Requirements and dependencies

This package uses `composer` to installing dependencies

### Composer

- "php": ">=5.5.9",
- "laravel/framework": "~5.5.0|~5.6.0",
- "laravelcollective/html": "^5.5.0"

## Installation

Run command line and go to your project folder and paste this command

```
    $ composer require natabio/bs4-form
```

## Form methods

> create `<form>` field

```php
{!! Form::open(['url' => mixed $route = null, string 'method' => 'POST|PATCH|DELETE|GET', (optional) bool 'files' => true]) !!}
```

> create `<form>` field with model

```php
{!! Form::model(mixed $model = null, ['url' => mixed $route = null, string 'method' => 'POST|PATCH|DELETE|GET', (optional) bool 'files' => true]) !!}
```

> create `</form>` tag

```php
{!! Form::close()) !!}
```

> create `<input>` field

```php
{!! Form::inputGroup(string $type = 'text', string $lable = null, string $name = null, mixed $value = null, array $options = []) !!}
```

> create `<select>` field

```php
{!! Form::selectGroup(string $lable = null, string $name = null, array $options = [], mixed $selected = null, array $options = []) !!}
```

> create `<input type="checkbox">` field

```php
{!! Form::inlineCheckbox(string $name, mixed $value = 1, mixed $label = null, bool $checked = null, array $options = []) !!}
```

> create `<input type="radio">` field

```php
Form::inlineRadio(string $name, mixed $value = 1, mixed $label = null, bool $checked = null, array $options = [])
``` 