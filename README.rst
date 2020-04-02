========
Overview
========

.. start-badges

.. list-table::
    :stub-columns: 1

    * - docs
      - |docs|
    * - tests
      - | |travis| |appveyor| |requires|
        | |codecov|
    * - package
      - | |version| |wheel| |supported-versions| |supported-implementations|
        | |commits-since|
.. |docs| image:: https://readthedocs.org/projects/oemof/badge/?style=flat
    :target: https://readthedocs.org/projects/oemof
    :alt: Documentation Status

.. |travis| image:: https://api.travis-ci.org/oemof/oemof.svg?branch=master
    :alt: Travis-CI Build Status
    :target: https://travis-ci.org/oemof/oemof

.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/oemof/oemof?branch=master&svg=true
    :alt: AppVeyor Build Status
    :target: https://ci.appveyor.com/project/oemof/oemof

.. |requires| image:: https://requires.io/github/oemof/oemof/requirements.svg?branch=master
    :alt: Requirements Status
    :target: https://requires.io/github/oemof/oemof/requirements/?branch=master

.. |codecov| image:: https://codecov.io/gh/oemof/oemof/branch/master/graphs/badge.svg?branch=master
    :alt: Coverage Status
    :target: https://codecov.io/github/oemof/oemof

.. |version| image:: https://img.shields.io/pypi/v/oemof.svg
    :alt: PyPI Package latest release
    :target: https://pypi.org/project/oemof

.. |wheel| image:: https://img.shields.io/pypi/wheel/oemof.svg
    :alt: PyPI Wheel
    :target: https://pypi.org/project/oemof

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/oemof.svg
    :alt: Supported versions
    :target: https://pypi.org/project/oemof

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/oemof.svg
    :alt: Supported implementations
    :target: https://pypi.org/project/oemof

.. |commits-since| image:: https://img.shields.io/github/commits-since/oemof/oemof/v0.4.0.beta0.svg
    :alt: Commits since latest release
    :target: https://github.com/oemof/oemof/compare/v0.4.0.beta0...master



.. end-badges

Open Energy Modelling Framework - Python toolbox for energy system modelling and optimisation.

The omeof project aims to be a loose organisational frame for tools in the wide field of (energy) system modelling.
Every project is managed by their own developer team but we share some developer and design rules to make it easier to understand each others tools.

All projects are in different states and some even may not have a stable release but all projects are open to join.
We do not belong to a specific institution and everybody is free to join the developer teams and will have the same rights.
There is no higher decission level.

This repository is also used to organise everything for the oemof community.

- Webconference dates
- Real life meetings
- Website and Mailinglist
- General communication


**Content**

.. contents::
    :depth: 3
    :local:
    :backlinks: top

Projects with stable releases
=============================

* `oemof-solph <https://github.com/oemof/oemof-solph>`_
   A model generator for energy system modelling and optimisation (LP/MILP).

* `oemof-thermal <https://github.com/oemof/oemof-thermal>`_
   Coming soon...

* `cydets <https://github.com/oemof/cydets>`_
   Cycle Detection in Time Series (CyDeTS). An algorithm to detect cycles in times series along with their respective depth-of-cycle (DoC) and duration.

* `demandlib <https://github.com/oemof/demandlib>`_
   The `demandlib <https://github.com/oemof/demandlib>`_ library can be used to create load profiles for elctricity and heat knowing the annual demand. See the `documentation of the demandlib <http://demandlib.readthedocs.io/en/latest/>`_ for examples and a full description of the library.

* `feedinlib <https://github.com/oemof/feedinlib>`_
   The `feedinlib <https://github.com/oemof/feedinlib>`_ library serves as an interface between Open Data weather data and libraries to calculate feedin timeseries for fluctuating renewable energy sources.

* `TESPy <https://github.com/oemof/tespy>`_
   Thermal Engineering Systems in Python (TESPy). This package provides a powerful simulation toolkit for thermal engineering plants such as power plants, district heating systems or heat pumps.

* `windpowerlib <https://github.com/wind-python/windpowerlib>`_
   The windpowerlib is a library that provides a set of functions and classes
   to calculate the power output of wind turbines. It was originally part of
   the feedinlib (windpower and photovoltaic) but was taken out to build up
   a community concentrating on wind power models.


Projects in an early state
==========================

* `DHNx <https://github.com/oemof/dhnx>`_
   District heating system optimisation and simulation models



All project libraries are free software licenced under the MIT license.



Installation
============

To install the `oemof.solph` package (previously just `oemof`), please use

::

    pip install https://github.com/oemof/oemof-solph/archive/master.zip"


Documentation
=============


https://oemof.readthedocs.io/


Development
===========

To run the all tests run::

    tox

Note, to combine the coverage data from all the tox environments run:

.. list-table::
    :widths: 10 90
    :stub-columns: 1

    - - Windows
      - ::

            set PYTEST_ADDOPTS=--cov-append
            tox

    - - Other
      - ::

            PYTEST_ADDOPTS=--cov-append tox