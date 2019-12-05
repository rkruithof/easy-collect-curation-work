easy-collect-curation-work
==========================
[![Build Status](https://travis-ci.org/DANS-KNAW/easy-collect-curation-work.png?branch=master)](https://travis-ci.org/DANS-KNAW/easy-collect-curation-work)


SYNOPSIS
--------

    easy-collect-curation-work

DESCRIPTION
-----------

Job that collects the curated deposits from the data managers' personal curation areas


ARGUMENTS
---------
```
  Usage: 
  
     easy-split-multi-deposit

  Options:
  
    -h, --help      Show help message
    -v, --version   Show version of this program
```

INSTALLATION AND CONFIGURATION
------------------------------
The preferred way of install this module is using the RPM package. This will install the binaries to
`/opt/dans.knaw.nl/easy-collect-curation-work` and the configuration files to `/etc/opt/dans.knaw.nl/easy-collect-curation-work`,

To install the module on systems that do not support RPM, you can copy and unarchive the tarball to the target host.
You will have to take care of placing the files in the correct locations for your system yourself. For instructions
on building the tarball, see next section.


BUILDING FROM SOURCE
--------------------

Prerequisites:

* Java 8 or higher
* Maven 3.3.3 or higher
* RPM

Steps:

        git clone https://github.com/DANS-KNAW/easy-collect-curation-work.git
        cd easy-collect-curation-work
        mvn install

If the `rpm` executable is found at `/usr/local/bin/rpm`, the build profile that includes the RPM
packaging will be activated. If `rpm` is available, but at a different path, then activate it by using
Maven's `-P` switch: `mvn -Pprm install`.

Alternatively, to build the tarball execute:

    mvn clean install assembly:single
