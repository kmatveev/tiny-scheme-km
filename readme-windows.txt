Tiny scheme could be built with Visual Studio either via command-line nmake, or from IDE itself.
If building from command-line, start cmd with either vcvars32.bat or vcvars64.bat, then cd to tinyscheme dir, and run nmake.
If building from IDE, following is recommended:
  In build -> properties -> C/C++ -> preprocessor, define WIN32 and _CRT_SECURE_NO_WARNINGS and _CRT_NONSTDC_NO_DEPRECATE
  last two will get rid of annoying error messages
  To work around "unused variable" error, in build properties -> C/C++ -> general switch off SDL checks

Tiny scheme could be built with msys2/mingw64