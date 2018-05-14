easy-collection-curation-work
=============================
[![Build Status](https://travis-ci.org/DANS-KNAW/easy-collection-curation-work.png?branch=master)](https://travis-ci.org/DANS-KNAW/easy-collection-curation-work)


SYNOPSIS
--------

    easy-collection-curation-work

DESCRIPTION
-----------

Job that collects the curated deposits from the data managers' personal curation areas


ARGUMENTS
---------

None

INSTALLATION AND CONFIGURATION
------------------------------
The preferred way of install this module is using the RPM package. This will install the binaries to
`/opt/dans.knaw.nl/easy-collect-curation-work`, the configuration files to `/etc/opt/dans.knaw.nl/easy-collect-curation-work`,

If you are on a system that does not support RPM, you can use the tarball. You will need to copy the
service scripts to the appropiate locations yourself.


BUILDING FROM SOURCE
--------------------

Prerequisites:

* Java 8 or higher
* Maven 3.3.3 or higher

Steps:

        git clone https://github.com/DANS-KNAW/easy-collection-curation-work.git
        cd easy-collection-curation-work
        mvn install
