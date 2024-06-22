# User Agent

A wrapper for the [foroco/php-browser-detection](https://github.com/foroco/php-browser-detection) library.

This package offers a simple class parsing the user agent string.

> [!IMPORTANT]
> This package is still in development.
>
> While it is considered MVP and stable, it may still undergo breaking changes.

## Installation

```bash
composer require northrook/user-agent
```

## Usage
The `UserAgent` class static, and cannot be instantiated.

Access pre-parsed data using these static methods:

```php
use Northrook\UserAgent;

// Retrieve the foroco\BrowserDetection object
$userAgent = UserAgent::detect() : BrowserDetection

// Pass a string to $match the current OS family.
// If no $match is passed, a string with the matched OS family is returned
$os = UserAgent::OS(); 

UserAgent::getAll();
UserAgent::getOS();
UserAgent::getBrowser();
```

## License
[MIT](https://github.com/northrook/user-agent/blob/main/LICENSE)