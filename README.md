# OpenPDF is a Java PDF library, forked from iText #

OpenPDF is a Java library for creating and editing PDF files with a LGPL and MPL open source license. OpenPDF is based on a fork of iText 4. We welcome contributions from other developers. Please feel free to submit pull-requests and bugreports to this GitHub repository.

[![Join the chat at https://gitter.im/LibrePDF/OpenPDF](https://badges.gitter.im/LibrePDF/OpenPDF.svg)](https://gitter.im/LibrePDF/OpenPDF) [![Build Status](https://api.travis-ci.org/LibrePDF/OpenPDF.png)](https://travis-ci.org/LibrePDF/OpenPDF) [![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.github.librepdf/openpdf/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.github.librepdf/openpdf) [![License (LGPL version 3.0)](https://img.shields.io/badge/license-GNU%20LGPL%20version%203.0-blue.svg?style=flat-square)](http://opensource.org/licenses/LGPL-3.0) [![License (MPL)](https://img.shields.io/badge/license-Mozilla%20Public%20License-yellow.svg?style=flat-square)](http://opensource.org/licenses/MPL-2.0)

## OpenPDF version 1.0.4 released 2017-10-11 ##
Get version 1.0.4 here - https://github.com/LibrePDF/OpenPDF/releases/tag/1.0.4

### Previous Versions
- [Version 1.0.3](https://github.com/LibrePDF/OpenPDF/releases/tag/1.0.3) _released 2017-07-24_
- [Version 1.0.2](https://github.com/LibrePDF/OpenPDF/releases/tag/1.0.2) _released 2017-06-03_
- [Version 1.0.1](https://github.com/LibrePDF/OpenPDF/releases/tag/1.0.1) _released 2017-01-28_
- [Version 1.0](https://github.com/LibrePDF/OpenPDF/releases/tag/1.0) _released 2016-05-03_

## License ##

GNU General Lesser Public License (LGPL) version 3.0 - http://www.gnu.org/licenses/lgpl.html

Mozilla Public License Version 2.0 - http://www.mozilla.org/MPL/2.0/


## Use OpenPDF as Maven dependency
Add this to your pom.xml file:

        <dependency>
            <groupId>com.github.librepdf</groupId>
            <artifactId>openpdf</artifactId>
            <version>1.0.5java7</version>
        </dependency>


## Background ##

Beginning with version 5.0 of iText, the developers have moved to the AGPL to improve their ability to sell commercial licenses. 
The OpenPDF project is a fork of iText 4, with a LGPL and MPL open source license.

## Changes ##
This repo has the following changes from the old "original" 4.2.0 version:
 - This code is taken from openpdf 1.0.5 https://github.com/LibrePDF/OpenPDF/tree/1.0.5
 - Code is modified to overcome below 2 vulnerabilitis 
 - CVE-2020-15522 Bouncy castle (https://www.cve.org/CVERecord?id=CVE-2020-15522)
 - Affected versions of this package are vulnerable to Timing Attack.
 - Upgraded org.bouncycastle:bcprov-jdk15on to version 1.66
 - CVE-2020-15250 Junit 4 (https://www.cve.org/CVERecord?id=CVE-2020-15250)
 - Affected versions of this package are vulnerable to Information Exposure
 - Upgraded junit:junit to version 4.13.1

## Contributing ##
Release the hounds!  Please send all pull requests.

## Dependencies ##

### Required: ###

 - BouncyCastle 1.66
   - Provider
   - PKIX/CMS
 - PDFRenderer
 - DOM4j

### Optional: ###

 - JUnit 4 - for unit testing
 - JFreeChart - for testing graphical examples
   - JFreeChart
   - JCommon
   - Servlet
