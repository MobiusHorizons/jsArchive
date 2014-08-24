jsArchive
=========

Fully in-browser JavaScript Archive format to allow offline applications to read and write multiple files at once.

because of the way it works, this Archive format is really fast even with large files. I opened an 8GB file almost instantly because the metadata is at the beginning, meaning that the browser does not have to read the whole Archive (unlike zip files) in order to extract one of the files.


Dependencies 
============

These are automatically pulled by GithubWindows, so the following is for command line only.


The demo uses FileSaver.js and Blob.js from eligrey on github to ensure a consistant API. These have been added as submodules.
To build simply call

```bash
$ cd jsArchive 				  # goto git repo
$ git submodule update --init --recursive # pulls dependencies
```

Then open Demo.html. This example works offline. It allows you to add and view content of text, image, and video files.

TODO's
======

- ~~I would love to make this work in Internet Explorer (at least 10+) I work on linux, so this is hard, but if anyone wants to take a look please let me know.~~ Tested working in ie 10. Had to enable downloads in internet options.

- ~~add support for removing files.~~

- ~~add duplicate filename handling.~~

