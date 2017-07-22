{% method %}

## mangapress_archive_gallery_style()

Filter for modifying default embedded CSS stylesheet for the Archive Gallery.

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


{% endmethod %}

