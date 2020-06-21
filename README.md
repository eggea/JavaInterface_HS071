## JavaInterface jipopt.dll compiled in 64-bits for Windows with HS71 example

Ipopt is a solver for large scale nonlinear optimization problems (NLP) with non-linear contraints. 
The Java Native Interface (JNI) is a programming framework that allows Java code running in the Java Virtual Machine (JVM) 
to call and be called by native applications and libraries written in languages such as C and C++.
JIpopt requires Java 5 or higher.

The [Official Jipopt website](https://projects.coin-or.org/Ipopt/wiki/JavaInterface) provides pre-compiled DLL's with Ipopt+MUMPS for  Win32 platforms and for Ubuntu Linux i386. 

Due to the lack of this jipopt library compiled for Java Runtime 64-bits, I compiled and providing in this repository with the original sample code HS71 together with the 64-bit compiled jipopt.dll. 

This jipopt library was compiled by the source [Ipopt-3.12.13](https://www.coin-or.org/download/source/Ipopt/Ipopt-3.12.13.tgz) in Windows10 using [MSYS2-64bits](https://www.msys2.org/) and following the instructions [Installing Ipopt](https://coin-or.github.io/Ipopt/INSTALL.html) with some workarounds.

### Prerequisites
[Java JDK 64-bits for Windows](https://www.oracle.com/java/technologies/javase-jdk14-downloads.html) - Java SE Development Kit

[Eclipse IDE](https://www.eclipse.org/downloads/) - Eclipse IDE

### Installing

1) Clone this GIT Project to Eclipse 

2) Add the folder "jni_dependency" to Windows PATH variable (See [README.TXT](https://github.com/eggea/JavaInterface_HS071/blob/master/JavaInterface_HS071/jni_dependency/README.TXT))

3) Restart Eclipse

4) Run the java example "HS01.java"

## Authors

* **[Rodrigo Eggea](https://github.com/eggea)** 

