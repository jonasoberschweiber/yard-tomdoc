# RELEASE HISTORY

## 0.4.0  2012-03-04

This major release now uses tomparse gem for parsing TomDoc,
instead of the tomdoc gem. This library only handles parsing
and none of the other features than the tomdoc gem provides,
so it is more suited to yard-tomdoc's needs. In addition,
support for the latest TomDoc specification are included in
this release.

Changes:

* Use tomparse gem for parsing TomDoc.
* Improve support for TomDoc features.


## 0.3.1 | 2011-11-10

This release simply modernizes the build configuration
and adds an systems test. Functionally it has not changed.

Changes:

* Modernize the build configuration.
* Add systems test and integrate Travis CI.


## 0.3.0 | 2011-06-08

Okay,looks like tomdoc is ready to handle the dependency. If there
are any problems with this there is a fallback plugin, `tomdoc-intern`.

Changes:

* Depend on tomdoc proper.
* Add fallback `yard-tomdoc-intern.rb`


## 0.2.1 | 2011-05-23

There is an as-of-yet undetermined issue with running yard-tomdoc under
Ruby 1.9. By depending on an internal copy of TomDoc's TomDoc class we
are able to avoid the problem. So, for now we are removing the dependency
on the `tomdoc` gem until this is fully resolved.

Changes:

* Remove dependency on tomdoc.
* Require internal copy of tomdoc/tomdoc.rb.


## 0.2.0 | 2011-05-22

This is first packaged release of YARD-TomDoc. Some minor improvements
have been made from the original version and the project now actually
depends on the `tomdoc` library.

Changes:

* Depend on `tomdoc` library.
* Support YARD's method return object.
* Fix args issues when missing section.
