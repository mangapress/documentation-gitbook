{% method %}
### mangapress_day_link

Create a date-archive permalink for Comics. Used by `mangapress_get_calendar()`. Returns a date-based url.

#### Usage
```php
<?php
    $day_link = mangapress_day_link('', 2014, 9, 2);
?>
```

#### Parameters

* `$daylink (string)(not used)` Existing link to be modified or replaced. Not used.
* `$year (string|int)(optional)` Desired year for URL.
* `$month (string|int)(optional)` Desired month for URL.
* `$day (string|int)(optional)` Desired day for URL.
{% endmethod %}

