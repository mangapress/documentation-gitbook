# Manga+Press Template API — Actions

This API provides a means of allowing support from 3rd party themes. [Also see Manga+Press Template API — Filters](/filters/template-api-filters.md)

## mangapress_after_body_open

Runs after wp_body_open. Allows for markup insertion following <body> and wp_body_open()

**@since** 4.0.0

## mangapress_page_header

Allows for site branding/main page header insertion

**@since** 4.0.0

## mangapress_after_page_header

Allows for content to be inserted directly after header

**@since** 4.0.0

## mangapress_get_comic_header

Output theme header specific to Manga+Press content types, or normal theme header.

**@since** 4.0.0

## mangapress_get_comic_footer

Output theme footer specific to Manga+Press, or normal theme footer.

**@since** 4.0.0

## mangapress_before_footer

Handle output before footer.

**@since** 4.0.0

## mangapress_before_content

Run scripts or insert content before the main content area.

**@since** 4.0.0

## mangapress_before_comic_loop

Run scripts or insert content before the main loop.

**@since** 4.0.0


## mangapress_before_article

Run scripts or insert content before the article tag but after the loop starts

**@since** 4.0.0


## mangapress_before_article_content

Run scripts or insert content before the article content but after the article opening tag.

**@since** 4.0.0

## mangapress_archive_style_template

Output the individual archive entry markup based on archive style.

**@since** 4.0.0

### Parameters

* $archive_style (string) The comic archive page style, can be `'list'`, `'gallery'`, or `'calendar'`


## mangapress_after_article_content

Run scripts or insert content after the article content but before the article closing tag.

**@since** 4.0.0

## mangapress_after_article

Run scripts or insert content after the closing article tag but before the main loop ends or iterates to the next post.

**@since** 4.0.0

## mangapress_after_latest_comic

Run scripts or insert content after latest comic loop conditional.

**@since** 4.0.0

## mangapress_output_no_comics_message

Outputs message if no comics are found for archive or other listings.

**@since** 4.0.0

## mangapress_archive_style_opening_tag

Output the opening wrapping tag based on the archive style.

**@since** 4.0.0

### Parameters

* $archive_style (string) $archive_style The comic archive page style, can be `'list'`, `'gallery'`, or `'calendar'`.
 

## mangapress_archive_style_closing_tag

Output the closing wrapping tag based on the archive style.

**@since** 4.0.0

### Parameters

* $archive_style (string) $archive_style The comic archive page style, can be `'list'`, `'gallery'`, or `'calendar'`.


## mangapress_after_archive_comic_loop

Run scripts or insert content directly after comic archive loop.
 
**@since** 4.0.0

## mangapress_after_content

Run scripts or insert content after the main content area.

**@since** 4.0.0

## mangapress_sidebar

Possibly insert a sidebar.

**@since** 4.0.0
