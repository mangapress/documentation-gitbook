# Using Manga+Press

Before reading this guide, make sure to read [Configuring Manga+Press](/getting-started/configuring-manga+press.md) and [Theme Customization](/getting-started/theme-customization.md) first.

## Introduction

Manga+Press uses both WordPress custom post-types and the Media Library to help you manage your comic series. On activation, Manga+Press creates a new CPT called "Comic" that is used to store your comic pages. Each "Comic" post is intended to be a comic page. Navigation is handled automatically, using the same backend functionality that handles navigation between blog posts.

## How To

Let's get started. First, we'll add a comic:

### Posting and Managing Comics

#### Adding a New Comic

Start by navigate to the WordPress admin and clicking on **Comics **\(below **Posts **in the menu\).

Next, click on **Add New Comic**. This will take you to the **Add New Comic** screen, which looks like the Add New Post screen \(minus Post-specific content areas\).

Start by entering a title for your comic, then to add the image click on the **Set Comic Image **link in the **Comic Image **meta-box. The link will open the Media Library popup — similar to adding a Featured Image to a post. From the Media Library popup, either upload your comic image or select it from the Media Library.

\*If you're intending to organize your comic by categories \(ie: Series taxonomy\), then either select or add a new category using the Series meta-box in the right sidebar.

Click the **Publish** button_, _or click the **Edit** link next to **Publish Immediately **to schedule the comic post to be published at a later date. More info on scheduling posts: [WordPress.com: Schedule A Post.](http://en.support.wordpress.com/posts/schedule-a-post/)

Repeat the above process until you have a group of comics.

\*Depending which options are chosen in Manga+Press settings, this will have an impact on comic navigation. See [Configuring Manga+Press: Configure Category Grouping](https://mangapress.github.io/documentation/Configuring-Manga-Press#configure-category-grouping) for more information.

#### Editing and Removing Comics

Editing and removing comics works the same as default WordPress posts and pages. Clicking on the title of an existing comic in the **Comic **screen or the **Edit **link when hovering over the same title take you to the **Edit Comic** screen.

Clicking on the **Trash **link \(which appears when you hover over the title\) will put the comic in the Trash bin, from where you can either restore it or delete it permanently.

### Organizing Your Comics with the Series Taxonomy

Comics can be ordered by category, just like regular WordPress posts. However, for Comics we have a custom taxonomy labeled "Series," which works like the default WordPress category taxonomy. Using this taxonomy, you can group your comics according to chapters, issues, or even serials. Using the Series taxonomy can also control how you navigate between each comic. The [Configure Category Grouping](https://mangapress.github.io/documentation/Configuring-Manga-Press#configure-category-grouping) section of the Configuring Manga+Press guide offers more information on comic organization and how navigation behaves between categories.

