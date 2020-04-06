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
  * When you clone gettext, you might also clone a submodule called gnulib. This is not necessary. You can turn off the recursive flag while cloning.
  * git clone [gettext-x86_x64](https://github.com/sridharb1/gettext-x86_x64)
  * Copy the contents of the gettext-x86_x64 folder into the build
    folder of gettext.
  * This is based off of [karhl's gettext-msvc](https://github.com/kahrl/gettext-msvc)
  * There is a small step to generate plural.c/h from plural.y. This requires utilities like bison and sed. I have provided the generated plural.c/h. In case there are problems with this file, go back to generating this file from the canonical plural.y. Instructions can be found in Makefile.am in the same folder as plural.y

# Note #

To compile gettext, you need 

  * [libiconv, tested w/ v1.16](https://github.com/sridharb1/libiconv-x86_x64)
