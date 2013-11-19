VersionControl_SVN
==================

VersionControl_SVN is a simple OO-style interface for Subversion,
the free/open-source version control system.

Some of VersionControl_SVN's features:

* Full support of svn command-line client's subcommands.
* Multi-object factory.
* Source fully documented with PHPDoc.
* Stable, extensible interface.
* Collection of helpful quickstart examples and tutorials.

This package is hosted at http://pear.php.net/package/VersionControl_SVN

Please report all new issues via the PEAR bug tracker.

Pull requests are welcome!

Installation via Composer
-------------------------
VersionControl\_SVN also depends on some basic pear packages. So to install 
VersionControl\_SVN you have to add the following to your `composer.json`

  
    "repositories": [
        {
            "type": "vcs",
            "url": "git://github.com/jpgerdeman/VersionControl_SVN.git"
        },
      	{
            "type": "pear",
            "url": "http://pear.php.net"
        }
    ],
    "require": {
        "PEAR/VersionControl": "*",
		    "pear-pear.php.net/pear": "*"
		}

Testing, building
-----------------

To test, run either
$ phpunit tests/
  or
$ pear run-tests -r

To build, simply
$ pear package

To install from scratch
$ pear install package.xml

To upgrade
$ pear upgrade -f package.xml
