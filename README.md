dwbackup
========

Name
----

dwbackup - Provides a simple means to manage multiple duplicity backup sets.

Synopsis
--------

dwbackup [--config config_file] [set]

Requirements
------------

* Perl
* Duplicity
* Config::INI

Usage
-----

dwbackup eases the management of running multiple duplicity backup sets by
allowing configuration via standard INI files. Instead of having a separate
cron with a long command line for each set, or a shell script wrapper with a
collection of long command lines, dwbackup allows multiple sets to be
specified in a single configuration file. When dwbackup is run, it parses the
configuration file and performs the appropriate commands to back up each set.

By default, the configuration file is located at /usr/local/etc/dwbackup.ini.
Each backup set is defined by a separate INI section. Each section must have
at least the 'source' identifier. See the included dwbackup.ini file for
examples.
