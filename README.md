inappbrowser-pgb-helloworld
===========================

No idea if I am doing things correctly but this simple Android App does open all links into the default Android (Chrome) web browser on at least a Samsung Galaxy S3.

All calls to _blank  _system  _self seem useless and I could not get the Phonegap Browser to work at all once the inappbrowser pluggin was working

The main criteria seems to be having an  <access origin="anySite.com" />   in your config.xml file. Not sure why since the  website does not have to go to that site. Note the two values 



        <access />            - a blank access tag denies access to all external resources.
        <access origin="*" /> - a wildcard access tag allows access to all external resource.

 did not work. Or at least all links went to the internal phonegap browser, which I think happens even if you do not have the inappbrower installed at all
 
 Done Jan 10, 2014
 
 
 
 
 Presently not seeing this behaviour at all. Either I do not use the plugin and all webpages go to the internal phongap browser or I use the plugin and all links to the installed device (Chrome on my phone)
 
 target: The target in which to load the URL, an optional parameter that defaults to _self. (String)

_self: Opens in the Cordova WebView if the URL is in the white list, otherwise it opens in the InAppBrowser.
_blank: Opens in the InAppBrowser.
_system: Opens in the system's web browser.


