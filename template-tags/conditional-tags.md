# Conditional Tags

Manga+Press has a few conditional template tags that work similar to Template Tags in WordPress

## is\_comic\(\)

Returns `true` if post is a comic, otherwise returns `false`. Used to detect comic posts from regular posts.

Short example of using `is_comic()`:

```php
<?php
    if (is_comic()) {
        // do something for comic posts here
    } else {
        // ignore for all other posts
    }
?>
```

## is\_comic\_page\(\) * behavior changed in 4.0

Returns `true` if page is a Comic Page, otherwise returns `false`.

Short example of using `is_comic_page()`:

```php
<?php
    if (is_comic_page()) {
        // do something for Comic Page here
    } else {
        // ignore for all other posts
    }
?>
```

## is_latest_comic_page()

Returns `true` if the page is the Latest Comic page, otherwise `false`


Short example of using `is_latest_comic_page()`:

```php
<?php
if (is_latest_comic_page()) {
// do something for Latest Comic Page here
} else {
// ignore for all other posts
}
?>
```



## is\_comic\_archive\_page\(\)

Returns `true` if page is the Comic Archive Page, otherwise returns `false`.

Short example of using `is_comic_archive_page()`:

```php
<?php
if (is_comic_archive_page()) {
// do something for Comic Archive Page here
} else {
// ignore for all other posts
}
?>
```

