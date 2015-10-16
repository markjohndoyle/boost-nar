boost-nar
=========

The Boost C++ libraries in maven form for producing Nar artefacts for use with the  [nar-maven-plugin](https://github.com/maven-nar/nar-maven-plugin)

The libraries are available as separate dependencies as per a typical module layout. This means if required you can depend only upon the boost filesystem module, the necessary transitive depedencies will be automatically available.

Building
-----------------

Simply execute your deisred maven goal e.g. mvn install

*There are two properties specifing compiler and linker in the root pom. This is set to use g++ which is our default on Windows. You can override this on the command line as follows:*

`mvn install -Dcompiler-name=yourcompiler -Dlinker-name=yourlinker`

*or you can simply remove the entries in the pom and use the default for your AOL. See the nar documentation for more details.*


Things to note
-----------------

* iostreams does not use bzip TODO compiler flag or edited the code? We don't want to be changing boost.
* asio does not have the asio/impl/src.cpp

Module status
--------------
Modules are added as required or via contributions. Currently we have:

* asio
* bind
* concept
* config
* container
* core
* date-time
* detail
* exception
* filesystem
* function
* function_types
* functional
* fusion
* integer
* io
* iostreams
* iterator
* interprocess
* lexical-cast
* math
* move
* mpl
* numeric
* optional
* phoenix
* predef
* preprocessor
* proto
* range
* regex
* smart-ptr
* spirit
* system
* type-traits
* type_index
* typeof
* utility
* variant
