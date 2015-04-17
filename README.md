boost-nar
=========

The Boost C++ libraries in maven form for producing Nar artefacts.

To install simply clone the repo and run:
  mvn install


The libraries are available as separate dependencies as per a typical module layout. This means if required you can depend only upon the boost filesystem module, the necessary transitive depedencies will be automatically available.

==========
JOHN MW

Added sections for the running of spirit and lex programs, 

iostreams does not use bzip

minor change to lexical-cast (converter_lexical_streams.hpp) to prevent error from running in visual studio environment

