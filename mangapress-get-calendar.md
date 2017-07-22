{% method %}
## mangapress_get_calendar()
Outputs a calendar displaying the current month's comic posts. Post-type-neutral version of `get_calendar()`. See [`get_calendar()`](https://codex.wordpress.org/Function_Reference/get_calendar) on WordPress.org for more information.

### Usage

```php
<?php mangapress_get_calendar(); ?>
```

### Parameters:

* $initial (boolean)(optional): If true, the day will be displayed using a one-letter initial; if false, an abbreviation based on your localization will be used.
* $echo (boolean)(optional): If true, will output the calendar. Defaults to true. False will return the markup as a string.

{% endmethod %}



