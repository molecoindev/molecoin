## Building molecoin

### On Ubuntu

Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, Boost 1.58, and Git.
Note: Building has only been confirmed to work on Ubuntu 16
To build on Ubuntu 16 run the following commands:
```
sudo apt-get update
sudo apt-get install build-essential cmake libboost-all-dev git
git clone https://github.com/molecoindev/molecoin.git
cd molecoin
make
```
you can also use ``make -j<number of threads>`` to specify the number of threads

### On Windows
Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, and Boost 1.55. You may download them from:

* http://www.microsoft.com/
* http://www.cmake.org/
* http://www.boost.org/

To build, change to a directory where this file is located, and run theas commands: 
```
mkdir build
cd build
cmake -G "Visual Studio 12 Win64" ..
```

And then do Build.
Good luck!
