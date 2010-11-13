dwbackup
========

Synopsis
--------

dwbackup provides a simple means to manage multiple duplicity backup sets.

Requirements
------------

* Perl
* Duplicity
* Config::INI

Usage
-----

Configuration is done via a standard INI style file. By default, this is
/usr/local/etc/dwbackup.ini. Each backup set is defined by an INI section.
Each section must have at least the 'source' identifier. See the included
dwbackup.ini file for examples.
