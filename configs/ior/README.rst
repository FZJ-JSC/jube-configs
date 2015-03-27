IOR
~~~

Description
-----------
IOR - (InterleavedOrRandom) I/O benchmark

Configuration creator
---------------------
* Creator: Stephan Graf, JSC, Forschungszentrum Jülich GmbH
* Date: 05.12.2014

JUBE info
---------
* Main configuration: ior.xml
* Tested version: 2.0.4

Source
------
* Download: `https://github.com/chaos/ior <https://github.com/chaos/ior>`_
* Version: 3.0.1
* License: GPLv2
* Comment: Copy ``ior-3.0.1.tar.gz`` into the same directory of ior.xml and use tag ``bootstrap`` to use autotools. You can also
  run bootstrap procedure before *JUBE* execution and create a new tar file ``ior.tar.gz`` (containing pre created ``configure`` and all other related files).
  For the second case you do not need the bootstrap tag.

Included files
--------------
+---------------+-----------------------------------------+
| file name     | purpose                                 |
+===============+=========================================+
| ior.xml       | master XML file for the IOR run in JUBE |
+---------------+-----------------------------------------+
| ior_specs.xml | default specifications for the IOR run  |
|               | is used by the master XML file          |
+---------------+-----------------------------------------+
| ior_input.in  | file for the later IOR run              |
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

* Execute the ior/JUBE job: ``jube run ior.xml --tag <platform>``
     - Tag ``gpfs`` will enable GPFS support in IOR
