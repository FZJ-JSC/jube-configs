HPL
~~~

Description
-----------
HPL - High-Performance Linpack Benchmark

Configuration creator
---------------------
* Creator: Stephan Graf, JSC, Forschungszentrum Jülich GmbH
* Date: 05.12.2014

JUBE info
---------
* Main configuration: hpl.xml
* Tested version: 2.0.7

Source
------
* Download: `http://www.netlib.org/benchmark/hpl/ <http://www.netlib.org/benchmark/hpl>`_
* Version: 2.1
* License: `http://www.netlib.org/benchmark/hpl/copyright.html <http://www.netlib.org/benchmark/hpl/copyright.html>`_
* Comment: Copy ``hpl-2.1.tar.gz`` into the same directory of hpl.xml

Included files
--------------
+---------------+-----------------------------------------+
| file name     | purpose                                 |
+===============+=========================================+
| hpl.xml       | master XML file for the HPL run in JUBE |
+---------------+-----------------------------------------+
| hpl_specs.xml | default specifications for the HPL run  |
|               | is used by the master XML file          |
+---------------+-----------------------------------------+
| HPL.dat.in    | file for the later HPL run              |
+---------------+-----------------------------------------+
| Makefile.in   | Makefile template                       |
+---------------+-----------------------------------------+

Comment
-------
* Preparation:
     - Platform definition available?
         - Predefined platforms are stored in ``<JUBE-INST-PATH>/platform/``
         - On 'unknown' systems this definition must be created first
     - Customize ior parameters to your demands
         - !!!only the master XML file should be modified!!!
         - look in the 'specs' file for the defaults
