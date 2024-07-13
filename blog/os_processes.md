*This document is a handnote of the book: Operating System Concepts [by Silberschatz, Galvin and Gagne]*

## Processes

**1. Process:** A process is (an instance of) a program in execution. For example: A word-processing program being run by an individual user on a PC is a process. Similary, a social media app being run on a mobile device is a process.

A process is the unit of work in a system. A system consists of a collection of processes. Some of which are operating system processes and the rest of which are  user processes.

The status of the current activity of a process is represented by the value of the program counter and the contents of the processor’s registers.

> The memory layout of a process is typically divided into multiple sections. These sections include: 
**(i)** Text section: the executable code.  
**(i)** Data Section: global variables.  
**(i)** Heap section: memory that is dynamically allocated during program run
time.  
**(i)** Stack section: temporary data storage when invoking functions (such as
function parameters, return addresses, and local variables).

<img src="process_layout_memory.JPG" />


## Process State
---

The state of a process refers to the current acitivity of the process. As a process executes, it changes state. A process may be in one of the following states:

**(i) New:** The process is being created.  
**(i) Ready:** The process is waiting to be assigned to a processor.  
**(i) Running:** Instructions are being exectued.  
**(i) Waiting:** The process is waiting for some event to occur (such as an I/O completion or reception of a signal).  
**(ii) Terminated:** The process has finished execution.

<img src="process_state.JPG" />

**>** Only one process can be running on any processor core at any instant. Many processes may be ready and waiting.

## Process Control Block (PCB)
<hr />

> **Process Control Block (PCB):** *[Wikipedia]* Process Control Block is a data structure used by the operating system of a computer to store all the information about a process.  
It is also known as task control block.

Each process is represented in the operating system by a process control block (PCB). It contains many pieces of information associated with a specific process. They are,

**(i)** &nbsp;<u>Process state</u>: The state may be new, raedy, running, waiting, terminated, and so on.  
**(i)** &nbsp;<u>Program counter</u>: The program counter indicates the address of the next instruction to be executed for the process.

<!-- PCB, where is it used? what are its contents -->

---
---
---

> [**Contact**](https://tawk.to/chat/66893d23eaf3bd8d4d18d232/1i241dlbj) us to buy the full document. *It's only $1.50!*