.. Comments start with '.. '. This line is an example.
.. This file encoded as reStructuredText, see http://docutils.sourceforge.net/rst.html
.. |author| replace:: Mike Carifio 
.. |email| replace:: mike@carifio.org
.. |book-title| replace:: *A Charming Book*
.. |repo| replace:: https://github.com/mcarifio/a-charming-book.git

:Author: |author| |email|


You Are Here
============

You're reading the `README` for the source content and supporting tooling for the very modest book |book-title|. 
The canonical repository for this content is '|repo|', a public git repository. The book's contents are also
encoded using reStructuredText and are located in `src`.

Quickstart
==========

You got this README with the following bash commands (or something similar)::

  export BOOKROOT=~/book
  export BOOKREPO=https://github.com/mcarifio/a-charming-book.git
  mkdir --parent $BOOKROOT; cd $BOOKROOT
  git clone $BOOKREPO ; cd $(basename $BOOKROOT .git) # ~/book/a-charming-book

You can read the content directly in `src`/*.rst. reStructuredText is quite readable in
"source" form. Or you can generate a suitable "output format" such as html using `sphinx`::

  sphinx-build src out/html
  gnome-open out/html/introduction.html





