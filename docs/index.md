---
author: Kumar Shaurya
updated: 2026-09-04
---

# M3: Kernel Module Loader (LKM)

A Linux-style dynamic module loading subsystem that parses relocatable kernel modules, resolves kernel symbols, and registers or unregisters them at runtime. This is what lets later subsystems such as the VFS and filesystems be developed and loaded independently of the process/scheduler track.

## Core Objectives
* Relocatable ELF (.ko-style) parsing
* Kernel symbol table and resolution
* Module register/init and cleanup API
* insmod / rmmod-style loading mechanism

## Architecture
Pending implementation details.
