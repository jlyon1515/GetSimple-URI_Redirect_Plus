# GetSimple - URI Redirect Plus
GetSimple CMS plugin. Redirect URIs to internal or external pages (with '301 Moved Permanently' header). Also view the count and date of last redirection for each redirect.

## Version 0.2.4 Changes
* Adding support for PHP 8. Fixed some associative array keys in the script that lacked quotation marks. PHP7 would assume the key should be quoted, and the script worked. PHP8 no longer made that assumption, so the script would break until the keys were put in quotes.

## Version 0.2.3 Changes
* Fixed an error where redirects to internal pages were created incorrectly if the page title had a colon
* When redirecting (or listing links to internal pages in the Existing Redirects table), URLs now conforms to the site's custom permalink setting (i.e., parent(s) and trailing slash after slug are included if appropriate)
* Added a redirect creation date to the XML (though it's not displayed in the Existing Redirects table)

## Version 0.2.2 Changes
* Imports redirect list from predecessor plugin on initial view, if available (see Earlier Versions)
* Select drop box for internal pages now sorts by parent then page title
* Added ability to redirect to external pages (i.e., other sites)
* Removed 'Incoming URI' and 'Redirect Page' terminology in favor of 'From' and 'To'
* Added redirect count and date of last redirection for each redirect
* Added multilingual support via the required I18N plugin (currently only English and Danish)

Note: For space reasons, long external destination URLs have their HTTP and WWW removed, as well as having their middle text removed, i.e., [example.com/...clste/wnerqylba](http://www.example.com/rtpfdwiHclste/wnerqylba "http://www.example.com/rtpfdwiHclste/wnerqylba"). You can see the full URL by mousing over the truncated external URLs.

## Earlier versions
This plugin is a successor to the no-longer-updated [original URI Redirect plugin](http://get-simple.info/extend/plugin/uri-redirect/150/) by Nathan Friemel (NathanF). Version numbering is continuing from where that earlier plugin left off (version 0.2.1).

## Installation
* Install required [I18N plugin](http://get-simple.info/extend/plugin/i18n/69/), if necessary.
* Unzip and upload the uri-redirect-plus folder and corresponding  uri-redirect-plus.php file into your GetSimple plugins folder. 
* Activate the plugin on the admin Plugins tab.
* Add redirects via the link on the side menu of the admin Pages tab.
