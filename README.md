# date_get_week_number() for PHP

According to the [documentation](http://php.net/manual/en/function.date.php) for `date` function of the `W` format character
> ISO-8601 week number of year, weeks starting on Monday (added in PHP 4.1.0)

`date_get_week_number` amends this issue by returing a week number of a year where the week starts on Sunday

# Requirements
**PHP >= 5.2.0** because of the `DateTime` object usage

# Usage

```php
$date = new \DateTime;
$week = \date_get_week_number($date);
```

# Installation

Via composer: 
```javascript
{
    "require": {
        "dv-affection/date_get_week_number": "0.0.*"
    }
}
```

# Tests

```
cd date_get_week_number; phpunit;

...
OK (2 tests, 3 assertions)
```

