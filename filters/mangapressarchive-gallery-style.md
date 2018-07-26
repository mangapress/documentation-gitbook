# mangapress\_archive\_gallery\_style

## mangapress\_archive\_gallery\_style

Filter for modifying default embedded CSS stylesheet for the Archive Gallery.

### Parameters

* `$styles (array)(optional)` Embedded CSS stylesheet string used to override defaults.

### Usage

```php
<?php
/**
 * Disable the default Manga+Press gallery styles
 */
function myplugin_disable_gallery_styles($styles)
{
    return '';
}
add_filter('mangapress_archive_gallery_style', 'myplugin_disable_gallery_styles');
?>
```

Default CSS styles \(use in your own stylesheet\):

```css
.mangapress-archive-gallery {
     font-size: 0;
}

.mangapress-archive-gallery > li {
    text-align: center;
    width: 125px;
    min-height: 200px;
    font-size: 12px;
    list-style: none;
    margin: 10px;
    float: left;
}

.mangapress-archive-gallery > li:after {
     visibility: hidden;
     display: block;
     font-size: 0;
     content: " ";
     clear: both;
     height: 0;
}

.comic-title-caption,
.comic-post-date {
    text-align: center;
    margin: 0;
    padding: 0;
}

.comic-title-caption {
    text-overflow: ellipsis;
    overflow: hidden;
    white-space: nowrap;
}
```

