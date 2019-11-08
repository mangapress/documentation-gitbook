# mangapress\_end\_latest\_comic

## mangapress\_end\_latest\_comic\(\)

Ends a Latest Comic loop. See [mangapress\_start\_latest\_comic\(\)](https://github.com/mangapress/documentation/tree/8f66c9321acc635a7720230fcb4f40706a404910/mangapress-start-latest-comic.md)

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

