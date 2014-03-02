jsArchive
=========

fully in-browser JavaScript Archive format to allow offline applications to read and write archive files.

Dependencies
============

depends on FileSaver.js and Blob.js from eligrey on github. These have been added as submodules.
To build simply call

$ cd jsArchive 
$ git submodule update --init --recursive # pulls dependencies

Then open Demo.html. This example works offline. It allows you to add and view content of text, image, and video files.
