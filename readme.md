# CliIO
A PHP library to read and write from/to standard input/output

## Usage example

Run this script in terminal window:
```php
<?php
use iotch\CliIO;

$cliio = new CliIO\CliIO;

$typed = $cliio
    ->write('Please, type something:', 'red|none|underline')
    ->prompt(' ');

$cliio
    ->write('You\'ve typed: ')
    ->write($typed, 'white|green|bold')
    ->newLine();
```