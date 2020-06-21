Ipopt is a solver for large scale nonlinear optimization problems (NLP) with non-linear contraints. 
The Java Native Interface (JNI) is a programming framework that allows Java code running in the Java Virtual Machine (JVM) 
to call and be called by native applications and libraries written in languages such as C and C++.
JIpopt requires Java 5 or higher.

This pre-compiled library jipopt.dll was compiled in Windows 10 64bits using MSYS2-64Bits, and depends on several files:
jipopt.dll 
         |- kernel32.dll  
         |- msvcrt.dll    
         |- libblas.dll 
         |- libgcc_s_seh-1.dll
         |- libgfortran-5.dll
         |- liblapack.dll
         |- libquadmath-0.dll
         |- libstdc++-6.dll
         |- libwinpthread-1.dll

To be able to run this example all these DLLs files MUST be in Windows PATH.

I recommend copying this directory "jni_dependency" to "C:\jni_dependency" and add this folder to Windows PATH.

Go to Control Panel-> System-> Advanced System Settings-> Advanced (tab)-> Environment Variables-> Double click on "Path"-> New-> Add "C:\jni_dependency"-> OK

After this restart Eclipse IDE and run HS071.java, it should work.

If you still have the error "java.lang.UnsatisfiedLinkError" review the previous steps, this error occurs when jipopt.dll does not find its dependencies.

Any question contact me: 

Rodrigo Eggea (rodrigo.eggea@gmail.com)
