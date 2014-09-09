=== User Frontend ===
Contributors: wpcodingde, inpsyde, HerrLlama
Donate Link: http://wpcoding.de
Tags: user, profile, login, logout, frontend, theme, multisite
Requires at least: 3.8
Tested up to: 4.0
Stable tag: 1.0.2
License: GPLv3

This plugin restricts the access to the admin panel and provides register, profile, login and logout features inside of the theme. This plugin is multisite-ready.

== Frequently Asked Questions ==

= What links uses this plugin? =

The user frontend works directly after activation. Every user will be redirected to the specific pages in the frontend. These are:

*	'http://yourdomain.tld/user-action/' - This is a custom URL which no user usually sees. It performs some actions, like updating profiles etc.
*	'http://yourdomain.tld/user-login/' - The login page
*	'http://yourdomain.tld/user-profile/' - The profil edit page
*	'http://yourdomain.tld/user-register/' - The user registration page
*	'http://yourdomain.tld/user-reset-password/' - The reset password page
*	'http://yourdomain.tld/user-forgot-password/' - The forgot password page
*	'http://yourdomain.tld/user-activation/' - The user activation page

= Can I style my own pages? =

Yes you can. As written in the 'Installation'-tab you only have to copy (donot move, just to be sure to have a backup) the templates from <code>/wp-content/plugins/user-frontend/templates/</code> to <code>wp-content/themes/your-theme/</code>. After that edit it wisely.

= Where is the logout located? =

The logout is a special case. It doesn't have a page to be displayed it is just an action performed by the system. However you can retrive the URL with the function <code>uf_logout_url()</code>. See its documentation for more information.

== Installation ==

1. Install and activate the plugin the known WordPress-Ways
2. Refresh your permalinks via Options -> Permalinks and click "Save"
3. For Developers: Copy the .php files from the template folder to your active theme folder and change the markup your way

== Screenshots ==

1. Profile edition with the twentythirteen theme

== Changelog ==

= 1.0.2 =
* Fixed problems with redirection and templates
* Implemented more API-Filters
* Added Doc-Block

= 1.0.1 =
* Update-Tests for WordPress 3.8