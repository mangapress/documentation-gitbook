# mangapress_the_comic_cover

## mangapress_the_comic_cover\(\)

Output the comic's cover image.

### Usage

```php
<?php mangapress_the_comic_cover(null, 'comic', ['class' => 'comic-image']); ?>
```

### Parameters:

* `$post (\WP_Post)(optional)`: Current post object. If null, global `$post` will be used instead
* `$size (string)(optional)`: Image size to load. Defaults to `thumbnail`.
* `$attr (array)(optional)`: Query string or array of attributrues

