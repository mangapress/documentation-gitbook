# mangapress_comic_navigation_args

## mangapress_comic_navigation_args

Filter available arguments for mangapress_comic_navigation. Returns array of arguments.

**@since** 2.7

### Parameters
 
* $parsed_args (array) Array of arguments, already parsed by wp_parse_args 
  
  * $container (string) Container wrapping tag, defaults to 'nav'.
 
  * $container_attr (array) Array of wrapper tag attributes. Data attributes can be added.

     * $id (string) Element's id attribute, defaults to comic-navigation

     * $class (string) Element's class attribute. Defaults to comic-nav-hlist-wrapper
 
* $items_wrap (string) Inner navigation wrapping markup, defaults to <ul%1$s>%2$s</ul>.

* $link_wrap (string) Link wrapper tag, defaults to li.
