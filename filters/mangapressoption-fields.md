{% method %}
## mangapress_options_fields
Filter for modifying array of options fields. Must be run on `admin_init`.

### Parameters
* `$options (array)` Default array of plugin options.

### Usage
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
### Example
```php
array(
    'archive_order'    => array(
        'id'     => 'order',
        'title'  => __('Archive Page Comic Order', MP_DOMAIN),
        'description' => __('Designates the ascending or descending order of the orderby parameter', MP_DOMAIN),
        'type'   => 'select',
        'value'  => array(
            'ASC'  => __('ASC', MP_DOMAIN),
            'DESC' => __('DESC', MP_DOMAIN),
        ),
        'valid'   => 'array',
        'default' => 'DESC',
        'callback' => array($this, 'settings_field_cb'),
    )
)
```
{% endmethod %}

