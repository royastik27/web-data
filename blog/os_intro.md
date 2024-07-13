*This document is a handnote of the book: Operating System Concepts [by Silberschatz, Galvin and Gagne]*

## Operating System
---

**Operating System:** An operating system is a program that manages the computer hardware and provides a basis for application programs acting as an intermediary between the computer user and the computer hardware.

There is a wide variety of operating systems developed for accomplishing the tasks:  
**(i)** Mainframe operation systems are designed primarily to optimize utilization of hardware.  
**(ii)** Personal computer (PC) operating systems support complex games, business applications and everything in between.  
**(iii)** Operating systems for handheld computers are designed to provide an environment in which a user can easily interface with the computer to execute programs.  

Thus some operating systems are designed to be efficient, others to be convenient, and others some combination of two.

We can view a computer system as consisting of ~~hardware~~, ~~software~~ and ~~data~~. The operating system provides the means for proper use of these resources in the opreating of the computer system.  
An Operating system is similar to a government. A government performs no useful function by itself, but simply provides an environment within which other programs can do useful work.


## OS role w.r.t differnt views
---

**User view:** The user view of the computer varies according to the interface being used. For example:

**(i)** Most computer users use ~~personal computers~~. In this case, the operating system is designed mostly for the ease of use, with some attention paid to performance, and none paid to resource utilization (how various hardware and sofware resources are shared).

**(ii)** In other cases, users sit at terminals connected to a ~~mainframe~~ or a ~~minicomputer~~. These users share resources and may exchange information. The operating system in such cases ~~is designed to maximize resource utilization~~.

**(iii)** In still other cases, users sit ~~workstations~~ connected to networks of other ~~workstations~~ and ~~servers~~. These users have dedicated resources at their disposal, but they also share resources such as networking and servers. The operating system in such cases ~~is designed to compromise between individual usabilty and resource utilization~~.

**(iv)** Recently, many varieties of handheld computers have come into fashion. Their operating systems ~~are designed mostly for individual usabilty, but performance per unit of battery life is important as well~~.

**(v)** Some computers have little or no user view. For example: embedded computers in home devices and automobiles. Their operating systems ~~are designed basically to run without user intervention~~.

**System view:** From the computer's point of view, the OS is the program most intimately involved with the hardware. A computer system has many resources that may be required to solve a problem: ~~CPU time~~, ~~memory space~~, ~~file-storage space~~, ~~I/O devices~~, and so on. The OS acts as the manager of these resources. In this context, we can view operating system as a ~~resource allocator~~.

Again, an operating system manages the execution of user programs to prevent errors and improper use of the computer. In this context, we can view operation system as a ~~control program~~.

> The fundamental goal of computer system is to execute user programs and to make solving user problems easier.

> A more common definition, and the one that we usually follow, is that:  
~~The operating system~~ is the one program running at all times on the computer - usually called the kernel.  
Along with the kernel, there are two other types of programs:  
(i) ~~System programs~~, which are associated with the OS but are not part of the kernel.  
(ii) ~~Application programs~~, Which include all programs not associated with the operation of the system.

> **Minicomputer:** *[AI Generated]* A minicomputer is larger and more powerful than a personal computer. Minicomputers are used by small businesses or departments within a company for tasks that require more computing power and can support multiple users simultaneously. Personal computers (PCs) are designed for individual use, typically for tasks like web browsing, word processing, and gaming. Minicomputers are less common today as PCs have become more powerful.  
**Control Program:** A control program manages the execution of user programs to prevent errors and improper use of the computer.

*Interesting fact: In 1998, th e US department of Justice filed suit against Microsoft, in essence claiming that Microsoft included too much functionality in its OS and thus preveneted application vendors from competing (for example, a web browser was an integral part of the operating systems)*

## Resource Management
---

An operating system is a resource manager. The resources that an operating system must manage are ~~CPU~~, ~~memory space~~, ~~file-storage space~~ and ~~I/O devices~~.

**1. Process management:** A process is an instance of a program in execution. For example: A word-processing program being run by an individual user on a PC is a process. Similary, a social media app being run on a mobile device is a process.

A process is the unit of work in a system. A system consists of a collection of processes. Some of which are operating system processes and the rest of which are  user processes.

The operating system is responsible for the following activities in connection with process management:

**(i)** Creating and deleting both user and system processes.  
**(ii)** Suspending and resuming processes.  
**(iii)** Scheduling processes and threads on the CPUs.  
**(iv)** Providing mechanisms for process communication.  
**(v)** Providing mechanisms for process synchronization.

**2. Memory management:** The main memory is generally the only large storage device that the CPU is able to address and access directly. To improve both the utilization of the CPU and the speed of the computer, general-purpose computers must keep several programs in memory, creating a need for memory management.

The operating system is responsible for the following activities in connection with memory management:

**(i)** Allocating and deallocating memory space as needed.  
**(ii)** Keeping track of which parts of memory are currently being used and which process is using them.  
**(iii)** Deciding which processes (or parts of processes) and data to move into and out of memory.

**3. File-System Management:** A file is a collection of related information defined by its creator. The operating system implements the abstract concept of a file <u>by managing mass storage media</u> and the devices that control them. In addition, files are usually organized into directories to make them easier to use.

The OS is responsible for the following activities in connection with file management:

**(i)** Creating and deleting files.  
**(ii)** Creating and deleting directories to organize files.  
**(iii)** Supporting primitives for manipulating files and directories.  
**(iv)** Mapping files onto mass storage.  
**(v)** Backing up files on stable (nonvolatile) storage media.  

**4. Mass-Storage Management:** The computer system must provide secondary storage to back up main memory. Most programs (including compilers, web browsers, word processors, games and so on) are stored on secondary storage devices until loaded into memory. The programs then use the devices as both the source and the destination of their processing. Hence, proper management of secondary storage is crucial.

The OS is responsible for the following activities in connection with secondary storage management:

**(i)** Mounting and unmounting.  
**(ii)** Storage allocation.  
**(iii)** Free-space management.  
**(iv)** Partitioning.  
**(v)** Disk Scheduling.  
**(vi)** Protection.

---
---
---

> [**Contact**](https://tawk.to/chat/66893d23eaf3bd8d4d18d232/1i241dlbj) us to buy the full document. *It's only $1.50!*