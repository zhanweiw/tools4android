**Compile 'perf' from linux-5.12 in termux:**

1. Add patch 'compile-perf-5.12.patch'.
2. pkg install libcap zlib-static slang zstd
3. Compile 'libunwind' & 
4. Compile 'binutils' for getting 'libiberty'

```
git clone git://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git
cd ~/source/linux-master/tools/perf
make WERROR=0 NO_SDT=1 NO_JVMTI=1
```
