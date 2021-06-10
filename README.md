darktable_xmp_relative_dir
==========================

A Software patch to add option in Darktable to store xmp files in a sub-directory of your image directories

Last tested with: darktable-3.4.1 and darktable-3.0.2

Synopsys:
---------
* download a release source file, IE: darktable-3.4.1.tar.xz
* install all the Darktable compiling pre-requisites
* untar the source tar file
* cd into darktable-3.4.1
* Apply patch with something like:  patch -p1 < /tmp/optional-subdir-for-storing-xmp-files.patch
* Build darktable with:  build.sh
* Install new darktable
* In your home/.config/darktable/ directory...
* Add this option:  xmp_relative_dir=xmp
* IE like this:  echo xmp_relative_dir=xmp >>darktablerc
* Now create a xmp sub-directory just before you import a new directory of photos
* Or in existing dirs, create the sub-dir and move the .xmp files into the sub-dir named xmp 

Note:
-----
* Take backups before you try any of this. Backups of your image dirs and/or xmp files.
* Not responsibile for any file losses or corruption.
* I have been using this patch successfully on LINUX for the last three years
