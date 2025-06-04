# xv6-assignments

![Final Grade](https://img.shields.io/badge/grade-100-brightgreen.svg)
![Semester](https://img.shields.io/badge/semester-2024A-blue.svg)
![Course](https://img.shields.io/badge/course-operating_systems-lightgrey.svg)

📘 Solutions for assignments based on the xv6 operating system — part of the *Operating Systems* course at the Open University of Israel.

## Overview

This repository contains my solutions to Maman 11 and Maman 12 — two programming assignments focusing on kernel development, system calls, process management, and container-like isolation in the xv6 educational operating system.

The assignments were completed as part of course **20502 – Operating Systems**.

### 🔍 Topics Covered

- Adding custom system calls to xv6  
- Printing process trees and process information from the kernel  
- Working with PID namespaces and basic container isolation  
- Modifying the xv6 kernel and user-level system interfaces  
- Compilation with `make` and debugging with QEMU  

## Structure

```text
xv6-assignments/
├── maman11/
│   ├── ps.c
│   ├── syscall.c
│   ├── sysproc.c
│   └── ...
├── maman12/
│   ├── updated-syscall-files/
│   │   ├── ...
│   └── namespace-related-code/
│       ├── ...
└── README.md
```


## How to Build & Run

To build and run the xv6 operating system with the included modifications:

```bash
make clean
make qemu

For testing:
./runtests.exp my.log
echo $?
# Should return 0 on success
```
Notes
These solutions follow the guidelines and limitations defined in the course, including restrictions on modifying certain files (e.g., syscall.h), and follow conventions for system call naming and kernel structure.

Disclaimer
This code is provided for learning purposes only. Please do not copy solutions directly — understanding and implementing the logic yourself is key to mastering systems programming.
