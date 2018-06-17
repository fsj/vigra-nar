VIGRA Computer Vision Library
=============================

Packages the [VIGRA Computer Vision Library][vigra] as a [Maven][maven]
artifact using the [NAR plugin][nar]. Please refer to the VIGRA home page for
usage documentation and licensing conditions.

Currently the core part of the VIGRA library which does not require external
dependencies has been packaged as **vigra-core**. The main omissions are the
import/export ('impex') functionality for loading and storing images in various
formats, random forests and the fast fourier transform algorithms, which will
be added as needed in form of separate Maven modules.

Building
--------

To build and install the Maven artifact execute:

    $ mvn clean install

Usage
-----

Add **vigra-core** as a dependency in your projects:
```xml
<dependency>
    <groupId>io.github.fsj</groupId>
    <artifactId>vigra-core</artifactId>
    <version>1.11.1+nar.1</version>
    <type>nar</type>
</dependency>
```

[vigra]: https://github.com/ukoethe/vigra
[maven]: https://maven.apache.org
[nar]: http://maven-nar.github.io
