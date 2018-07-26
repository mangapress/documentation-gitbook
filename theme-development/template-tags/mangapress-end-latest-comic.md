# mangapress\_end\_latest\_comic

## mangapress\_end\_latest\_comic\(\)

Ends a Latest Comic loop. See [mangapress\_start\_latest\_comic\(\)](mangapress-start-latest-comic.md)

### Parameters

None

### Usage

```php
<?php mangapress_end_latest_comic(); ?>
```

### Example

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

