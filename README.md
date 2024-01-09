# String Manipulation

This is a PHP library that provides various string manipulation utilities. It is designed to be easy to use and
efficient, making it ideal for any PHP project that requires string manipulation.

[![Packagist Version](https://img.shields.io/packagist/v/marjovanlier/stringmanipulation)](https://packagist.org/packages/marjovanlier/stringmanipulation)
[![Packagist Downloads](https://img.shields.io/packagist/dt/marjovanlier/stringmanipulation)](https://packagist.org/packages/marjovanlier/stringmanipulation)
[![Packagist License](https://img.shields.io/packagist/l/marjovanlier/stringmanipulation)](https://choosealicense.com/licenses/mit/)
[![PHP from Packagist](https://img.shields.io/packagist/php-v/marjovanlier/stringmanipulation)](https://packagist.org/packages/marjovanlier/stringmanipulation)
[![Latest Stable](https://poser.pugx.org/marjovanlier/stringmanipulation/v/stable)](https://packagist.org/packages/marjovanlier/stringmanipulation)
[![PHPStan Enabled](https://img.shields.io/badge/PHPStan-enabled-brightgreen.svg?style=flat)](https://phpstan.org/)
[![Phan Enabled](https://img.shields.io/badge/Phan-enabled-brightgreen.svg?style=flat)](https://github.com/phan/phan/)
[![Psalm Enabled](https://img.shields.io/badge/Psalm-enabled-brightgreen.svg?style=flat)](https://psalm.dev/)

## Features

- **Search Words**: Transforms a string into a format suitable for database searching.
- **Name Fix**: Fixes a given last name to conform to specific naming standards.
- **UTF-8 to ANSI**: Converts UTF-8 encoded characters to their ANSI counterparts.
- **Remove Accents**: Removes accents and special characters from a given string.
- **Date Validation**: Validates a date string against a specified format and checks for logical errors.
- **Time Part Validation**: Checks if the time part of a date is valid.

## Installation

You can install the package via composer:

```bash
composer require marjovanlier/stringmanipulation
```

## Usage

Here is a basic example of how to use the `searchWords` function:

```php
use MarjovanLier\StringManipulation\StringManipulation;

$result = StringManipulation::searchWords('Hello_World');
echo $result; // Outputs: 'hello world'
```

## Testing

Run the tests with:

```bash
vendor/bin/phpunit
```

## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.

## Detailed Examples

### Name Fix

```php
use MarjovanLier\StringManipulation\StringManipulation;

$fixedName = StringManipulation::nameFix('mcdonald');
echo $fixedName; // Outputs: 'McDonald'
```

### UTF-8 to ANSI Conversion

```php
use MarjovanLier\StringManipulation\StringManipulation;

$ansiString = StringManipulation::utf8Ansi('Äpfel');
echo $ansiString; // Outputs: 'Äpfel' in ANSI format
```

## Requirements

- PHP 8.2 or higher.

## Support

For support, issues, or questions, please open an issue on the GitHub repository.

