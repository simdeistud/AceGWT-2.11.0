# AceGWT

An integration of the [Ace Editor](http://ace.c9.io/) into [GWT](http://www.gwtproject.org/).  If you want to embed a powerful text editor in a GWT application, AceGWT might be just what you're looking for!

The [wiki](https://github.com/daveho/AceGWT/wiki) has more information, including:

* [Documentation](https://github.com/daveho/AceGWT/wiki/Documentation) on using AceGWT in your application
* [Screenshots](https://github.com/daveho/AceGWT/wiki/Screenshots)
* [Status](https://github.com/daveho/AceGWT/wiki/Status): what is implemented and what isn't

Also, there is [javadoc](http://daveho.github.io/AceGWT/api/).

## What is included in this forked version

This version has been updated to use GWT 2.11.0 which has switced to using a different Maven repository.

To include this library in your project you need to set up this GitHub repository as a maven repo in your pom.xml file by doing as follows:

## Latest news

15 June 2018

* Converted the library and demo to Maven, using a github branch as repository
    * Package AceGWT lib `mvn clean gwt:generate-module compile gwt:package-lib`
    * Deploy AceGWT lib `mvn clean gwt:generate-module compile gwt:package-lib deploy`
    * Run demo app `mvn clean gwt:generate-module compile gwt:devmode`
* Updated to latest version of Ace (1.3.3)
* All courtesy of [José C.Paiva](https://github.com/josepaiva94).

06 February 2016:

* Bugfix for [ConcurrentModificationException on removeAllMarkers()](https://github.com/daveho/AceGWT/pull/25), courtesy of [Gottfried Huber](https://github.com/paxdei).

20 January 2015:

* Support for selection change events, courtesy of [Roman Sutormin](https://github.com/rsutormin).

12 October 2014:

* Updated to latest version of Ace from [here](https://github.com/ajaxorg/ace-builds/tree/master/src), plus applied a small fix which has been submitted as a [push request](https://github.com/ajaxorg/ace/pull/2189) (code changes in this push request already applied to code in this repository).
* Added autocomplete tooltip support based on latest updates to Ace Editor ([forum](https://groups.google.com/forum/#!topic/ace-discuss/M4vw4XdVzBU), push request [2148](https://github.com/ajaxorg/ace/pull/2148)).

27 June 2014:

* Added experimental support for custom autocompleters, based on suggestions from Chris Ainsley.

26 June 2014:

* Updated to latest version of Ace. A handful of new modes and themes added.  Autocomplete is now supported.

18 March 2014:

* Updated to latest version of Ace.  Various new editor modes and themes added.  Also, AceGWT now packages the minified versions of the Ace JavaScript files, which should reduce load time.
* Issues with the text cursor position in Safari may be fixed.

25 June 2013:

* Updated to latest version of Ace, many new editor modes added.
* Initialization of AceEditor object has changed: the default constructor has been un-deprecated, and **no** changes should be made to the .ace\_editor CSS class.
