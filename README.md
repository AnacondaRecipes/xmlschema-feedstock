About xmlschema
===============

Home: https://github.com/brunato/xmlschema

Package license: MIT

Feedstock license: BSD 3-Clause

Summary: An XML Schema validator and decoder

This is an implementation of XML Schema for Python (supports versions 2.7
and Python 3.3+).

This library arises from the needs of a solid Python layer for processing
XML Schema based files for MaX (Materials design at the Exascale) European
project. A significant problem is the encoding and the decoding of the XML
data files produced by different simulation software. Another important
requirement is the XML data validation, in order to put the produced data
under control. The lack of a suitable alternative for Python in the
schema-based decoding of XML data has led to build this library. Obviously
this library can be useful for other cases related to XML Schema based
processing, not only for the original scope.


Current build status
====================

All platforms:
[![noarch](https://img.shields.io/circleci/project/github/conda-forge/xmlschema-feedstock/master.svg?label=noarch)](https://circleci.com/gh/conda-forge/xmlschema-feedstock)

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-xmlschema-green.svg)](https://anaconda.org/conda-forge/xmlschema) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/xmlschema.svg)](https://anaconda.org/conda-forge/xmlschema) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/xmlschema.svg)](https://anaconda.org/conda-forge/xmlschema) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/xmlschema.svg)](https://anaconda.org/conda-forge/xmlschema) |

Installing xmlschema
====================

Installing `xmlschema` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
```

Once the `conda-forge` channel has been enabled, `xmlschema` can be installed with:

```
conda install xmlschema
```

It is possible to list all of the versions of `xmlschema` available on your platform with:

```
conda search xmlschema --channel conda-forge
```


About conda-forge
=================

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/)
and [TravisCI](https://travis-ci.org/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](https://anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating xmlschema-feedstock
============================

If you would like to improve the xmlschema recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/xmlschema-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string)
   back to 0.
