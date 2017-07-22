{% method %}
## mangapress_month_link

Create a date-archive permalink for Comics (for monthly links). Used by mangapress_get_calendar(). Returns a date-based url.

### Usage
```php
<?php
    $month_link = mangapress_month_link('', 2014, 9);
?>
```

### Parameters
* `$monthlink (string)(not used)` Existing link to be modified or replaced. Not used.
* `$year (string|int)(optional)` Desired year for URL.
* `$month (string|int)(optional)` Desired month for URL.

{% endmethod %}

