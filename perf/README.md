patch for compile 'perf' from linux-5.12 in termux.

```
git clone git://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git
cd ~/source/linux-master/tools/perf
make NO_LIBPYTHON=1 NO_LIBPERL=1 NO_LIBBABELTRACE=1 WERROR=0
```
