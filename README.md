## Building molecoin

### On Ubuntu
Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, Boost 1.58, and Git.
<br>
Note: Building has only been confirmed to work on Ubuntu 16
<br>
To build on Ubuntu 16, open the terminal and run the following commands:
```
sudo apt-get update
sudo apt-get install build-essential cmake libboost-all-dev git
git clone https://github.com/molecoindev/molecoin.git
cd molecoin
make
```
you can also use ``make -j<number of threads>`` to specify the number of threads

### On Windows
Dependencies: MSVC 2013, CMake 2.8.6 or later, Boost 1.58, Python 3.10.1 or later, and Git. You may download these from:
* https://docs.microsoft.com/en-us/visualstudio/releasenotes/vs2013-update5-vs#download-visual-studio-community-2013
* https://cmake.org/download/
* https://sourceforge.net/projects/boost/files/boost-binaries/1.58.0/boost_1_58_0-msvc-12.0-64.exe/download
* https://www.python.org/downloads/
* https://git-scm.com/downloads

To build, open the command prompt and run the following commands:
```
git clone https://github.com/molecoindev/molecoin.git
mkdir molecoin\build
cd molecoin\build
cmake -G "Visual Studio 12 Win64" ..
```
Once the configuring is done, go to the build files in file explorer (should be something like ``C:\Users\(your username)\molecoin\build).``
<br>
Find and open the file named cryptonote.sln in Visual Studio 2013.
<br>
Navigate to the build tab inside Visual Studio and click Build Solution from the dropdown menu.
<br>
The finished daemons will be located in molecoin\build\src\Debug
