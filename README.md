Images_To_ePub
==============

Convert a folder with images to an ePub file. Great for photo albums, comics, and manga!

Run <code>main.py</code> or <code>_Gui.py</code> to start a GUI. Select a folder, a file to save to and the name of the book (this is what most eBooks show as name).

The directory will be searched for image files (png,jpg,GIF) and every image will be added to the ePub file.
The first image with the word "cover" somewhere in the name is used as the cover, but some readers will use the first page regardless of this.
Every subfolder of the given directory will be a separate chapter in the book.
You will not notice this while reading, but if you want to jump to another chapter you can use the table of contents. Images will appear before the images of sibling directories.

Some screens do not support color images, so this program has the option to turn all images into grayscale versions.
The maximum resolution of the images can also be set, resulting in the resizing of images if needed.
The original image files will not be changed.

This program can also run without a GUI. Run <code>main.py</code> with the <code>-h</code> flag to get more info.
You can also perform a batch operation by giving a list of directories (more than one directory) as arguments to <code>main.py</code>.

Changes made in this fork (Specifically for Warp Pages option)
----------------------------------------------------------------
* This fork is customized for Manga output.
* ePubs generated will be RTL (Right to Left) paginated.
* Images are shown as Spread Pages only (Even in Portrait Mode!) so, joining spread pages is not recommended. Also, keep any original blank pages so spreads are correctly shown.
* Most readers should now show images without distortion.
* Tested on:
  * iBooks
  * [Bib/i](https://bibi.epub.link/)
  * [Calibre eBook Reader](https://calibre-ebook.com/)


Requirements
------------

* Python 3.6 or later
* jinja2
* Pillow

License
-------

Please read the license. If you are lazy go to http://choosealicense.com/licenses/agpl/ and read the summary on the right.

If you have any ideas of how to make this code more awesome please let me know via the issue tracker!

Info about ePubs
----------------

* To check if your ePub file is correct: http://validator.idpf.org/
