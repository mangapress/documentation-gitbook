# FAQ \(Frequently Asked Questions\)

#### _I'm using the bundled theme for TwentyEleven, -Twelve, or -Thirteen but the Custom CSS and/or Insert Navigation options have no effect? Or they add a second navigation bar_

This is because the navigation for the comics is built into the theme. Using a different theme or overriding the default theme's template will allow you to use the options. \(however, see[issue \#17](https://github.com/jesgs/mangapress/issues/17)for additional issues\)

#### _Does Manga+Press work on WordPress Multi-site?_

Yes, it does. However, a few steps must be taken to make Manga+Press' child-themes available to your network. See the question below on the steps to take to enable the child-themes on Multisite.

#### _The bundled themes aren't available in WordPress Multi-site. What's going on?_

This is because the plugin hasn't been activated for the entire MS network. In order for the child-themes to be available, Manga+Press must be available to the entire network. This can be done by going to**Network Admin &gt; Plugins**and clicking the_Network Activate_link for Manga+Press. Once this is done, then both the parent- and child-themes need to made available to the network as well. This can be accomplished by going to**Network Admin &gt; Themes**, selecting the themes in question, choosing**Bulk Actions &gt; Network Enable**, and then clicking**Apply**.

#### _Is Manga+Press responsive?_

Not by itself. However, Manga+Press doesn't output markup other than the comic navigation. Responsiveness depends on the theme that is being used. The themes bundled with Manga+Press — the TwentyEleven thru TwentyFourteen child-themes — all have some level of responsiveness that is dependent on their parent themes.

#### _Is Manga+Press compatible with Advanced Custom Fields_

Yes, it is! Manga+Press is simply a stripped down custom post-type with a custom Featured Image meta-box. Like any other post-type, you can add a new field group using ACF — however, you_will_have to configure your theme to display these custom fields.

#### _Is Manga+Press compatible with the WPML plugin?_

I have never had the chance to test Manga+Press with the WPML plugin so I cannot guarantee compatibility.

#### _Do you take feature requests?_

I do take feature requests — however, there are a few criteria on which I judge each request:

1. Does the new feature fit with Manga+Press' current goals?
2. How well will the new feature fit with Manga+Press' current functionality?
3. The level of effort needed to integrate the new feature into the Manga+Press core.

#### _Do you provide support for 3rd party themes?_

The only themes that I provide support for are the themes that come with Manga+Press, which are child-themes of the default WordPress themes.

