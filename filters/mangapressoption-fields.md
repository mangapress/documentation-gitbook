{% method %}
## mangapress_options_fields
Filter for modifying array of options fields. Must be run on `admin_init`.

### Parameters
* `$options (array)` Default array of plugin options.

### Usage
Example for removing/disabling options in Manga+Press
```php
/**
 * Run the action that disables the insert_nav option.
 */
function _disable_options_init() {
    add_action('mangapress_option_fields', '_disable_options');
}
add_action('admin_init', '_disable_options_init');

/**
 * Remove the insert_nav option from the options array.
 *
 * @param array $options
 * @return array
 */
function _disable_options($options)
{
    // we're specifically looking for navigation...
    if (isset($options['nav']['insert_nav'])) {        
        unset($options['nav']['insert_nav']);
    }
    
    return $options;    
}

```

{% sample lang="php" -%}
### Example
Use `mangapress_option_fields` to add custom options.

```php
<?php
/**
 * Initialize custom options.
 */
function my_options_init() {
    add_action('mangapress_option_fields', 'add_custom_option');
}
add_action('admin_init', 'my_options_init');

/**
 * Add new option to the options array.
 *
 * @param array $options
 * @return array
 */
function add_custom_option($options)
{
    // register section with mangapress_options_section
    $custom_option['my_custom_section'] = array(
        'my_custom_option' => array(
            'id' => 'custom-option',
            'title' => __('My Custom Option', MY_TEXT_DOMAIN),
            'description' => __('Description of text field', MY_TEXT_DOMAIN),
            'type' => 'text',
            'value' => 'your value',
            'callback' => array($this, 'settings_field_cb'), // default value
        )
    );

    return array_merge($options, $custom_option);
}
```
{% endmethod %}

