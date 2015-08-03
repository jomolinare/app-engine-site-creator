## Downloading ##

Download the trunk distribution of the code from Subversion by following the instructions provided [here](http://code.google.com/p/app-engine-site-creator/source/checkout).

You'll also need to download the App Engine SDK from [here](http://code.google.com/appengine/downloads.html).

## Customizing ##

Most user configurable settings are stored in the file configuration.py and are documented by comments in that file.  In addition, a unique name for the deployed instance should be registered with App Engine and specified in app.yaml

## Deploying ##

After customization app can be deployed by executing
```
appcfg.py update .
```
from the root directory of the application.  Once an install is running on App Engine, an administrator of the app should log in and go to http://your-app-name.appspot.com/admin/ and click on the "Create Page" link in the side bar.  This will result in the creation of a root page for the site, which can be optionally renamed.

## Administering ##

The App Engine admin interface allows for the creation of users profiles (only Google accounts with a registered profile are granted access to the site), user groups, pages, and access control lists.  The interfaces to modify this data are accessible via the sidebar in the admin interface.

Additionally, a sidebar can be specified in YAML format.  Clicking "add to sidebar" from the page editing interface will cause a YAML entry to be added to the sidebar definition.  That entry can then be repositioned from the sidebar editing view.