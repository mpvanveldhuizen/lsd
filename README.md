List Static Dependencies
===
### About
A tool that tries to emulate [List Dynamic Dependencies](http://man7.org/linux/man-pages/man1/ldd.1.html) or `ldd` but for statically linked binaries.

### Setup Instructions
1. Run the `dblsd` script first with a name to give to the database to build a database of static libraries on the system.
  2. `dblsd [FILE NAME]`
3. Once the database is constructed the main `lsd` script is used, given a file to check a specified binary against a database. 
  3. `lsd [FILE NAME] [DATABASE]`

`lsd` reports back which matches were hash matches, if it is not a hash match it does a basic measure to see how alike they are (differences in the bytes).
