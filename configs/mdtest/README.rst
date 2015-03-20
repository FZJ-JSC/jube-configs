mdtest
~~~~~~

Description
-----------
Metadata test benchmark

Configuration creator
---------------------
* Creator: Stephan Graf, JSC, Forschungszentrum Jülich GmbH
* Date: 05.12.2014

JUBE info
---------
* Main configuration: mdtest.xml
* Tested version: 2.0.4

Source
------
* Download: `http://sourceforge.net/projects/mdtest/ <http://sourceforge.net/projects/mdtest/>`_
* Version: 1.9.3
* License: GPLv2
* Comment: Copy ``mdtest-1.9.3.tgz`` into the same directory of mdtest.xml

Comment
-------
* Preparation:

  1. Platform definition available?

     - Predefined platforms are stored in ``<JUBE-INST-PATH>/platform/``
     - On 'unknown' systems this definition must be created first

  2. Customize mdtest parameters to your demands

     - !!!only the master XML file should be modified!!!
     - look in the 'specs' file for the defaults

* Execute the mdtest/JUBE job: ``jube run mdtest-jube-master.xml --tag <platform>``
