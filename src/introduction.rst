.. Comments start with '.. '. This line is an example.
.. This file encoded as reStructuredText, see http://docutils.sourceforge.net/rst.html
.. |author| replace:: Mike Carifio 
.. |email| replace:: mike@carifio.org
.. |book-title| replace:: *A Charming Book*
.. |repo| replace:: https://github.com/mcarifio/a-charming-book.git

:Author: |author| |email|

Introduction
============

|book-title| explains `juju`, a service orchestration tool developed by Canonical, the Ubuntu distro company. 
Juju provides the capabilities to:

* Provision computing resources from "the cloud".
* Deploy services to those machines, for example the Apache webserver, wordpress or mysql.
* Connect services together to do things. For example, wordpress requires both Apache and
  mysql to provide a blog service. 

Juju handles certain common needs, like machine provisioning and deployment in an OpenStack cloud. But rely
on sets of scripts, together called a  *charm*, to deploy the specific services (wordpress, mysql) 
and wire them together.

This book describes enough juju for a devop to write charms. This includes how to test and document them.

The book's approach is *bottom up* and *learn by doing*. We start with very simple charms executed "locally",
for example on your host (laptop or desktop computer).
