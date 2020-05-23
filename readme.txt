./configure --prefix=/usr/local/qemu_debug --target-list=i386-softmmu,i386-linux-user --disable-kvm

./test
nasm a.asm -o test.bin

1, config-host.h:14:22: warning: missing terminating " character [enabled by default]  #define QEMU_VERSION "0.10.6"

2, vl.c:1575: undefined reference to `timer_gettime'
  Makefile.target:30  -lrt
