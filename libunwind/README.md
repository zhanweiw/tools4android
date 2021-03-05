**Compile 'libunwind' lib in termux:**

```
$ git clone https://github.com/libunwind/libunwind.git
$ cd libunwind
$ mkdir -p build && cd build
$ ../autogen.sh
$ ../configure --prefix=/data/data/com.termux/files/usr
$ make
$ make install prefix=/data/data/com.termux/files/usr
```
