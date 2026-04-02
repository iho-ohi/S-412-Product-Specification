# WMO S-412 Marine Weather Warnings Product Specification

//image:https://github.com/metanorma/S-412-Product-Specification/actions/workflows/generate.yml/badge.svg["Build Status", link="https://github.com/metanorma/S-412-Product-Specification/actions/workflows/generate.yml"]

This document is available in its rendered forms here:

* https://iho-ohi.github.io/S-412-Product-Specification/[IHO S-412(HTML)]

Metanorma: https://github.com/iho-ohi/S-412-Product-Specification-Development/blob/main/Documents/PS/document.html[Product Specification]

## Purpose

This is the WMO repository for developing the next edition of
the S-412 Marine Weather Warnings Products.

WARNING: The contents of this repository are in draft form and are not necessarily in force yet.
Please refer to the final version published on the official
https://registry.iho.int[GI Registry] website.


## General

This repository contains the source files of S-412 standards, including:

* S-412 1.0.0
* S-412 x.x.x

These documents are encoded in the
https://www.metanorma.org/author/topics/document-format/[Metanorma AsciiDoc format].


## Structure

`sources/`::
source of the S-412 documents and models

`site/`::
(automatically generated, in the `gh-pages` branch) published document.


## Usage

This repository uses `metanorma` to run these processes.

Please refer to
https://www.metanorma.org/author/iho/authoring-guide/[Metanorma-IHO documentation]
for authoring guidance.


## Installing build tools

See the https://www.metanorma.org/install/[Metanorma install] page.


## Building the document

If you have installed the build tools locally, and wish to run the
locally-installed compilation tools, there is nothing further to set.

If you use a locally installed Metanorma, run:

[source,sh]
----
metanorma site generate
----

If you wish to avoid using local dependencies, use the docker
version by:

[source,sh]
----
docker run -v "$(pwd)":/metanorma -w /metanorma -it metanorma/mn metanorma site generate
----

## License

See link:LICENSE.adoc[LICENSE].
