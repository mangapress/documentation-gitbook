# Manga+Press Template API — Filters

## mangapress_opening_article_tag

Filter and then output the opening article tag. Returns string

The $style parameter is only used for the `archive-comic.php` template. If $style is provided,
it will check against the three known archive page styles, and return an `li` tag for `list` and
`gallery`. Overrides will be provided in the near future.


**@since** 4.0.0

### Parameters

* $archive_style (string) Defines the tag used to wrap the post area. Defaults to `article`.

* $args array $args Array of arguments to pass
    
    * $style (string) $style The comic archive page style, can be `'list'`, `'gallery'`, or `'calendar'`

## mangapress_closing_article_tag

Filter and then output the closing article tag. Returns string.

The $style parameter is only used for the `archive-comic.php` template. If $style is provided,
it will check against the three known archive page styles, and return an `li` tag for `list` and
`gallery`. Overrides will be provided in the near future.

**@since** 4.0.0

### Parameters

* $archive_style (string) Defines the tag used to wrap the post area. Defaults to `article`.

* $args array $args Array of arguments to pass
    
    * $style (string) $style The comic archive page style, can be `'list'`, `'gallery'`, or `'calendar'`
