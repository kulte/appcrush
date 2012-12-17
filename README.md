appcrush
========

Modified version of the original appcrush script written by Peter Boctor to run unzip and extract images from an IPA package. Modified to account for the new location of developer tools.

Credit
------

Peter Boctor wrote the original appcrush script for extracting images from an IPA package. This script adds some simple modifications to account for the new location of developer tools, since the Boctor script was written awhile ago. Credit for good stuff is Peter's, and responsibility for bad stuff is mine.

Introduction
------------

It can be helpful to draw inspiration from how existing applications are built, and to that extent this script allows you to extract and view images from iOS applications you've downloaded from the App Store. 

Downloading and using this script
---------------------------------

	mkdir bin # If you don't have ~/bin directory
	cd ~/bin
	git clone https://github.com/kulte/appcrush.git
	mv appcrush/appcrush.rb .
	chmod +x appcrush.rb

If you have ~/bin in your path, then this script will be executable from anywhere on your system.

Extracting images from an IPA package
-------------------------------------

The first thing you must do is find the app you've downloaded in iTunes. Right click on the app and click "Show in Finder" to accomplish this. Now that you have this, simply run the script for a specific IPA on your system:
	
	appcrush.rb PATH_TO_APP.ipa

This will unzip and extract all images from the package, uncrushing each as it is extracted. You'll be left with a folder on your Desktop with the extracted images.

Usage Caveat
------------

This is really first and foremost, but it's worth mentioning that you should not use these images in your own applications. This technique is very useful to see how something was accomplished, but it is not meant as a tool for stealing other developer's assets!

Happy Uncrushing!
---------------
