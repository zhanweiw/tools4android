**For compile bcc & bpftrace, make change in '~/../usr/include/':**
```
/usr/include/asm-generic/types.h
+ #define __user
+ #define __force
```

```
usr/include/linux/eventpoll.h
+ typedef unsigned __bitwise __poll_t;
```

**For compile 'perf' from linux-5.12, make change in '~/../usr/include/'：**
```
/usr/include/linux/stddef.h
-#include <linux/compiler_types.h>
+#include <linux/compiler.h>
```

```
/usr/include/netinet/in.h
+typedef uint32_t in_addr_t;
```

**For coompile 'libunwind' for Android, make change in '~/../usr/include/':**
```
/usr/include/linux/elfcore.h
-typedef elf_fpxregset_t fpxregset_t;

+/*
 28 struct elf_siginfo {
 29   int si_signo;
 30   int si_code;
 31   int si_errno;
 32 };
+*/
```

**Run termux app with root permission:**
```
adb root
adb shell
# source termux.sh
```
