PhpStorm PrestaShop Autocomplete
================================

![phpstorm-prestashop-autocomplete-screenshot.png](http://cdn.sigerr.org/phpstorm-prestashop-autocomplete/phpstorm-prestashop-autocomplete-screenshot.png "Follow this tutorial and this is what you'll get")

## Why do I need this ?

If you use PhpStorm and PrestaShop you probably noticed that you can't get
your IDE to autocomplete everything. PrestaShop is designed to be overridden,
and every class from the core is suffixed with 'Core'.

For example, Address class is actually declared this way:

```php
class AddressCore extends ObjectModel
{
  // ...
}
```

## How to get autocomplete with PrestaShop

1. Download the file autocomplete.php (or clone this repo)
1. Add the file to your project as an "External Library"
 1. Double click "External Libraries"
 1. Click on '+'
 1. Select the folder containing autocomplete.php

 ![how-to-get-phpstorm-autocomplete-prestashop.png](http://cdn.sigerr.org/phpstorm-prestashop-autocomplete/how-to-get-phpstorm-autocomplete-prestashop.png "How to get autocomplete with PhpStorm and PrestaShop")

## How It Works

The file autocomplete.php will extend each Core class and use the correct name.

```php
class Address extends AddressCore {}
```

### Credits

This is based on an original idea from [dkarvounaris](https://github.com/dkarvounaris/PHPStorm-CC-PrestaShop)
