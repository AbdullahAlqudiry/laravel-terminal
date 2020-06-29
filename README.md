# Laravel Terminal package
Run shell command easy in your laravel projects

This package is copy of [MrJoshLab/laravel-terminal](https://github.com/MrJoshLab/laravel-terminal) with some changes.

## Install

Via Composer

``` bash
$ composer require alqudiry/laravel-terminal
```

## Usage
You can run Terminal shell commands in laravel just like this:

```php
use Alqudiry\Terminal\Command;

$command  = new Command();
$response = $command->command('ls')->execute();
```

and you can get output of command just like this:
```php
return $response->getBody()->getContents();
```