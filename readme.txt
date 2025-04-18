=== Contact Form 7 Add Password field ===
Contributors: kimipooh
Tags: contact form
Requires at least: 6.2
Requires PHP: 7.4
Tested up to: 6.7.2
Stable tag: 5.0.1
License: GPL v2
License URI: http://www.gnu.org/licenses/gpl-2.0.html


The plugin is to add a password filed to Contact form 7 plugin.
 
== Description ==

The plugin is to add a password filed to Contact form 7 plugin.
ex. [password example] (optional) /  [password* example] (required)

== Installation ==

It's the simple.
Please install this plugin and activate it.

== Frequently Asked Questions ==
= How to use the ability of the password check? =
Enter the value of the "name" on the field if you wish to verify a value of a password field. 
Ex. If you set [password password-100], set [password* password-101 password_check:password-100]. Please pay attention a miss with uppercase and lowercase letters.

= How the use the ability to display a password? =
Set the "id" and the value sets same as "name" value.
Ex. If you set [password password-100], change to [password password-100 id:password-100].

The feature uses the library(Web fonts and CSS) of Font Awesome ( https://fontawesome.com/ ).

= How the customize the validation check? =
Please see the following document.
https://info.cseas.kyoto-u.ac.jp/en/links-en/plugin-en/wordpress-dev-info-en/cf7-add-password-field_en

= How to save a password in hashed form =
This plugin only adds a password field the Contact Form 7 plugin and does not encrypt(hash) input data.
If you want to hash a password value for keeping a database using an other plugin or sending by email, you need to add the code for hashing the data  when you submit it pass through Contact Form 7, for example in your theme’s functions.php.
Reference: “Changing Contact Form 7 input values (28 January, 2023)” in https://info.cseas.kyoto-u.ac.jp/en/links-en/plugin-en/wordpress-dev-info-en/cf7-add-password-field_en

== Screenshots ==
1. Setting of Contact Form 7
2. View of Contact Form 7

== Changelog ==
= 5.0.1 = 
* Tested up WordPress 6.7.2 with PHP 8.3.19 and 8.4.5.

= 5.0 =
*Supported for the Tag generator (version 2), which was changed in version 6.0 of Contact Form 7. For more information, please see https://aurisecreative.com/blog/2024/11/how-to-use-tag-generator-version-2-in-contact-form-7/.

= 4.2 =
* Added 5 options (Icon_position, Icon_float, Icon_top, Icon_margin, Icon_marginleft) to customize icon position. Each of them corresponds to position, float, top, margin, and margin-left. The position setting is required for customization.

= 4.1 =
* Update the css and webfonts powered by fontawesome.com from 5.15.4 to version 6.4.2.
* New "hideIcon" option has been added. By setting this, it can hide the icon for displaying passwords.
* Tested up WordPress 6.3 with PHP 8.2.
* Tested up WordPress 6.5.2 with PHP 8.3.6.

= 4.0 =
* Fxied the issue for the version 5.8 of Contact form 7; Since the version 5.8 of Contact form 7 ignores the id attribute if the same ID is already used for another element.
* Changed to require WordPress 6.2+ and PHP 7.4+ according to the specifications required by Contact Form 7 itself.

= 3.31 =
* Fixed some error message.

= 3.3 =
* Added "specific_password_check" option for matching with specific passwords specified in advance.

= 3.2 =
* Fixed the markup changes in form controls, such as error message, since the version 5.6 of Contact Form 7 plugin (https://contactform7.com/2022/05/20/contact-form-7-56-beta/).
* Tested up 6.1

= 3.1 =
* Fixed misspelling of id in maxlength on input tag (it was naxlength).

= 3.0 =
* Fixed the password strength check.

= 2.10 =
* Added character count option "minlength" ad "maxlength" implemented in Contact Form 7 plugin.
* If both of "password_min" and "minlength" are set, the "minlength" setting takes precedence.

= 2.92 =
* Fixed one of  language translation.
* Tested up 6.0

= 2.91 =
* The css and webfonts powered by fontawesome.com for the password display icon was involded to the plugin for supporting an offline or CDN.

= 2.9 =
* Added the hook "wpcf7_k_password_validation_filter" for customizing the validation check. Please refer to the FAQ for details.

= 2.8 =
* Added the ability to display a password. Please refer to the FAQ for details.

= 2.7 =
* Fixed some language transtaion.
* Added the ability to verify a field value like a password. 

= 2.6 =
* Fixed the error message regarding the description on the password generation form.
* Tested up 5.7 with PHP 8.0
* Tested up 5.8

= 2.5 =
* Added two restrictions; "Number of characters", “Password Strength".
* Tested up 5.5.1 with PHP 7.4
* Tested up 5.6 with PHP 7.4

= 2.4 =
* Fixed the issue where hook "cf7-add-password-field-features" were not available.
* Tested up 5.5 with PHP 7.4

= 2.3 =
* Add the option of placeholder text (https://contactform7.com/en/setting-placeholder-text/).
* Tested up 5.3.2 with PHP 7.4

= 2.2 =
* Tested up 5.3.1
* Add the hook "cf7-add-password-field-features" for customizing wpcf7_add_form_tag option.

= 2.1 =
* Tested up 5.2.4 with PHP 7.3.
* Fixed the arguments of load_plugin_textdomain as WordPress 3.7 or later.

= 2.0 =
* Tested up 5.2.2 with PHP 7.3.
* Support "Password" form button.

= 1.0 =
* First release.

== Upgrade Notice ==
