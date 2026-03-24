[![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)


# Preamble

This GitHub repository contains the sources of a library called ADQLLib. This library is a Java implementation of the [ADQL-2.1](http://www.ivoa.net/documents/ADQL/20231215/index.html "Astronomical Data Query Language") standard and related standards and protocols.

It has been forked from the original [VOLLT repository](https://github.com/gmantele/vollt) created by Grégory Mantelet with the following aims

- Isolate the ADQLLib library from the rest of the original VOLLT codebase and make it available as a standalone library
    - this allows easier maintenance and development of the ADQLLib library as PRs related to this library can be merged without having to merge the rest of the codebase
- Allow the future development of the ADQLLib library to be driven by the needs of Javastro libraries.
    - though it is still an aim to make ADQLLib a standalone library


# Build the library

This project uses [Gradle](https://gradle.org/) as build automation tool. It
is configured for each project in its `build.gradle`. All dependencies
declared in this configuration are automatically resolved. It also includes
configuration for Eclipse and IntelliJ IDEA ; for Visual Studio Code one may
install an extension such as [Gradle for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-gradle).

To use Gradle, one may install it on its own computer (see
[installation instructions](https://gradle.org/install/) in the Gradle website).
Alternatively, one may simply use the provided [gradlew](gradlew) script
(or [gradlew.bat](gradlew.bat) for Windows) to run exactly the same build
commands. This latter will download Gradle in the temporary hidden directory
dedicated to this project [.gradle/](.gradle). This way, you are always
guaranteed to use exactly the same version of Gradle used by the source code
developer.

