# Configuring Manga+Press

Instructions on configuring Manga+Press are intended for working with the provided child-themes for TwentyEleven, -Twelve, -Thirteen, -Fourteen, and -Fifteen. Other third-party themes may require additional adjustment.

## How To Configure Manga+Press

Manga+Press can work out of the box using the available child-themes for TwentyEleven through TwentyFifteen if there is no need for a Comic Archive page or a Latest Comic page.

### Set up Latest Comic and Comic Archive pages

Start by creating two new pages in the WordPress Admin, then navigate to **Settings &gt; Manga+Press Options**. On the first tab, labeled "Basic Options," select the pages you created in both the Latest Comic- and Comic Archive drop-downs. Manga+Press includes templates for both these pages, which are loaded by default. For further fine-tuning, add a custom template to your theme — ideally by creating child-theme of your selected theme. For more information on creating child-themes, see the WordPress Codex article on [child-themes](http://codex.wordpress.org/Child_Themes).

Note: do not use the Latest Comic or Comic Archive pages as your Home and Posts page (WordPress Admin > Reading Settings) as this will override the queries on those pages and prevent your comics from displaying.

### Configure Category Grouping

On the "Basic" options tab of the Manga+Press Settings page, the first two options are "Group Comics" and "Use Parent Category." These two options control how navigation between comics is handled. By default, comics navigate between each other regardless of their assigned category.

#### Group Comics

When "Group Comics" is enabled, then comics are grouped according to their mutually assigned categories. For example, if Comic A and Comic B are a part of **Series \#1**, but Comic C and -D are a part of **Series \#2**, then navigation will exist between Comic A and -B, and Comic C and D — but not between Comics A, B, C, and D.

#### Use Parent Category

This option only works when the "Group Comics" option is selected. It works similar to "Group Comics" but the comics are grouped according to their top-most parent category. In this example, Comics A, B, C, and D are assigned to **Issue \#2.1**, which has a parent called **Series \#2**, while the next group: Comics E, F, G, and I are assigned to **Issue \#3.1**, which has a parent called **Series \#3**. Navigation will exist between the comics assigned to **Series \#2**, and to the comics assigned to **Series \#3** but navigation will not exist between Comic D \(Series \#2\) and Comic E \(Series \#3\).

#### Archive Page Style \(Manga+Press 3.0\)

Manga+Press 3.0 adds a new option for changing the appearance of the Archive Page. You now have three options: List \(default\), Calendar, and Gallery. Calendar displays a standard monthly calendar similar to the post calendar provided by WordPress. Gallery will show all comics in a grid layout using that post's thumbnail.

#### Archive Page Sorting Order Options \(Manga+Press 3.0\)

Manga+Press 3.0 adds new options for changing the sorting order on the Archive Page. These options are the same basic parameters used by `order` and `orderby` in the [`WP_Query` object](https://codex.wordpress.org/Class_Reference/WP_Query#Order_.26_Orderby_Parameters). The drop-downs don't include the advanced sorting options available for WP\_Query \(for example: sorting by meta-data, comment-count, etc\).

### Custom Comic Page image sizes

This setting is intended to control the size of the image displayed. Manga+Press uses the WordPress thumbnail system to create image sizes based on values entered by the user. This is the image-size used on the Latest Comic page. This image can also be loaded in your template using`<?php the_post_thumbnail('comic-page'); ?>`

### Navigation

#### Navigation CSS

The Navigation CSS option allows you to use your own styling with the provided selectors \(Custom CSS\), or use Manga+Press' default styles \(Default CSS\).

#### For 3.0.x

Starting with 3.0, the "Insert Navigation" option has been removed. The content templates that come with Manga+Press already contain the navigation. These template will work with most themes, which removes the need for having an "Insert Navigation" option.

