<script>{
	"title": "Download jQuery",
	"customFields": [
		{ "key": "hide_title", "value": 1 }
	]
}</script>

## Downloading jQuery

Compressed and uncompressed copies of jQuery files are available. The uncompressed file is best used during development or debugging; the compressed file saves bandwidth and improves performance in production.
You can also download a [sourcemap file](http://www.html5rocks.com/en/tutorials/developertools/sourcemaps/) for use when debugging with a compressed file.
The map file is _not_ required for users to run jQuery, it just improves the developer's debugger experience.
As of jQuery 1.11.0/2.1.0 the `//# sourceMappingURL` comment is [not included](https://blog.jquery.com/2014/01/24/jquery-1-11-and-2-1-released/) in the compressed file.

To locally download these files, right-click the link and select "Save as..." from the menu.

### jQuery 1.x

The jQuery 1.x line had major changes as of jQuery 1.9.0. We _strongly_
recommend that you also use the jQuery Migrate plugin if you are upgrading from
pre-1.9 versions of jQuery or need to use plugins that haven't yet been updated.
Read the [jQuery 1.9 Upgrade Guide](https://jquery.com/upgrade-guide/1.9/)
and the [jQuery 1.9 release blog post](https://blog.jquery.com/2013/01/15/jquery-1-9-final-jquery-2-0-beta-migrate-final-released/)
for more information.

<a href="https://code.jquery.com/jquery-1.12.4.min.js" download>Download the compressed, production jQuery 1.12.4</a>

<a href="https://code.jquery.com/jquery-1.12.4.js" download>Download the uncompressed, development jQuery 1.12.4</a>

<a href="https://code.jquery.com/jquery-1.12.4.min.map" download>Download the map file for jQuery 1.12.4</a>

[jQuery 1.12.4 release
notes](https://blog.jquery.com/2016/05/20/jquery-1-12-4-and-2-2-4-released/)

### jQuery 2.x

jQuery 2.x has the same API as jQuery 1.x, but _does not support Internet Explorer 6, 7, or 8_.
All the notes in the [jQuery 1.9 Upgrade Guide](https://jquery.com/upgrade-guide/1.9/) apply here as well.
Since IE 8 is still relatively common, we recommend using the 1.x version unless you
are certain no IE 6/7/8 users are visiting the site.
Please read the [2.0 release notes](https://blog.jquery.com/2013/04/18/jquery-2-0-released/) carefully.

<a href="https://code.jquery.com/jquery-2.2.4.min.js" download>Download the compressed, production jQuery 2.2.4</a>

<a href="https://code.jquery.com/jquery-2.2.4.js" download>Download the uncompressed, development jQuery 2.2.4</a>

<a href="https://code.jquery.com/jquery-2.2.4.min.map" download>Download the map file for jQuery 2.2.4</a>

[jQuery 2.2.4 release
notes](https://blog.jquery.com/2016/05/20/jquery-1-12-4-and-2-2-4-released/)

## Downloading jQuery using Bower
jQuery is registered as a package with [Bower](http://bower.io). You can install the latest version of jQuery with the command:
```
bower install jquery
```
This will install jQuery to Bower's install directory, the default being `bower_components`. Within `bower_components/jquery/dist/` you will find an uncompressed release, a compressed release, and a map file.

The jQuery Bower package contains additional files besides the default distribution. In most cases you can ignore these files, however if you wish to download the default release on its own you can use Bower to install jQuery from one of the above urls instead of the registered package. For example, if you wish to install just the compressed jQuery file, you can install just that file with the following command:
```
bower install https://code.jquery.com/jquery-2.2.4.min.js
```

## jQuery Migrate Plugin

We have created the [jQuery Migrate plugin](https://github.com/jquery/jquery-migrate/#readme)
to simplify the transition from older versions of jQuery. The plugin restores deprecated features and behaviors so that older code will still run properly on jQuery 1.9 and later. Use the _uncompressed development_ version to diagnose compatibility issues, it will generate warnings on the console that you can use to identify and fix problems. Use the _compressed production_ version to simply fix compatibility issues without generating console warnings.

<a href="https://code.jquery.com/jquery-migrate-1.3.0.min.js" download>Download the compressed, production jQuery Migrate 1.3.0</a>

<a href="https://code.jquery.com/jquery-migrate-1.3.0.js" download>Download the uncompressed, development jQuery Migrate 1.3.0</a>

## Cross-Browser Testing with jQuery

Be sure to test web pages that use jQuery in all the browsers you want to support. The [Microsoft Developer Resources](https://developer.microsoft.com/en-us/microsoft-edge/) site makes available [virtual machines](https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/) for testing many different versions of Internet Explorer. Older versions of other browsers can be found at [oldversion.com](http://oldversion.com/).

## jQuery Pre-Release Builds

The jQuery team is constantly working to improve the code. Each commit to the Github repo generates a work-in-progress version of the code that we update on the jQuery CDN. _These versions are sometimes unstable and never suitable for production sites._ We recommend they be used to determine whether a bug has already been fixed when reporting bugs against released versions, or to see if new bugs have been introduced.

<a href="https://code.jquery.com/jquery-git.js" download>Download the work-in-progress jQuery build</a>

## Using jQuery with a CDN

[CDNs](https://en.wikipedia.org/wiki/Content_delivery_network) can offer a performance benefit by hosting jQuery on servers spread across the globe. This also offers an advantage that
if the visitor to your webpage has already downloaded a copy of jQuery from the same CDN, it won't have to be re-downloaded.

### jQuery's CDN provided by [MaxCDN](https://www.maxcdn.com)

The jQuery CDN supports [https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity](Subresource Integrity) (SRI) which allows the browser to verify that the files being delivered have not been modified. This [https://www.w3.org/TR/SRI/](specification) is currently being implemented by browsers. Adding the new integrity attribute will ensure your application gains this security improvement as browsers support it.

To use the jQuery CDN, just reference the file in the script tag directly from the jQuery CDN domain. You can get the complete script tag, including Subresource Integrity attribute, by visiting https://code.jquery.com and clicking on the version of the file that you want to use. Copy and paste that tag into your HTML file.

Starting with jQuery 1.9, [sourcemap files](https://blog.jquery.com/2013/01/09/jquery-1-9-rc1-and-migrate-rc1-released/#sourcemaps) are available on the jQuery CDN. However, as of version 1.10.0/2.1.0 the compressed jQuery no longer includes the sourcemap comment in CDN copies because it requires the the uncompressed file and sourcemap file to be placed at the same location as the compressed file. If you are maintaining local copies and can control the locations all three files, you can add the sourcemap comment to the compressed file for easier debugging.

To see all available files and versions, visit [https://code.jquery.com](https://code.jquery.com)

### Other CDNs

The following CDNs also host compressed and uncompressed versions of jQuery releases. Starting with jQuery 1.9 they may also host [sourcemap files](https://blog.jquery.com/2013/01/09/jquery-1-9-rc1-and-migrate-rc1-released/#sourcemaps); check the site's documentation.

**Note that there may be delays between a jQuery release and its availability there. Please be patient, they receive the files at the same time the blog post is made public. Beta and release candidates are not hosted by these CDNs.**

* [Google CDN](https://developers.google.com/speed/libraries/devguide#jquery)
* [Microsoft CDN](https://www.asp.net/ajax/cdn#jQuery_Releases_on_the_CDN_0)
* [CDNJS CDN](https://cdnjs.com/libraries/jquery/)
* [jsDelivr CDN](https://www.jsdelivr.com/#!jquery)

## About the Code

**jQuery is provided under the <a href="https://jquery.org/license/">MIT license</a>.**

The code is hosted and developed in the [jQuery GitHub repository](https://github.com/jquery/jquery). If you've spotted some areas of code that could be improved, please feel free to discuss it on the [Developing jQuery Core Forum](https://forum.jquery.com/developing-jquery-core). If you'd like to participate in developing jQuery, peruse our [contributor site](https://contribute.jquery.org) for more information.

To find and download plugins developed by jQuery contributors, please visit the <a href="https://plugins.jquery.com/">Plugins site</a>. Plugin authors are responsible for maintenance of their plugins. Feedback on plugins should be directed to the plugin author, not the jQuery team.

### Build from Git

*Note:* To just use the latest work-in-progress version of jQuery, please try the jQuery Pre-Release Build described above.

All source code is kept under Git revision control, which you can browse online. The repository's <a href="https://github.com/jquery/jquery/blob/master/README.md">README</a> has more information on building and testing your own jQuery, as well as instructions on creating a custom build that excludes some APIs to reduce file size.

If you have access to Git, you can connect to the repository here:

``` bash
git clone git://github.com/jquery/jquery.git
```

You can also check out and build a specific version of jQuery from GitHub:

``` bash
git clone git://github.com/jquery/jquery.git
git checkout 1.2.6
```

The README file for a specific version will have instructions for building that version, as the process has changed over time.

***

## Past Releases

All past releases can be found on the [jQuery CDN](https://code.jquery.com).

