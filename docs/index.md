---
author: Kumar Shaurya
updated: 2026-09-04
---

# M3: Kernel Module Loader (LKM)

A Linux-style dynamic module loading subsystem that parses relocatable kernel modules, resolves kernel symbols, and registers or unregisters them at runtime. This is what lets later subsystems such as the VFS and filesystems be developed and loaded independently of the process/scheduler track.

## Core objectives

- Relocatable ELF (.ko-style) parsing
- Kernel symbol table and resolution
- Module register/init and cleanup API
- insmod / rmmod-style loading mechanism

## Architecture

Pending implementation details.

## References

- [OSDev Wiki — ELF](https://wiki.osdev.org/ELF)
- [Linux kernel source — kernel/module/main.c](https://github.com/torvalds/linux/blob/master/kernel/module/main.c)
- [Linux kernel source — kernel/module/kallsyms.c](https://github.com/torvalds/linux/blob/master/kernel/module/kallsyms.c)
- [Linux kernel source — include/linux/module.h](https://github.com/torvalds/linux/blob/master/include/linux/module.h)
- [Linux From Scratch](https://www.linuxfromscratch.org/lfs/view/stable/)

This module is explicitly modeled on Linux's own LKM subsystem, so the kernel source itself is the primary reference — read kernel/module/ before anything else. LFS is included for general context only; it doesn't cover this.
