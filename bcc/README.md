**build bcc**

```
$ export CC=clang
$ export CXX=clang++
$ git clone https://github.com/iovisor/bcc.git
$ cd bcc
$ mkdir -p build && cd build
$ cmake .. -DCMAKE_INSTALL_PREFIX=/data/data/com.termux/files/usr -DBCC_PROG_TAG_DIR=/data/local/tmp/bcc -DKERNEL_INCLUDE_DIRS=/data/local/tmp/headers/include/
$ make -j4
$ make install
```
