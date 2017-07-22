{% method %}

## mangapress_comic_navigation($args, $echo)

Generates an unordered list of links for navigating between comic posts. Should be used inside a loop.

### Parameters

* `$args (array)` Navigation output arguments
* `$echo (boolean)` Specifies whether to echo comic navigation or return it as a string. Defaults to true.

#### Parameters for `$args`
* `$container`: Wrapper tag for comic navigation. Defaults to nav. Use false for no container.
* `$container_attr`: Attributes for container tag. Can be used for setting custom IDs or classes. Defaults to `array('id' => 'comic-navigation')`.
* `$items_wrap`: Navigation items wrapper. Defaults to `<ul%1$s>%2$s</ul>`. Can be useful for those situations when you don't want the navigation to be an unordered list.
* `$items_wrap_attr`: Same as $container_attr.
* `$link_wrap`: Wrapper tag for navigation link. Defaults to li.
* `$link_before`: Content before navigation link (but inside tag specified by `$link_wrap`).
* `$link_after`: Content after navigation link (but inside tag specified by `$link_wrap`).

{% sample lang="php" -%}
Short example of using `mangapress_comic_navigation()`:
```php
<div class="container">
    <?php if (have_posts()): ?> 

        <div class="hfeed">
        <?php while (have_posts()): the_post() : ?>

            <div <?php post_class(); ?>>
                <?php mangapress_comic_navigation($args); ?>

                <h2><?php the_title(); ?></h2>

                <div class="entry-content">
                    <?php the_post_thumbnail(); ?>
                </div>
            </div>            

        <?php endwhile; ?> 
        </div>

    <?php endif; ?>    
</div>
```
{% endmethod %}