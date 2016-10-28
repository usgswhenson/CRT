                      CRT - Version: 1.2
                      Cascade Routing Tool


NOTE: Any use of trade, product or firm names is for descriptive purposes only and
does not imply endorsement by the U.S. Government.

CRT Version 1.2 is packaged for personal computers using one of the Microsoft 
Windows operating systems. An executable file compiled for 32-bit and 64-bit are
provided, as well as the source code. 

The executables were compiled on a personal computer with the Intel(R) Core(TM)
2Duo CPU T9500 chipset, running the Microsoft Windows 7 operating system,using the
Microsoft Visual Studio 2010 Version 10.0.40219.1 development environment and the
Intel(R) Parallel Studio XE 2015 Fortran Compiler.

The source code is provided to aid users in compilation on other computers.
However, no support is provided for compilation.

IMPORTANT: Users should review the file Summary_CRT.txt for a description of, and
references for, this software. Users should also review the file release.txt, 
which describes changes that have been introduced into CRT with each official 
release; these changes may substantially affect users.

Instructions for installation, execution, and testing of this version of CRT are
provided below.



                            TABLE OF CONTENTS

                         A. DISTRIBUTION FILE
                         B. INSTALLING
                         C. EXECUTING THE SOFTWARE
                         D. TESTING
                         E. COMPILING


A. DISTRIBUTION FILE

The following distribution file is for use on personal computers:

          CRT_1.2.zip

The distribution file contains:

          Executable and source code for CRT
          CRT documentation
          Cascade Routing Visualization ArcGIS Toolbox (CRV)
          Two CRT example applications

The distribution file is a zip file for use on personal computers running Windows
operating systems. The distribution file creates numerous individual files 
contained in the following directory structure:

   |
   |--CRT_1.2
   |    |--APPLICATIONS  ; Input and output files for two CRT sample 
                           applications    
        |--BIN           ; Compiled CRT executables for personal computers
        |--CRV           ; ArcGIS Toolbox and CRV installation instructions 
        |--DOC           ; CRT documentation
        |--SOURCE        ; Source code for CRT


Included in directory CRT_1.2\DOC is the CRT documentation report, which is a 
Portable Document Format (PDF) file. The PDF file is readable and printable on 
various computer platforms using Acrobat Reader from Adobe. The Acrobat Reader is
freely available from the following World Wide Web site: http://www.adobe.com/


B. INSTALLING

To make the executable version of CRT accessible from any directory, the directory 
containing the executable (CRT_1.2\BIN) should be included in the PATH environment 
variable. Also, if a prior release of CRT is installed on your system, the 
directory containing the executables for the prior release should be removed from 
the PATH environment variable.

As an alternative, the executable files in the CRT_1.2\BIN directory can be copied 
into a directory already included in the PATH environment variable. The sample 
problems provided with the release (described below) have sample batch files that
provide an alternative, additional approach for accessing the executable files.


C. EXECUTING THE SOFTWARE

CRT has 32-bit and 64-bit (CRT_1.2.exe and CRT_1.2x64.exe) executables in
the CRT_1.2\BIN directory. CRT can be executed by placing a CRT executable in the
directory containing the input files and double clicking the file. Alternatively,
the Windows batch file located in each application subdirectory (crt.bat) can be
used to run the 32-bit version of CRT. CRV uses the 32-bit version of CRT to take
advantage of the 64-bit CRT executable, run CRT outside of CRV to generate a 
vis.txt file, then use CRV in visualization-only mode. CRT will provide output to
the terminal window and to the outputstat.txt output file.

The arrays in CRT are dynamically allocated, so models are not limited by the 
size of input data. However, it is best to have at least 4 MB of random-access 
memory (RAM) for CRT execution and more RAM for large models. If there is less 
available RAM than the model requires, which depends on the size of the 
application, the program will use virtual memory; however, this can slow execution
significantly. If there is insufficient memory to run the model, then CRT will not
initiate the beginning of the simulation; however, the Windows Command-Prompt 
window may continue to indicate that CRT is executing. For this circumstance, 
the program must be terminated manually using the Windows Task Manager 
application.

CRT input and output files are all ASCII format and can be read or edited using 
any standard text editing software


D. TESTING

Two sample applications with CRT data sets are provided to verify that CRT 
is correctly installed and running on the system.  The sample applications may 
also be looked at as examples of how to use the program. A description of the file
structure for the example problem and of directions for running the example 
problem are described in the 'Readme.sagehen.txt' file located in directory 
CRT_1.2\APPLICATIONS\APPLICATION 1 SAGEHEN and the Readme.LWRB.txt file located in
directory CRT_1.2\APPLICATIONS\APPLICATION 2 LWRB. (Note, users may want to
download the supplemental GIS data for the two test problems separately from the 
CRT webpage).


E. COMPILING

The executable files provided in CRT_1.2\BIN were created using the Intel
Visual Fortran compiler. Although executable versions of the program are provided, 
the source code also is provided in the CRT_1.2\SOURCE directory so that CRT can 
be recompiled if necessary.  However, the USGS cannot provide assistance to those
compiling CRT. In general, the requirements are a Fortran compiler and the 
knowledge to use the compiler. 

