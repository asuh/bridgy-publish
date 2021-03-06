=== Bridgy Publish ===
Contributors: dshanske
Tags: indieweb, POSSE, bridgy
Stable tag: 1.3.3
Requires at least: 4.7
Tested up to: 4.9
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

[Bridgy](https://www.brid.gy) is a service that pull comments, likes, and reshares on social networks back to your web site. You can also use it to post to social networks - or comment, like, reshare, or even RSVP - from your own web site.

== Description == 

This plugin is a user interface for the Bridgy service and requires the [webmention](https://wordpress.org/plugins/webmention/) plugin to 
notify Bridgy to post. 

It also stores a link to the syndicated version for display by [Syndication Links](https://wordpress.org/plugins/syndication-links/) 
or other uses.

[Bridgy](https://www.brid.gy) posts to social networks by reading the HTML of your site. This means that the post is generates depends on your 
theme and any content generated by plugin. Bridgy offers a preview mode on their site to test your theme. 

Development/Issues/Feature Requests for the plugin only should be submitted through [Github](https://github.com/dshanske/bridgy-publish).

For development/issues/enhancements for the Brid.gy service, please submit on their [Github](https://github.com/snarfed/bridgy) page. Please read their About page for the features of the service prior to submission.


== Changelog == 

= Version 1.3.3 =
	* Fix Twitter excerpt issue due closing bracket missing
	* Fix Omit Link Issue
	* Move from embedding omit link and ignore formatting to using query parameters
	* Support alternate URL paths for WordPress when registering

= Version 1.3.2 =
	* Add testing environment
	* Fix PHPCS issues
	* Ensure PHP compatibility
	* Fix typo on class for bridgy excerpt (props @miklb )

= Version 1.3.1 =
	* Fix micropub syndicate standard compliance.

= Version 1.3.0 =
	* Rebrand as Bridgy
	* Allow simple registration on the settings page.
	* Disable shortlinks if the send shortlinks option is not enabled

= Version 1.2.2 =
	* Switch adding publish links to content to adding to footer
	* Remove async hook introduced in 1.2.0 due request
	* Errors returned by Bridgy display in the Post UI
	* Invert description for Backlink Option from Omit to Show due confusion
	* Add support for pages
	* Add `bridgy_publish_post_types` filter to show Bridgy post box on other post types

= Version 1.2.1 =
	* Omit Links option not set on Micropub so will now pull from the default setting if the post setting is not enabled

= Version 1.2.0 =
	* Add per post support for Bridgy backlink settings. Credit to @iamwebrocker for addition
	* Redo Settings Page and allow default to checked to be on a per-service basis.
	* Publish Now Works Off of a Cron Job Hook 5-10 seconds after the post is published
	* Support for Setting and Being Triggered by Micropub Syndication Requests
	* Storage of Syndication Preferences now stored in `mf2_` microformats 2 properties
	* Optionally set the Twitter post based on the post excerpt

= Version 1.1.1 =
	* Fix compatibility with changes in Syndication Links and change storage to array from EOL separated string

= Version 1.1.0 =
	* Remove Instagram setting as deprecated
	* Add Flickr setting as now supported
	* Change webmention support notice to activate on send_webmention per request
	* Comply with WordPress Standards

= Version 1.0.1 = 
	* Bug Fixes
	* If Indieweb Plugin is installed, move settings under that menu
	* If WP_DEBUG is set - send Publish entries to the error log

= Version 1.0.0 =
	* Initial release
	* Takes over Syndication Links storage of Bridgy Publish links

