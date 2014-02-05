lsd
===

list static dependencies

A tool that tries to emulate ldd but for statically linked binaries.  The process is to run the dblsd script first to build a database of static libraries on the system. Once the database is constructed the main lsd script is used to check a specified binary against the database.  It reports back which matches were hash matches, if it is not a hash match it does a basic measure to see how alike they are (differences in the bytes).
