{% method %}
### mangapress_comic_front_slug

Allow plugins (or options) to modify Comic front slug (default: /comic/)

#### Parameters
* `$slug (string)` Default front slug

#### Usage

```php
<?php    
    /**
     * Change post-type's front slug
     */
    function my_new_slug($slug)
    {
        return 'new-slug';
    }
    add_filter('mangapress_comic_front_slug', 'my_new_slug');
?>
```

{% endmethod %}

