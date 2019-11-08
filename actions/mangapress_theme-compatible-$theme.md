# mangapress_theme_compatible-$theme

## mangapress_theme_compatible-$theme

Allow third-party themes to declare Manga+Press compatibility options.

**@since** 4.0.0

## Usage

```php

function my_theme__add_manga_press_support() {
  /**
   * Add Manga+Press template hooks or load a file to handle support.
   */
}
add_action('mangapress_theme_compatible-my_theme', 'my_theme__add_manga_press_support');
```
