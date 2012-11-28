.. Comments start with '.. '. This line is an example.
.. This file encoded as reStructuredText, see http://docutils.sourceforge.net/rst.html
.. |author| replace:: Mike Carifio 
.. |email| replace:: mike@carifio.org
.. |book-title| replace:: *The Little Charmer*
.. |repo| replace:: https://github.com/mcarifio/the-little-charmer.git

.. http://docutils.sourceforge.net/docs/ref/rst/directives.html#date
.. |date| date::
.. |time| date:: %H:%M

:Author: |author| |email|


You Are Here
============

You're reading the `README` for the source content and supporting tooling for the very modest book |book-title|. 
The canonical repository for this content is '|repo|', a public git repository. The book's contents are also
encoded using reStructuredText and are located in `source` consistent with the conventions of Sphinx 
<http://sphinx-doc.org/tutorial.html>.


Quickstart
==========

You got this README with the following bash commands (or something similar)::

  export BOOKROOT=~/book
  export BOOKREPO=https://github.com/mcarifio/the-little-charmer.git
  mkdir --parent $BOOKROOT; cd $BOOKROOT
  git clone $BOOKREPO ; cd $(basename $BOOKROOT .git) # ~/book/the-little-charmer

You can read the content directly in `source`/*.rst. reStructuredText is quite readable in
"source" form. Or you can generate a suitable "output format" such as html using ``sphinx-build`` in
directory ``$BOOKDIR``::

  sphinx-build -b html source build/html # in $BOOKROOT, generates $BOOKROOT/build/html
  gnome-open build/html/index.html # view HTML output


