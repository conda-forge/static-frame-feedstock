About static-frame
==================

Home: https://github.com/InvestmentSystems/static-frame

Package license: MIT

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/static-frame-feedstock/blob/master/LICENSE.txt)

Summary: Immutable structures for one- and two-dimensional calculations with labelled axis

Development: https://github.com/InvestmentSystems/static-frame

Documentation: https://static-frame.readthedocs.io

A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.

While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy types; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.

A wide variety of table storage and representation formats are supported, including input from and output to CSV, TSV, JSON, MessagePack, Excel XLSX, SQLite, HDF5, NumPy, Pandas, Arrow, and Parquet; additionally, output to xarray, HTML, RST, Markdown, and LaTeX is supported, as well as HTML representations in Jupyter notebooks.

StaticFrame features a family of multi-table containers: the Bus is lazily loaded container of tables, the Batch is a deferred processor of tables, and the Quilt is a virtual concatenation of tables. All permit operating on large collections of tables with minimal memory overhead, as well as writing too and reading from zipped bundles of pickles, Parquet, or delimited files, as well as XLSX workbooks, SQLite, and HDF5.


Current build status
====================


<table><tr><td>All platforms:</td>
    <td>
      <a href="https://dev.azure.com/conda-forge/feedstock-builds/_build/latest?definitionId=6190&branchName=master">
        <img src="https://dev.azure.com/conda-forge/feedstock-builds/_apis/build/status/static-frame-feedstock?branchName=master">
      </a>
    </td>
  </tr>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-static--frame-green.svg)](https://anaconda.org/conda-forge/static-frame) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/static-frame.svg)](https://anaconda.org/conda-forge/static-frame) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/static-frame.svg)](https://anaconda.org/conda-forge/static-frame) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/static-frame.svg)](https://anaconda.org/conda-forge/static-frame) |

Installing static-frame
=======================

Installing `static-frame` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
conda config --set channel_priority strict
```

Once the `conda-forge` channel has been enabled, `static-frame` can be installed with:

```
conda install static-frame
```

It is possible to list all of the versions of `static-frame` available on your platform with:

```
conda search static-frame --channel conda-forge
```


About conda-forge
=================

[![Powered by
NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/)
and [TravisCI](https://travis-ci.com/) it is possible to build and upload installable
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


Updating static-frame-feedstock
===============================

If you would like to improve the static-frame recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/static-frame-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@brandtbucher](https://github.com/brandtbucher/)
* [@flexatone](https://github.com/flexatone/)

