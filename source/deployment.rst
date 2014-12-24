
======================
Application Deployment
======================

:Page Status: Incomplete
:Last Reviewed: 2014-12-20


In this section, we'll focus on the solutions and tools people use to install
Python applications across many Python environments and servers.

Although this guide offers a :doc:`confident set of recommendation <current>`
for building and installing packages (into a single Python environment), for
deployment, there's much less consensus.

Below, we'll break down some of the variables and mention some specific
solutions that are commonly used.


.. contents:: Contents
   :local:


Variables
=========

Let's break down the ways that deployment solutions can vary.

1. Python Environment
---------------------

The type of Python environment that packages are installed into.

1.1 System Python
~~~~~~~~~~~~~~~~~

A "System Python" is a Python that is managed by the OS package manager.  For
example, most Linux distributions will manage and offer packages for some
version of Python2 and Python3.  These Pythons are "System" Pythons.

It's commonly frowned upon to deploy your own application into a "System"
Python due to the possibility of corrupting the OS or it's supporting tools.

1.2 Alternate Python
~~~~~~~~~~~~~~~~~~~~

"Alternate Python" here simply means non-"System", i.e. a Python that is not
managed by the OS package manager.

mention the tools

1.3 Virtual Environment
~~~~~~~~~~~~~~~~~~~~~~~

These are Python environments that are rendered by tools like :ref:`virtualenv` and
:ref:`venv`.

2. Package Format
-----------------

The package format that's used for installation.

2.1 Native OS Packaging
~~~~~~~~~~~~~~~~~~~~~~~

For example, "rpm"s or "deb"s on Linux systems.

2.2 PyPI Packaging
~~~~~~~~~~~~~~~~~~

Packages that are compatible with the Python Package Index, like sdist and wheel.


2.3 Conda
~~~~~~~~~


2.3 Custom Bundles
~~~~~~~~~~~~~~~~~~

3. Build Time
-------------

3.1 Prebuilt
~~~~~~~~~~~~

3.2 Built during install
~~~~~~~~~~~~~~~~~~~~~~~~


4. Release Artifact
-------------------

Package
~~~~~~~

Virtual Machine
~~~~~~~~~~~~~~~

Linux "Container"
~~~~~~~~~~~~~~~~~


Solutions
=========

Fabric/Invoke Tasks
-------------------

CM Systems
----------

Puppet
~~~~~~

Chef
~~~~

Saltstack
~~~~~~~~~

Ansible
~~~~~~~

OS Packaging
------------

Package per App
~~~~~~~~~~~~~~~

Package per Project
~~~~~~~~~~~~~~~~~~~

PEX
---
