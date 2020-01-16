=================================
Pre-commit Hooks for cmake-format
=================================

This repository contains configuration to add `cmake-format`__ hooks to a git
project using `pre-commit`__.

.. __: https://pypi.org/project/cmake-format/
.. __: https://pre-commit.com/

-----
Usage
-----

To add ``cmake-format`` and ``cmake-lint`` to your pre-commit configuration,
add something like the following to your ``.pre-commit-config.yaml`` file:

.. code:: yaml

   repos:
     - repo: https://github.com/cheshirekow/cmake-format-precommit
       rev: v0.6.6
       hooks:
       - id: cmake-format
       - id: cmake-lint


----------------
Acknowledgements
----------------

Thanks to `@aharrison24`__ for prototyping configuration in this `issue`__ and
`this repository`__ and to `@asottile`__ for showing us how to create a
configuration that sources from pypi.org.

.. __: https://github.com/aharrison24
.. __: https://github.com/cheshirekow/cmake_format/pull/44
.. __: https://github.com/aharrison24/cmake-format-pre-commit.git
.. __: https://github.com/asottile
