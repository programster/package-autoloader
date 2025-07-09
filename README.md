This is a package for PHP which simplifies the setup of autoloading. This requires your class names 
to exactly reflect your file names. E.g. the class called `MyClass` should be in a file called 
`MyClass.php`. You should use unique class names.

## Example Usage

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php'); # this autoloads all vendor packages

$autoloader = new Programster\Autoloader\Autoloader([
    __DIR__ . '/controllers',
    __DIR__ . '/libs',
    __DIR__ . '/views',
    __DIR__ . '/middleware',
    __DIR__ . '/models',
]);
```

That's it! Now all of your classes will automatically load. You don't need to use any `include` or 
`require` statements.
