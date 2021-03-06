====
Mate
====

Mate is an implementation of matchers for Python's ``unittest``
module, which it largely tears out from `testtools
<https://testtools.readthedocs.org/>`_\ .

There are two purposes in doing so:

    * Extract portions suitable for submission upstream for inclusion in the
      unittest module and modify them so that they're able to be integrated
    * Separate out details, matchers, and delayed assertions from
      ``testtools.TestCase`` so that they can be used with other ``TestCase``
      subclasses

the second of which supports the first, and an ultimate goal is to contribute a
shared implementation that can be used by both the standard library, testtools,
and any other consumers.


Licensing
---------

The fundamental API and large portions of the code are taken with
slight modifications from the aformentioned testtools package, which
is MIT-licensed. Its license and authors are included in the license
distributed with this package.
