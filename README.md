** Originally from https://github.com/zicanl/NemoLib-Java-V2


nemolib
=======

Description
-----------
The nemolib library includes tools specifically designed for executing the the detection of network motifs. Classes have also been designed with parallelization in mind.
It includes network-centric and motif-centric approach. In network-cenric approach, both of explicit and direct methods are implemented for statistical analysis.

DOI
---
https://zenodo.org/badge/173347013.svg

https://zenodo.org/badge/latestdoi/173347013

Installation and Use in Linux
--------------------
**Prerequisites 
* A Linux operating environment.
* JDK version 8 or higher
* [Maven](https://maven.apache.org/) version 3.0 or higher
Use the `mvn package` command from the root directory to generate a jar file
in the `target` subdirectory containing the nemolib library. Any classes 
which implement nemolib should use the statement `import edu.uwb.nemolib;`.

// added 3/5/2019
git clone https://github.com/Kimw6/NemoLib-Java.git

cd nemolib

mvn package

Installation and Use in Windows
--------------------
* Prerequisites: Netbeans IDE and jdk 8.x version (jdk 9.x not work)
* Download and install Cygwin (follow the link to learn how to install gcc and g++)
http://preshing.com/20141108/how-to-install-the-latest-gcc-on-windows/
* Systems->advanced->Environment Variables
 From the path variable, add C:\Cygwin64\bin (for 64 bit) or (3)	C:\cygwin\bin (for 32 bit)
 
* NemoLib install
  Download NemoLib as zip file.
  Open the project in the NetBeans, build the library.
  With default setting, the library is, nemolib-master/target/ nemolib-0.1-SNAPSHOT.jar
  For external library, use dependency to add it (see pom.xml for details)

Example Program (testing the library)
---------------
The example java main file can be also found at 
NemoLib-Java/src/main/java/edu/uwb/nemolib_examples/network_motif_detector/


Documentation
-------------
JavaDocs are auto-generated when Maven creates the project.


Future Project Ideas
--------------------
* Parallelize random graph analysis (embarassingly parallel).
* Complete parallelization using MPI.
* * Implement the nauty algorithm in Java and include it as a dependency in nemolib. 
* Research other graph/network parallelziation libraries and implement NemoProfile to compare.
* Write unit tests.



