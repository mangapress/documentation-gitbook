{% method %}
### mangapress_start_latest_comic()
Starts a Latest Comic loop. See [mangapress_end_latest_comic()](//mangapress-end-latest-comic.md)

#### Parameters
None

#### Usage
```php
<?php mangapress_start_latest_comic(); ?>
```
{% sample lang="php" -%}
#### Example
```php
<?php    
    mangapress_start_latest_comic();

    if (have_posts()) :
        while (have_posts()) : the_post(); ?>

        <!-- loop markup -->

        <?php endwhile;
    endif;

    mangapress_end_latest_comic();
?>
```
{% endmethod %}

