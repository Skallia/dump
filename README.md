# Dump - PHP Function

[![](https://img.shields.io/packagist/v/assouan/dump.svg)](https://packagist.org/packages/assouan/dump)
[![](https://img.shields.io/packagist/dt/assouan/dump.svg)](https://packagist.org/packages/assouan/dump)

Dumps information about a variable.

## Installation

Install using composer:

```bash
$ composer require monolog/monolog
```

## Usage

Simple dump:

```php
dump($var);
```

Multiple dump:

```php
dump($var1, $var2, $var3);
```

## Example

```php
$fake = [
    'var10' => null,
    'var11' => false,
    'var12' => true,
    'var13' => 123,
    'var14' => 9.99,
    'var15' => 'Hello world!',
    'var21' => [],
    'var22' => [123,456,789,'end',55.99],
    'var31' => fopen(__FILE__, 'r'),
    'var32' => ($tmp = fopen(__FILE__, 'r') AND fclose($tmp)) ? $tmp : $tmp,
    'var41' => new stdClass(),
    'var42' => new DateTime(),
];

dump($fake);
```

## Screenshot

![](https://i.imgsafe.org/1f254e6.png)
