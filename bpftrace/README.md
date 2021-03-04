**use-ghc-filesystem.patch**

Use ghc filesystem(https://github.com/gulrak/filesystem) for compiling bpftrace in termux(Android device).
You need to copy 'ghc/filesystem.hpp' to '~/../usr/include'.

**build bpftrace**

*build and install 'bcc' first, then:*
```
$ export CC=clang
$ export CXX=clang++
$ git clone https://github.com/iovisor/bpftrace.git 
$ cd bpftrace
$ mkdir -p build && cd build
$ cmake .. -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=/data/data/com.termux/files/usr
$ make bpftrace -j4
$ ./src/bpftrace
```
