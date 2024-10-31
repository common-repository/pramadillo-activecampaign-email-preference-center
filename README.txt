=== ActiveCampaign Email Preference Center ===
Contributors: mattpramschufer, freemius, emoxie
Donate link: pramschufer.com
Tags: activecampaign, active campaign, email preference center, active campaign lists, activecampaign lists
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=mattpram%40gmail%2ecom
Tested up to: 6.2
Requires at least: 3.8
Stable tag: 2.0.12
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Allow users to manage their subscriptions to your ActiveCampaign lists through an integrated email preference center for WordPress.

== Description ==

ActiveCampaign does not have a native email preference center to allow your customers to manage their subscriptions to various lists.
I developed this plugin to make it quick and easy to integrate an ActiveCampaign email preference center into WordPress.

= The FREE version of this plugin gives you the following features: =

*   Easy Access to all of your ActiveCampaign lists
*   Ability for users to look up their subscriptions
*   Ability for users to subscribe and un-subscribe from all of your ActiveCampaign lists
*   Easy integration via Wordpress shortcode

= Usage =
Integration is easy, just use the shortcode
`[ac-preference-center]`
on any page, post or widget area to integrate your email preference center.

= The PREMIUM version of this plugin includes the following additional features: =

*   Select which ActiveCampaign lists to show in email preference center
*   The ability to change the name of your ActiveCampaign list for presentational purposes. *(i.e.  If your list is called Our Customers in ActiveCampaign, you could change that to Mailing List for the frontend*
*   Assign a description for each of your ActiveCampaign lists to describe your difference email lists
*   Control various template elements through use of simple shortcode flags.
*   Able to have logged in users automatically pull their subscribed lists.
*   Ability to implement tamper protection to send an email to user to confirm their email address before updating email preferences.


== Installation ==

After you install the plugin, make sure to go to the Settings->ActiveCampaign Preference Center page and input your ActiveCampaign Url and API Key.
You can find your API url and key by going to (https://help.activecampaign.com/hc/en-us/articles/207317590-Getting-started-with-the-API)

== Frequently Asked Questions ==

**Question:** I have several lists in ActiveCampaign but only want to show a couple of them, can I hide various lists?
**Answer:** Yes, but only with the Premium version of this plugin.  With the Premium version you can toggle on and off
each of the lists you want to show in the email preference center.

**Question:** Can I style the email preference center to match my theme?
**Answer:** Yes, I specially did not include any styles with this plugin to make it utilize your themes built in styles.
If you navigate to the settings page, at the bottom I have included some basic styles which you could add to your
additional CSS section of Appearance->Customize

**Question:** I really wish this plugin did X, do you offer customizations?
**Answer:** Yes, please reach out and let me know what feature you wish this plugin had.  I might add it to the road map
if I think it would benefit everyone, or we could discuss the possibility of custom development for your specific case.  Please add a feature request at https://pramadillo.com

== Screenshots ==

1. Settings Screen
4. Preference Center Email Lookup
5. Preference Center Lists

== Changelog ==
= 2.0.12 =
* UPDATE - Updated third-party dependencies to latest versions (Freemius 2.5.7 to 2.5.10)

= 2.0.11 =
* BUGFIX - Fixed bug which would not subscribe user to list when first creating contact in AC.
* UPDATE - Update all vendor libraries to latest versions.

= 2.0.10 =
* UPDATE - Updated all vendor libraries

= 2.0.9 =
* UPDATE: Updated to latest version of Freemius SDK
* UPDATE: Code refactoring for performance

= 2.0.8 =
* BUG FIX: Fixed issue which admin was only showing first 20 lists.  Thanks @Israel
* UPDATE: Updated to latest version of Freemius SDK

= 2.0.7 =
* BUG FIX: Fixed issue in which if trying to auto load list from logged in user is enabled but the user is not logged in.
* UPDATE: Added in verbiage if a user is not a subscriber.
* UPDATE: Updated to latest vendor SDKs
* UPDATE: Confirmed WP 5.6+

= 2.0.6 =
* BUG FIX: Fixed issue in premium version where it was not pulling the correct contact if logged in.

= 2.0.5 =
* UPDATE: Updated to latest version of Freemius SDK
* UPDATE: Confirmed working with WP 5.5.x

= 2.0.4 =
* BUG FIX: Fixed issue which if you installed premium version without free version first it would error out.

= 2.0.3 =
* BUG FIX: Fixed issue in premium version where if pulling lists from logged in wordpress user, it would not pull correct first and last name
* BUG FIX: Fixed issue with 2.0.2 bug fix... :(

= 2.0.2 =
* BUG FIX: Fixed issue in premium version where on settings screen modified list name was not showing.

= 2.0.1 =
* UPDATE: Removed ActiveCampaign PHP SDK
* UPDATE: Upgraded all code to utilize ActiveCampaign V3 API
* UPDATE: Fixed various PHP Warnings
* UPDATE: Addressed issue with slowness relating to accounts that had a large number of automations.  This was a direct result from the ActiveCampaign V2 PHP SDK

= 1.1.4 =
* UPDATE: Confirmed working with Wordpress 5.1
* UPDATE: Updated ActiveCampaign API SDK
* UPDATE: Updated Freemius SDK

= 1.1.3 =
* NEW FEATURE: Added ability to only display specific lists via shortcode attribute.
* BUG FIX: Fixed issue with premium version placeholder text not showing up.

= 1.1.3 =
* NEW FEATURE: Added ability to only display specific lists via shortcode attribute.
* BUG FIX: Fixed issue with premium version placeholder text not showing up.

= 1.1.2 =
* FEATURE: Added ability to specify the sort order of the lists being displayed

= 1.1.1 =
* FIX: Fixed issue with tamper protection message not actually displaying.
* FIX: Fixed item with not being able to have both Load Lists from Logged in User AND Tamper Protection enabled.

= 1.1.0 =
* FEATURE: Added in ability to toggle top or bottom to display first and last name fields.
* FIX: Fixed warning message if first name and last name were not already set

= 1.0.9 =
* added in ability to override text that is outputted via javascript

= 1.0.8 =
* added in First and Last Name support
* added in ability to override all headings, placeholders and button labels

= 1.0.7 =
* FIX: Fixed bug which was introduced in 1.0.6 Again Big thanks to Thomas for pointing that out!

= 1.0.6 =
* FIX: Fixed bug which if you had hidden lists, user would then get unsubscribed from automatically when updating preferences.  Big thanks to Thomas for pointing that out!
* IMPROVEMENT: Removed several classes which were no longer needed.

= 1.0.5 =
* Updated translations
* Minor code refactoring

= 1.0.4 =
* Fixed warning message if email was passed in url but user was not a contact in ActiveCampaign
* Added work around code to account for GMAIL's + alias's when passing in email+alias@domain.com to address bar

= 1.0.3 =
* Added in ability for preference center to display all lists before user has to retrieve preferences.

= 1.0.2 =
* Changed the format of the preference sent to not be `<h4>` tags but rather `<label>` tags.
* Correct notice that could happen if there was no actual lists in ActiveCampaign
* Removed the text that said "Already Subscribed" or "Subscribe to list".  This seemed redundant.

= 1.0.1 =
* Added in Spanish, Spanish (Mexico), French, German Translations
* Corrected bug in loading i18n files
* Changed plugin version constant to something unique to not collide with other plugins.

= 1.0.0 =
* Initial Release

== Upgrade Notice ==
Updated third-party dependencies to latest versions (Freemius 2.5.9 to 2.5.10, Carbon 2.67.0 to 2.68.1)