# ExpOS Implementation

**Author:** Ruturaj Malavade  
**Project Reference:** [ExpOS Official Roadmap](https://exposnitc.github.io/index.html)

---

## 📘 Overview

This repository documents my implementation of the **Experimental Operating System (ExpOS)** project developed by NIT Calicut.  
The project walks through building an educational operating system from the ground up, implementing core modules such as process management, memory allocation, system calls, and interrupt handling.

**Progress:** Completed up to **Stage 27** of the official roadmap.  
**Pending:** Stage 28 (Device Driver Interface).

## 🧠 Project Structure

- **expl/samples/** — EXPL programs used to test the XSM environment and system calls.  
- **spl/spl_progs/** — SPL source files implementing OS modules such as process creation, scheduling, paging, and interrupts.  
- **spl/spl_progs/testing/** — Test and debugging SPL routines for validating system modules.  
- **screenshots/** — Captures of successful program execution and validation tests.  

---

## ⚙️ How to Run

### 1. Initialize the Disk Image  

Go to the `xfs-interface` folder and start the interface:  

```
./xfs-interface
```

Then enter the following commands:  

```
fdisk
run runfile.txt
exit
```

---

### 2. Start the XSM Simulator  

Navigate to the `xsm` directory and start the simulator:  

```
./xsm
```

---

### 3. Log In and Execute Programs  

```
username: root
password: root
```

After logging in, run available test programs,  
or shut down with:  

```
Shutdown
```

---

## 🧩 Sample Test Programs

The output of several test runs is available in the `screenshots/` directory.

init_odd.xsm — prints odd numbers from 200–300
even.xsm — prints even numbers from 100–200
gcd.xsm — takes two numbers as input and returns their GCD

---

## 🧱 What This Project Shows

This implementation demonstrates the step-by-step construction of a working educational operating system on the **XSM simulator** using the **ExpOS** framework. It covers:

- Boot and interrupt handling
- Process creation and scheduling
- Memory allocation and paging
- System calls and context switching
- Basic file system interaction and exception handling

The system successfully runs user-level EXPL programs on top of the custom kernel, reflecting a hands-on understanding of OS internals.
