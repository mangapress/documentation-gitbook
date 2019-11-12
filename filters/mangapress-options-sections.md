# mangapress_options_sections

## mangapress_options_sections

Allow 3rd party themes and plugins to add their own sections to Manga+Press options. Returns array.

**@since** 2.9

### Parameters

* $sections (array) Array of sections used for Manga+Press Options page.

### Usage

```php

function my_theme_mangapress_options($options) {
  
  if (!isset($options['my_section']) {
    $options['my_section'] = [
      'title' => 'My Theme Section Title',
      'description' => 'My Theme Section description.'
    ]
  }
  
  return $options;
}
add_filter('mangapress_options_sections', 'my_theme_mangapress_options');
```
