
# Fork of TextGrid

This is a fork from https://github.com/kylebgorman/textgrid

I made some minor changes in this fork such that the textgrid file loading has more tolerance on mal-formatted inputs.
E.g., textgrid files with below formatting issues can still be loaded:

- 1st line is empty. The script will still try to read the header from the 2nd line.
- The stated number of intervals does not match the actual number of intervals in the content. The loading of intervals will stop when hitting an empty line without causing exception.

# Original README

textgrid.py
===========

Python classes for Praat TextGrid and TextTier files (and HTK .mlf files)

Kyle Gorman <kylebgorman@gmail.com> and contributors (see commit history).

How to cite:
------------

While you don't have to, if you want to cite textgrid.py in a publication, include a footnote link to the source:

    http://github.com/kylebgorman/textgrid.py/

How to install:
---------------

The code can be placed in your working directory or in your `$PYTHONPATH`,  and then imported in your Python script. You also can install it via `pip`, like so:

    pip install textgrid

(if you're not working in a virtualenv, you may need to do this with `sudo`.)

Synopsis:
---------

See the docstrings in `textgrid.py`
