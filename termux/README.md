For compile bcc & bpftrace, make change in '~/../usr/include/':
usr\include\asm-generic\types.h
+ #define __user
+ #define __force

usr\include\linux\eventpoll.h
+ typedef unsigned __bitwise __poll_t;
