<pre>Cannibal Open Touch Themes
==============================

The included themes are examples for custom sdcard themes; these can be side-loaded and ran on any device running Cannibal Open Touch Recovery v2.1-dev2 or above.

At this time the theme engine only supports one custom theme at a time to be loaded from '/sdcard/cotrecovery/theme/custom/'.

All themes for the gingerbread based recovery consist of 21 pngs files and one ini file (png defined as following):
<ul>
<li>A primary background png to be labeled icon_background.png</li>
<li>4 secondary background images to be displayed during different processes (these are):</li>
</ul>
	* icon_install.png : to be displayed when installing a zip.
	* icon_error.png : to be displayed whenever there is a generic error.
	* icon_firmware_install.png : to be displayed when flashing a firmware update (this is uncommon).
	* icon_firmware_error.png : to be displayed upon error while flashing a firmware update (like the previous this is uncommon).
<ul>
<li>8 progress indicator images (as listed):</li>
</ul>
	* progress_empty.png (recommended that you pull this from an existing theme).
	* progress_fill.png (set this to your theme color).
	* indeterminate1.png - indeterminate6.png (recommended that you pull these from an existing theme as well).
<ul>
<li>8 navigation icons (defined as following):</li>
</ul>
	* icon_select.png : select icon.
	* icon_selectM.png : select icon when depressed.
	* icon_back.png : back icon.
	* icon_backM.png : back icon when depressed.
	* icon_up.png : up icon.
	* icon_upM.png : up icon when depressed.
	* icon_down.png : down icon.
	* icon_downM.png : down icon when depressed.

The theme ini should be something similar to the following (replace the colors with those of the html color code for the desired theme).

	;
	; Dooderbutt Blue Theme
	;
	
	[Theme]
	Name = custom ; Do not change this!
	UICOLOR0 = 0 ; Color0
	UICOLOR1 = 0 ; Color1
	UICOLOR2 = 255 ; Color2

One thing to consider before creating a theme is that not all devices use the same resolution, what looks good on one device will likely require different size images to work on another device.

<ul>
<li>Once you have your theme created and tested, feel free to submit it for sharing with other Cannibal Open Touch users by forking this repo and opening a pull request.</li>
<li>Please make sure all pull requests use the following format for branch names:</li>
</ul>
	* XX-RESxRES
	* Where XX is the recovery base; for example 'gb' for gingerbread.
	* The res entries are dependent of the device where X or Y is listed prior in order dependent on whether the device is portrait or landscape.
	* Please see current branch names for an example.
