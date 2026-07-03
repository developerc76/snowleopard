# snowleopard

**SYSTEMS PROGRAMMING WORK IS HERE !!**

### Barebones 32-bit x86 Kernel:

**Description:**
* A simple OS kernel written in mostly C and Assembly. This should be able to load itself on x86 machines in 32-bit. 
* Compiled using GCC Cross-Compiler and tested on QEMU. 
* This is from the OSDev Wiki Barebones Tutorial on the Hello World x86 Kernel. 

**Install and Run:**
* Use QEMU (qemu-system-i386) and GCC (i686-elf-gcc) to compile it and run it
```
$ i686-elf-gcc -T linker.ld -o myos.bin -ffreestanding -O2 -nostdlib boot.o kernel.o -lgcc
$ qemu-system-i386 -kernel myos.bin
```

---

### Memory Allocators in C

(Now Moved from [small-projects](https://github.com/jasr4j/small-projects/))

**Types of Allocators:**
* Linear - Can only reset, but is very lightweight and fast
* Stack - Last In First Out Memory Allocator with a few additions
* Heap - Dynamic Memory Allocation (with a static maximum amount of memory)

**Install and Run:**
* Prerequisites: GCC (s**upport for at least C11), a UNIX-like (Linux, BSD, OS X) or DOS-like (Windows) OS.
* Install locally using git: 
```
$ git clone https://github.com/jasr4j/snowleopard.git
$ cd memory-allocators
$ gcc <filename>.c -o <executable name>
$ ./<executable name>
```