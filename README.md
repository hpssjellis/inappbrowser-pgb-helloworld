pgb-rookie-inappbrowser

No idea if I am doing things correctly but this simple Android App does open all links into the default Android (Chrome) web browser on at least a Samsung Galaxy S3.

All calls to _blank  _system  _self seem useless and I could not get the Phonegap Browser to work at all once the inappbrowser pluggin was working

The main criteria seems to be having an <access = ""> in your config.xml file. Not sure why since the  website does not have to go to that site.


