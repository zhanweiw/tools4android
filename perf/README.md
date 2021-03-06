**Compile 'perf' from linux-5.12 in termux:**

1. pkg install libcap zlib-static slang zstd
2. Compile 'libunwind'.
3. Compile 'binutils' for getting 'libiberty'.
4. Compile 'numactl' for getting 'libnuma'.
5. Compile 'perf'.
```
git clone git://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git
cd ~/source/linux-master/tools/perf
Add patch 'compile-perf-5.12.patch'.
make WERROR=0 NO_SDT=1 NO_JVMTI=1 NO_AIO
```
