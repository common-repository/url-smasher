=== URL Smasher ===
Contributors: Rick Hellewell
Donate link: http://cellarweb.com/wordpress-plugins/
Tags: url shortener automatic goo.gl
Requires at least: 4.0.1
Tested up to: 6.5
Version: 3.10
PUP Version: 7.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Automatically shortens URLs in posts, pages, and comments using goo.gl. 

== Description ==

Automatically - and without any effort on your part - shortens URLs in posts, pages, and comments using goo.gl. Does not require any special shortcodes, buttons, or anything - just enable it, and URLs are smashed when the post/page/comment is saved. Just use your Google API Key (it's free) and off you go!



== Installation ==

This section describes how to install the plugin and get it working.

1. Download the zip file, uncompress, then upload to `/wp-content/plugins/` directory. Or download, then upload/install via the Add Plugin page.
1. Activate the plugin through the 'Plugins' menu in WordPress.
1. Change settings in Settings, 'URL Smasher Settings' to your requirements.

* Note: do a "Save" on the URL Smasher settings page once after an upgrade to ensure all is well; your settings will be preserved.

== Frequently Asked Questions ==

= Do I have to do anything special to enable this? =

You need to have your own Google API key (they are free, unless you have an extremely active site), and set up the two options on the Settings page.

Get API key from : http://code.google.com/apis/console/

= What settings are available? =

Just three: your Google API Key, and checkboxes to enable URL Smashing for posts/pages or comments.

= What if the URLs aren't smashed? =

That is usually caused by an invalid Google API Key. Or, you have done too many URL Smashes in one day. Check your Google API account for details. Sometimes it's because you didn't specify the full URL, including the "http(s)://" part - 'relative' URLs are not smashed.

If the URL Smash fails for some reasosn, the URL is not changed.

= What if I don't like how the plugin changes things or there is a problem? = 

You can just deactivate the plugin. Your settings will be saved if you want to reactivate later.

= Does the plugin make changes to the database? = 

The plugin only adds one 'row' to the Options database, using standard WordPress functions. The plugin will read the values as needed, minimizing calls to the database to limit any overhead against the database.

= Does the plugin require anything extra on the client (visitor) browser? = 

Not that we are aware of. The things we do are done through standard WordPress calls. It works with the standard 'jQuery' code that WordPress already includes and uses.

= Where can we go for support if there is a problem or question - or a new feature we think will be nifty? = 

You can use the plugin support page for questions. Or you can contact us directly via the Contact Us page at www.CellarWeb.com . We usually respond within 24 hours (and are usually faster than that).

= How much does the plugin cost? = 

It's free! But there is a place to donate at www.CellarWeb.com, if you are so inclined. (And we will appreciate that inclination!)

= What else do you do? = 

We have a plugin that stops comment spam in it's tracks. Plus a contact template that does the same thing. Our process doesn't rely on things that don't work, like hidden fields, or hard to use Captcha things. You'll find all the details at our FormSpammerTrap site: http://www.FormSpammerTrap.com .

We do lots of WordPress sites: implementation, customization, and more. You can find more info at our business site at www.CellarWeb.com .


== Screenshots ==

1. Shows information about the plugin on the Settings screen. (assets/screenshot-1.jpg)
2. Shows the Settings area. You enter the Bitly Generic Access Token, and enable 'URL Smashing' for post/pages and/or comments content.  (assets/screenshot-2.jpg)

== Changelog ==

= 3.10 (10 Jun 2022) =
* fix for warning message caused if a settings variable not set yet.

= 3.00 (26 May 2022) =
* updated for bit.ly API version 4. This requires you to get a new bit.ly Generic Access Code; instructions on the Settings page.
* updated for up to PHP version 8.
* updated/tested for latest WP versions.
* changed functions and variables names for consistancy .
* added sidebar for our other plugins.
* changed logo/header/etc for current branding.
* visual and text changes to settings screen and screenshot .
* updated screenshots and other images in assets folder.
* code efficiencies.

= 2.01 (27 Jan 2017) = 
* added button to test for a valid Bit.ly API Key (hopefully, it is your key).
* verified for WordPress 4.7.2
* moved version number to header on the Settings page.
* removed version number from being stored in the options table.
* fix to the date of version 1.06 in the readme (year was wrong).
* minor changes to the information/text on the Settings screen.

= 1.06  (27 Dec 2016) = 
* fix to set options on the first install, rather than uncermoniously just dying.
* minor code change to how the version number is changed
* changed the header image/info the settings page

= 1.05 (2-Aug-2016) =
* code changes to ensure 'safe' URLs (reduce XSS vulnerability)
* other minor code efficiencies
* minor changes to readme file and the Settings page area

= 1.04 = 
* Don't you hate it when a bug creeps in after you do all the testing and then release a revision and then things don't work right. Yeah, me too. (sigh)
* Fixed a bug where not all post content would be affiliated. And then tested everything again.

= 1.03 = 
* released 15 Dec 2015 
* tested for WordPress version 4.4
* some code efficiencies, adjusted variables for unique names
* minor visual changes to the settings screen
* minor adjustments to text of settings screen
* tested to ensure proper behavoir with other plugins (like our - shameless plug - "AmazoLinkenator" - which automatically adds your Amazon Affiliate code to Amazon URLs)

= 1.02 =
* released 31 Aug 2015
* adjusted URL Smasher's process priority to allow other URL-adjusting plugins to do their work first. For instance, if another plugin is adding an affiliate code to links on content save (shameless plug: like the "AmazoLinkenator" plugin we have), then that process should be allowed to finish before URL Smasher does its thing. Otherwise, URL Smasher's work may cause the other plugin not to 'see' the URL. URL Smasher now has a lower priority of '99', rather than the normal '10'. 
* removed version-checking code; it needs to be more efficiently done in a later version.

= 1.01b =
* released 24 Aug 2015
* code efficiencies
* corrected "Invalid Header" activation error 

= 1.01a =
* released 22 Aug 2015
* fixed formatting errors in the readme.txt file.
* updated the screenshot .
* changed the icon/graphic on the settings page

= 1.01 =
* Tested and Certified for WordPress 4.3 (21 Aug 2015)
* Changed top graphic for Settings page
* Added icon for WordPress plugin page

= 1.00 =
* Initial release (10 Aug 2015)


== Upgrade Notice ==

= 2.01 (27 Jan 2017) = 
* added button to test for a valid Bit.ly API Key (hopefully, it is your key).
* verified for WordPress 4.7.2
* moved version number to header on the Settings page.
* removed version number from being stored in the options table.
* fix to the date of version 1.06 in the readme (year was wrong).
* minor changes to the information/text on the Settings screen.

= 1.06  (27 Dec 2016) = 
* fix to set options on the first install, rather than uncermoniously just dying.
* minor code change to how the version number is changed
* changed the header image/info the settings page

= 1.05 = (2-Aug-2016)
* code changes to ensure 'safe' URLs (reduce XSS vulnerability)
* other minor code efficiencies
* minor changes to readme file and the Settings page area

= 1.04 = 
* Don't you hate it when a bug creeps in after you do all the testing and then release a revision and then things don't work right. Yeah, me too. (sigh)
* Fixed a bug where not all post content would be affiliated. And then tested everything again.

= 1.03 = 
* released 15 Dec 2015 
* tested for WordPress version 4.4
* some code efficiencies, adjusted variables for unique names
* minor visual changes to the settings screen
* minor adjustments to text of settings screen
* tested to ensure proper behavoir with other plugins (like our - shameless plug - "AmazoLinkenator" - which automatically adds your Amazon Affiliate code to Amazon URLs)

= 1.02 =
* released 31 Aug 2015
* adjusted URL Smasher's process priority to allow other URL-adjusting plugins to do their work first. For instance, if another plugin is adding an affiliate code to links on content save, then that process should be allowed to finish before URL Smasher does its thing. Otherwise, URL Smasher's work may cause the other plugin not to 'see' the URL. URL Smasher now has a lower priority of '99', rather than the normal '10'. 
* removed version-checking code; it needs to be more efficiently done in a later version.

= 1.01b =
* released 24 Aug 2015
* code efficiencies
* corrected "Invalid Header" activation error 

= 1.01a =
* released 22 Aug 2015
* fixed formatting errors in the readme.txt file.
* updated the screenshot .
* changed the icon/graphic on the settings page

= 1.01 =
* Tested and Certified for WordPress 4.3 (21 Aug 2015)
* Changed top graphic for Settings page
* Added icon for WordPress plugin page

= 1.00 =
* Initial release (10 Aug 2015)


