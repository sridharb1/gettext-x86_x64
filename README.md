# gettext-x86_x64
Native Visual Studio project files to compile gettext (aka libintl) on Windows

# Background #
Compiling libintl on Windows requires a unix-like development
environment (like cygwin or mingw32). This allows you to compile
natively using Visual Studio

# Compiling #
This project provides native Visual Studio solution/project files that
can be used to compile gettext on Windows.

# Installation #

  * git clone [gettext, tested with v0.20.1](git://git.savannah.gnu.org/gettext.git) into a local folder
  * git clone [gettext-x86_x64](https://github.com/sridharb1/gettext-x86_x64)
  * Copy the contents of the gettext-x86_x64 folder into the build
    folder of gettext.
    
# Note #

To compile gettext, you need 

  * [libiconv, tested w/ v1.16](https://github.com/sridharb1/libiconv-x86_x64)
