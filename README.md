Easy and clean launch TFTN coin using ForkNote, the most advanced CryptoNote software supporting numerous networks.

### Overview

Forknote uses configuration files to describe the properties of a Cryptonote blockchain. To get started you must download the latest version of Forknote.

Connecting the daemon to a blockchain

To connect to the daemon to existing blockchain, just start forknoted with the corresponding configuration file.

$ ./TFTNd --config-file configs/imaginary_blockchain.conf New blockchains are created by creating new configuration files. Configuration files are created with our blockchain creation form. You can find more about the available configuration options in our documentation.

### Examples

To connect the daemon to the TFTN coin, start TFTNd with its corresponding configuration file:

$ ./TFTNd --config-file configs/TFTN.conf To connect to the TFTN blockchain

Starting simplewallet

Simplewallet uses the same configuration file as the daemon.

To start simplewallet:

$ ./TFTN_simplewallet --config-file configs/TFTN.conf 

Building TFTN

On Linux

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, and Boost 1.55 or later.

You may download them from:

http://gcc.gnu.org/
http://www.cmake.org/
http://www.boost.org/

Alternatively, it may be possible to install them using a package manager.
To build, change to a directory where this file is located, and run make. The resulting executables can be found in build/release/src.

Advanced options:

Parallel build: run make -j<number of threads> instead of make.
Debug build: run make build-debug.
Test suite: run make test-release to run tests in addition to building. Running make test-debug will do the same to the debug version.
Building with Clang: it may be possible to use Clang instead of GCC, but this may not work everywhere. To build, run export CC=clang CXX=clang++ before running make.

On Windows

Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, and Boost 1.55. You may download them from:

http://www.microsoft.com/
http://www.cmake.org/
http://www.boost.org/

To build, change to a directory where this file is located, and run theas commands:

mkdir build
cd build
cmake -G "Visual Studio 12 Win64" ..
And then do Build. Good luck!
