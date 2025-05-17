# Operating System - Unit 1: Introductory 🎓

## ⚙️ Components of a Computer

- **Central Processing Unit (CPU)**
    
    - Control Unit
        
    - Arithmetic Logic Unit
        
- **Input Unit** ⌨️🖱️🎤 (e.g., Mouse, Keyboard, Microphone)
    
- **Memory Unit**
    
    - Memory (Temporary) 💾
        
    - Storage (Permanent) 📦
        
- **Output Unit** 🖥️🖨️🔊 (e.g., Monitor, Printer, Speakers)
    

## 💻 Program

A program is a set of instructions in binary form (0s and 1s) that a computer executes.

0010101011101001010110101111010...

## 🗣️ Programming Languages

Examples: C, C++, Java, Python, JavaScript, C#, PHP, Perl, Go, Objective-C, Visual Basic.

## 🔄 Translators

A translator converts **Source Code** (written by programmers) into **Object Code** (machine-understandable code).

- **Types of Translators:**
    
    - **Assembler:** Converts assembly language (low-level) to binary machine language.
        
        - `Source text file` ➡️ `Assembler` ➡️ `Binary Machine Language (01101101...)`
            
    - **Compiler:** Translates the entire high-level language program into machine code at once, creating an executable file.
        
        - `Source file (e.g., Hi.cpp)` ➡️ `Compiler` ➡️ `Machine code (e.g., Hi.exe)` ➡️ `Output`
            
    - **Interpreter:** Translates and executes the high-level language program line by line.
        
        - `Source Code` ➡️ `Interpreter` ➡️ `Output`
            
- **Language Levels:**
    
    - High-Level Languages (e.g., C, Java, C++)
        
    - Assembly Language (Low-level)
        
    - Machine Code (Lowest-level, hardware-specific)
        

## 💾 Software

Software is a set of programs used to operate computers and execute specific tasks. It's the opposite of hardware.

- **Types of Software:**
    
    - **Application Software (Apps) 📱:** Programs designed for a specific purpose from the end-users' perspective.
        
        - _Examples:_ Web browser 🌐, word processors 📝, spreadsheet software 📊.
            
    - **System Software 🛠️:** Programs that:
        
        - Control and manage computer hardware operations.
            
        - Provide an environment for developing application software.
            
        - Provide an environment for executing application software.
            

## 🌟 Operating System (OS)

An OS is **system software** that controls and manages computer hardware operations and provides an environment for the execution of application software. It acts as an intermediary between the user/applications and the computer hardware.

- **Components of Operating System:**
    
    - **Kernel 核心:** The core component of the OS.
        
        - Manages system resources (memory, processes, devices).
            
        - Provides services to other programs.
            
        - Responsible for memory management, process scheduling, device drivers.
            
        - **Must always reside in memory.**
            
    - **Shell 🐚:** The layer where application programs and some system programs run. It's the interface for the user to interact with the OS.
        
        - _Note:_ In Linux, "shell" often refers to the command-line interpreter program. In general, it's the layer around the kernel.
            
- **System Call 📞:** The programmatic way in which a computer program requests a service from the kernel of the operating system.
    
    - `User Programs` ➡️ `System Calls` ➡️ `Kernel` ➡️ `Hardware`
        

## 📋 Operating System Types

1. **Batch Operating System ⏳:**
    
    - Popular in the 1970s.
        
    - Similar jobs were batched together and executed at once.
        
    - _Example:_ Early versions of OS/360, DOS/360 (1960s).
        
2. **Multiprogramming Operating System 📈:**
    
    - When a process does I/O, the CPU starts executing other processes.
        
    - Improves system efficiency.
        
3. **Multitasking Operating System 🤹:**
    
    - Enables a user to execute multiple computer tasks concurrently (seemingly at the same time).
        
4. **Multiprocessing Operating System 🚀:**
    
    - Has more than one processor.
        
    - Can execute more than one process simultaneously (true parallelism).
        
5. **Real-Time Operating System (RTOS) ⏱️:**
    
    - Each job has a specific deadline.
        
    - Delay can cause huge loss or make the result useless.
        
    - _Examples:_ PSOS, VRTX, RT Linux, Lynx OS, Windows CE.
        
    - **Hard RTOS:** Deadlines _must_ be met.
        
    - **Soft RTOS:** Missing a deadline is not critical for every task, but tasks should generally meet deadlines based on priority.
        
6. **Network Operating System (NOS) 🌐:**
    
    - Connects multiple devices and computers on a network.
        
    - Allows resource sharing on the network.
        
7. **Mobile Operating System 📱:**
    
    - Allows smartphones, tablets, etc., to run applications.
        
    - _Examples:_ Android, iOS, Symbian, KaiOS, Sailfish OS, Harmony OS.
        
8. **Distributed Operating System 🔗:**
    
    - Various autonomous interconnected computers communicate via a shared network.
        
    - Each system has its own memory and CPU (loosely coupled).
        
    - _Examples:_ Solaris, OSF/1, Micros, Dynix, Locus, Mach.
        
9. **Multiuser Operating System 👥:**
    
    - Multiple users can access different computer resources simultaneously.
        
    - Access is often via a network of PCs attached to a mainframe.
        

## 🛠️ Functions of Operating System

1. **Process Management 🏃:**
    
    - A program under execution is a process (active entity). A program is passive.
        
    - Scheduling processes/threads on CPUs.
        
    - Creating/deleting user and system processes.
        
    - Suspending/resuming processes.
        
    - Providing mechanisms for process communication.
        
2. **Process Synchronization 🔄:** (Mentioned in the list, but not detailed in this section of the PDF)
    
3. **Memory Management 🧠:**
    
    - Main memory is a repository of quickly accessible data.
        
    - Keeping track of memory usage.
        
    - Deciding which processes/data move into/out of memory.
        
    - Allocating/deallocating memory space.
        
    - Mapping logical to physical addresses.
        
4. **CPU Scheduling 📊:**
    
    - Deciding which task/process uses the CPU at a particular time.
        
    - Aims to: Maximize CPU utilization, Minimize response/waiting time.
        
5. **File Management / Storage Management 📂💾:**
    
    - Disks are the principal online storage for programs and data.
        
    - Free-space management.
        
    - Storage allocation.
        
    - Disk scheduling.
        
    - **Tertiary Storage:** (e.g., Magnetic tapes, CDs, DVDs)
        
        - Mounting/unmounting media.
            
        - Allocating/freeing devices.
            
        - Migrating data between secondary and tertiary storage.
            
6. **I/O Management 🎛️:**
    
    - Hides peculiarities of specific hardware devices from the user.
        
    - Components: Memory management (buffering, caching, spooling), general device-driver interface, drivers for specific hardware.
        
7. **Security 🛡️:**
    
    - Protection: Controlling access of processes/users to resources.
        
    - Defending the system from external/internal attacks (viruses, worms, denial-of-service, identity theft, theft of service).
        

## 🌀 Virtualization

Technology that allows operating systems to run as applications within other operating systems.

- An OS compiled for a specific CPU architecture runs within another OS native to that CPU.
    
- Originated on IBM mainframes for concurrent multi-user tasks.
    
- **Virtual Machine Manager (VMM):**
    
    - Runs guest operating systems.
        
    - Manages their resource use.
        
    - Protects each guest from others.
        
    - _Examples:_ VMware, ESX, Citrix XenServer (some now run as hosts themselves).
        
- **Virtual Machine (VM) 🖥️➡️💻:**
    
    - Virtual environments simulating a physical computer in software.
        
    - Comprise files for VM configuration, virtual hard drive storage, and snapshots.
        
- **Hypervisors ✨:**
    
    - Software layer coordinating VMs.
        
    - Interface between VM and physical hardware.
        
    - Ensures VMs don't interfere with each other.
        
    - **Type 1 Hypervisor (Bare-metal):** Interacts directly with physical resources, replacing the traditional OS.
        
    - **Type 2 Hypervisor:** Runs as an application on an existing OS. (Common on endpoints for running alternative OSs; has performance overhead).
        

## ☁️ Cloud Computing

Delivers computing, storage, and applications as a service across a network. A logical extension of virtualization.

- _Example:_ Amazon Elastic Compute Cloud (EC2).
    
- **Types based on Accessibility:**
    
    - **Public Cloud 🌍:** Available via the Internet to anyone willing to pay.
        
    - **Private Cloud 🏢:** Run by a company for its own use.
        
    - **Hybrid Cloud 🔄:** Includes both public and private components.
        
- **Types based on Content/Service Model:**
    
    - **Software as a Service (SaaS) 📧:** Applications available via the Internet (e.g., word processors, spreadsheets).
        
    - **Platform as a Service (PaaS) 🛠️:** Software stack ready for application use via the Internet (e.g., database server).
        
    - **Infrastructure as a Service (IaaS) 🏗️:** Servers or storage available over the Internet (e.g., backup storage).
        
- Cloud management tools (e.g., VMware vCloud Director, Eucalyptus) manage VMMs.
    

## 🔓 Open Source Operating System

Software released under a license where the copyright holder grants users the rights to use, study, change, and distribute the software and its source code.

- **Linux-based:** Ubuntu, Kali Linux, Linux Mint.
    
- **Non-Linux-based:** FreeDOS, ReactOS, Haiku.
    

## 🚀 System Boot (Booting / Bootstrapping)

The process of starting a computer.

- When a CPU is powered on, its main memory has no software. Booting loads software into memory.
    
- Involves turning on the computer, loading the OS into main memory, and preparing it for user commands.
    
- **BIOS (Basic Input/Output System) / UEFI (Unified Extensible Firmware Interface):**
    
    - Essential firmware interfaces; the first software layer on the motherboard.
        
    - BIOS: Traditional firmware for older systems.
        
    - UEFI: Modern replacement.
        
- **Steps of Booting:**
    
    1. **BIOS/UEFI is loaded:** When power is turned on.
        
    2. **BIOS/UEFI: Power-On Self-Test (POST):** Checks main memory, disk drives, I/O devices, etc. Errors indicated by beeps or on-screen notifications.
        
    3. **Loading of OS:** After successful POST, BIOS/UEFI reads the bootable sequence and loads the OS kernel.
        
    4. **System Configuration:** Device drivers are loaded into memory.
        

## 📜 History of Operating System

- **1956:** GM-NAA I/O by General Motors for IBM 704 (first OS for real work).
    
- **Early OSs:** Diverse, vendor/customer-specific for mainframes. New machine often meant a new OS.
    
- **1960s (IBM):**
    
    - System/360 series (same instruction & I/O architecture).
        
    - Goal: Single OS - **OS/360**.
        
    - Versions: PCP (Primary Control Program), MFT (Multiprogramming with a Fixed number of Tasks), MVT (Multiprogramming with a Variable number of Tasks).
        
    - **DOS/360** for smaller System/360 models. IBM maintained backward compatibility (programs from the 60s can still run on z/VSE or z/OS).
        
- **1960s (Control Data Corporation):**
    
    - SCOPE (batch processing).
        
    - MACE (time-sharing), basis for Kronos.
        
- **1970s (Control Data Corporation & University of Minnesota):**
    
    - Kronos, NOS (supported simultaneous batch and time-sharing).
        
- **UNIVAC (first commercial computer manufacturer):**
    
    - EXEC I for UNIVAC 1107.
        
    - EXEC II (by Computer Sciences Corporation) for UNIVAC 1107, ported to 1108.
        
    - EXEC 8 for UNIVAC 1108 (basis for later OSs in the family).
        
- **1962 (GE):**
    
    - GE-600 series with GECOS (General Electric Comprehensive Operating Supervisor).
        
    - Renamed GCOS (General Comprehensive Operating System) after Honeywell acquired GE's computer business.
        
- **1967 (Digital Equipment Corporation - DEC):**
    
    - TOPS-10 for PDP-10 (36-bit computers). Popular in universities and early ARPANET.
        
    - Improved to TOPS-20.
        
- **Scientific Data Systems/Xerox Data Systems (Sigma series):**
    
    - BCM (Basic Control Monitor), BPM (Batch Processing Monitor), BTM (Basic Time-Sharing Monitor).
        
    - UTS (Universal Time-Sharing System) succeeded BPM & BTM (multi-programming for online and batch).
        
    - CP-V succeeded UTS (combined UTS with Xerox Operating System).
        

## 🌟 Emergence of UNIX

- **Mid-1960s:** MIT, Bell Labs, General Electric developed **Multics** (time-sharing OS for GE 645 mainframe). Innovative but complex.
    
- Bell Labs researchers (Ken Thompson, Dennis Ritchie, Douglas McIlroy, Joe Ossanna) withdrew due to Multics' complexity and started a new, smaller project.
    
- **1970:** Coined the name **Unics** (Uniplexed Information and Computing Service) as a pun on Multics.
    
- Originally written in assembly language.
    
- **1973:** Version 4 Unix rewritten in **C**.
    
- **Research Unix:** Versions produced by Bell Labs.
    
- **1975:** First source license for UNIX sold to the University of Illinois Urbana–Champaign (UIUC).
    
- **Late 1970s - Early 1980s:** Large-scale adoption by commercial startups due to academic influence.
    
    - Led to fragmentation: DYNIX, HP-UX, SunOS/Solaris, AIX, Xenix (similar but often incompatible).
        
- **Wide Acceptance:** Because it was essentially free in early editions, easily obtainable, and modifiable.
    
- **1990s:** Unix and Unix-like systems grew popular.
    
    - OS of choice for >90% of the world's top 500 fastest supercomputers.
        
    - BSD and Linux distributions developed through worldwide collaboration.
        
- **2000:** Apple released **Darwin** (Unix system), the core of Mac OS X (later macOS).
    

## ✅ POSIX (Portable Operating System Interface)

- **Late 1980s:** Open operating system standardization effort.
    
- Provided a common baseline for all operating systems.
    
- **1988:** IEEE published the first POSIX standard, based on the common structure of major competing Unix variants.
    

## 🐧 Linux

A family of open-source Unix-like operating systems based on the **Linux kernel**.

- Kernel first released on **September 17, 1991, by Linus Torvalds**.
    
- Typically packaged as a **Linux distribution (distro)**: includes kernel, supporting system software, and libraries.
    
- Designed as a clone of Unix and released under the copyleft GPL license.
    

## 📱 History of Mobile Operating System

- **Early 1990s:** Psion released Psion Series 3 PDA with **EPOC** OS.
    
    - Later versions of EPOC became **Symbian**. Used by Nokia, Ericsson, Sony Ericsson, Motorola, Samsung, etc.
        
- **Symbian:** World's most widely used smartphone OS until 2010 (peak market share of 74% in 2006).
    
- **1996:** Palm Computing released Pilot 1000 & 5000 running **Palm OS**.
    
- **Microsoft Windows CE:** Base for Pocket PC 2000, renamed **Windows Mobile** in 2003.
    
    - Most common smartphone OS in the U.S. at its peak in 2007.
        
- **2007:** Apple introduced the **iPhone** and **iPhone OS** (later **iOS**).
    
    - Based on Unix-like Darwin.
        
    - Powerful and innovative graphic user interface (also used on iPad).
        
- **2008:** **Android** introduced.
    
    - Based on a modified Linux kernel, with its own graphical user interface.
        
- **2010:** Microsoft re-entered with **Windows Phone**.
    
- **2015:** Windows Phone replaced by **Windows 10 Mobile**.



---


# Operating System - Unit 2: Process and Thread 📄⚙️🧵

## 🏃 Process

- A program does nothing unless its instructions are executed by a CPU.
    
- A **program under execution** is called a **process**.
    
- To accomplish its task, a process needs computer resources.
    
- The OS manages processes and resources.
    
- A process is more than just program code. It includes:
    
    - Current activity (value of program counter, processor's registers).
        
- **Program:** Passive entity (e.g., executable file on disk).
    
- **Process:** Active entity (program counter, associated resources).
    
- A program becomes a process when an executable file is loaded into memory.
    

## 🚦 Process States

A process goes through different states during its lifecycle:

1. **New ✨:** The process is being created.
    
2. **Ready ✅:** The process is waiting to be assigned to a processor.
    
3. **Running 💨:** Instructions are being executed.
    
4. **Waiting ⏳:** The process is waiting for some event to occur (e.g., I/O completion, signal reception).
    
5. **Terminated 🛑:** The process has finished execution.
    

**(Diagram: new → admitted → ready ↔ scheduler dispatch ↔ running → interrupt → ready / → I/O or event wait → waiting → I/O or event completion → ready / running → exit → terminated)**

## 📇 Process Control Block (PCB)

Also called a **Task Control Block**. Each process is represented in the OS by a PCB. It contains information associated with a specific process:

- **Process State:** New, ready, running, waiting, halted, etc.
    
- **Process Number:** Unique identifier for the process.
    
- **Program Counter:** Address of the next instruction to be executed.
    
- **CPU Registers:** Accumulators, index registers, stack pointers, general-purpose registers, condition codes.
    
- **CPU-Scheduling Information:** Process priority, pointers to scheduling queues, other scheduling parameters.
    
- **Memory-Management Information:** Base and limit registers, page tables, or segment tables.
    
- **Accounting Information:** Resources used by the process (CPU time, memory usage).
    
- **I/O Status Information:** Open files, network connections, I/O devices allocated.
    

## 🗓️ Process Scheduling

- **Process Scheduling (CPU Scheduling):** The task of selecting a process for allocation to the CPU in a multiprogramming OS.
    
- **Process Scheduler (Scheduler):** Part of the OS that performs this task using a CPU scheduling algorithm.
    
- The scheduler selects an available process for execution on the CPU.
    

## რი Scheduling Queues

Processes move between various queues during their lifetime:

1. **Job Queue:** When a program execution is requested, the corresponding process is put in the Job Queue.
    
2. **Ready Queue:** Processes residing in main memory, ready and waiting to execute.
    
    - Generally stored as a linked list.
        
    - Header contains pointers to the first and final PCBs. Each PCB points to the next.
        
3. **Device Queues:** List of processes waiting for a particular I/O device (e.g., disk). Each device has its own device queue.
    

## 👨‍⚖️ Schedulers

The OS must select processes from these queues for scheduling.

1. **Long-Term Scheduler (Job Scheduler):**
    
    - Selects processes from the Job Queue and loads them into memory (new → ready state transition).
        
    - Controls the **degree of multiprogramming** (number of processes in memory).
        
    - Executes much less frequently.
        
    - Can afford to take more time to decide.
        
    - Should select a good mix of **I/O-bound** (spends more time on I/O) and **CPU-bound** (spends more time on computations) processes to keep the system balanced.
        
        - All I/O-bound: Ready queue often empty.
            
        - All CPU-bound: I/O waiting queue often empty, devices unused.
            
2. **Short-Term Scheduler (CPU Scheduler):**
    
    - Selects from processes in the Ready Queue and allocates the CPU to one of them.
        
    - Executes frequently (e.g., at least once every 100 milliseconds).
        
    - Must be very fast to minimize scheduling overhead.
        
3. **Medium-Term Scheduler (Optional):**
    
    - Sometimes advantageous to remove a process from memory (and later reintroduce it). This is called **swapping**.
        
    - The process is swapped out and later swapped in by the medium-term scheduler.
        
    - Swapping may be necessary to:
        
        - Improve the process mix.
            
        - Free up memory if it's overcommitted.
            

## 🔄 Context Switching

- Switching the CPU from one process to another.
    
- Requires performing a **state save** of the current process and a **state restore** of a different process.
    
- The system saves the current context (represented in the PCB) of the running process and loads the saved context of the new process.
    
- **Context-switch time is pure overhead** (no useful work is done).
    
- Speed varies based on memory speed, number of registers to copy, and existence of special hardware instructions.
    
- Hardware support can significantly reduce context-switch time (e.g., processors with multiple register sets).
    

## ⚙️ CPU Scheduling (Detailed)

- Decides the way and order in which processes should be executed.
    
- Process execution consists of a cycle of **CPU burst** (CPU execution) and **I/O burst** (I/O wait).
    
    - Execution begins with a CPU burst, followed by I/O burst, then another CPU burst, and so on.
        
    - The final CPU burst ends with a system request to terminate.
        
- The **short-term scheduler (CPU scheduler)** selects a process from the ready queue.
    
- The ready queue is not necessarily FIFO; it can be a FIFO queue, priority queue, tree, or unordered linked list.
    
- **Preemptive vs. Non-preemptive Scheduling:**
    
    - **Non-preemptive:** Processes are not deallocated the CPU unless an I/O occurs or the process terminates.
        
    - **Preemptive:** Processes can be interrupted (preempted) without an I/O operation or termination (e.g., when a higher-priority process arrives or a time slice expires).
        

## ⚖️ Scheduling Criteria

Used to compare CPU scheduling algorithms:

- **CPU Utilization ↑:** Keep the CPU as busy as possible (e.g., 40% for lightly loaded, 90% for heavily loaded).
    
- **Throughput ↑:** Number of processes completed per time unit.
    
- **Turnaround Time ↓:** Total time from submission to completion of a process.
    
    - `Turnaround Time (TAT) = Completion Time (CT) – Arrival Time (AT)`
        
    - `TAT = Burst Time (BT) + Waiting Time (WT)`
        
- **Waiting Time ↓:** Sum of periods spent waiting in the ready queue.
    
    - `Waiting Time (WT) = TAT – BT`
        
- **Response Time ↓:** Time from submission of a request until the first response is produced (time to get a response from the CPU).
    

**Goal:** Maximize CPU utilization and throughput; Minimize turnaround time, waiting time, and response time.

## 📊 CPU Scheduling Algorithms

### 1. First-Come, First-Served (FCFS) 🚶➡️🚶‍♀️➡️🚶‍♂️

- Simplest CPU scheduling algorithm.
    
- **Non-preemptive.**
    
- Process requesting the CPU first is allocated the CPU first.
    
- Managed with a FIFO queue (PCB linked to tail, CPU allocated to head).
    
- Simple to write and understand.
    
- **Convoy Effect:** If processes with high burst times arrive first, shorter processes may get blocked for a long time.
    
- **Advantages:** Easy to implement.
    
- **Disadvantages:** Convoy effect, non-preemptive (doesn't release CPU until completion/IO).
    
    _Example calculation provided in slides for TAT and WT._
    

### 2. Shortest Job First (SJF) 📏➡️🥇

- **Non-preemptive** (as described in this section of PDF, though a preemptive version exists).
    
- Heavily dependent on Burst Times.
    
- CPU is allotted to the process in the ready queue with the least Burst Time.
    
- If two processes have the same Burst Time, FCFS is typically used.
    
- Generally has less average waiting time (heavy processes executed last).
    
- **Starvation:** A major negative trait. Long processes might never get executed if short processes keep arriving.
    
    _Example calculation provided in slides._
    

### 3. Shortest Remaining Time First (SRTF) ⏱️⚡

- **Preemptive version of SJF.**
    
- Execution can be stopped after a certain amount of time.
    
- At the arrival of every process, the short-term scheduler schedules the process with the **least remaining burst time** among available processes and the currently running process.
    
    _Example calculation provided in slides._
    

### 4. Round Robin (RR) 🔄🕰️

- **Preemptive** scheduling algorithm.
    
- Uses a **Time Quantum (TQ)** or time slice.
    
- Main emphasis is on **Time Sharing**.
    
- Each process is allocated CPU time equal to TQ before being preempted and moved to the end of the ready queue.
    
- **Advantages:**
    
    - Fair CPU allocation.
        
    - Can be implemented in the system (doesn't depend on burst time).
        
    - Not affected by convoy effect or starvation.
        
- **Disadvantages:**
    
    - Small TQ leads to increased context switching overhead, decreasing CPU output.
        
    - Longer context swap times.
        
    - Performance heavily depends on the chosen TQ.
        
    
    _Example calculation provided in slides._
    

### 5. Priority Scheduling 🥇🥈🥉

- A priority is associated with each process.
    
- CPU is allocated to the process with the **highest priority**.
    
- Equal-priority processes are scheduled in FCFS order.
    
- SJF can be considered a priority algorithm where priority is the inverse of the predicted next CPU burst (larger burst = lower priority).
    
- Priorities: Indicated by a fixed range of numbers (e.g., 0 to 7). Convention varies (low number = high priority OR low number = low priority). **Here, assume low numbers = high priority.**
    
- Can be **preemptive** or **non-preemptive**:
    
    - **Preemptive:** If a new process arrives with higher priority than the running process, the CPU is preempted.
        
    - **Non-preemptive:** The new process is put at the head of the ready queue.
        
- **Starvation (Indefinite Blocking):** Low-priority processes may wait indefinitely.
    
    - **Solution: Aging** - Gradually increasing the priority of processes that wait in the system for a long time.
        
    
    _Example calculation provided in slides._
    

### 6. Multilevel Queue Scheduling 📊➡️📊➡️📊

- For situations where processes are easily classified into different groups.
    
- Partitions the ready queue into several **separate queues**.
    
- Processes are **permanently assigned** to one queue based on properties like memory size, priority, or type.
    
- Each queue has its **own scheduling algorithm** (e.g., foreground queue with RR, background queue with FCFS).
    
- **Scheduling among queues** is needed:
    
    - Commonly implemented as **fixed-priority preemptive scheduling** (e.g., system processes > interactive > batch). Higher-priority queues must be empty for lower-priority queues to run.
        
    - Alternatively, **time-slicing among queues** (each queue gets a certain portion of CPU time).
        

### 7. Multilevel Feedback Queue Scheduling 🔄📊⬆️⬇️

- Allows a process to **move between queues**.
    
- Separates processes based on their CPU burst characteristics.
    
- If a process uses too much CPU time, it's moved to a lower-priority queue.
    
    - Keeps I/O-bound and interactive processes in higher-priority queues.
        
- **Aging:** A process waiting too long in a lower-priority queue may be moved to a higher-priority queue (prevents starvation).
    
- **Characterization Parameters:**
    
    - Number of queues.
        
    - Scheduling algorithm for each queue.
        
    - Method to upgrade a process.
        
    - Method to demote a process.
        
    - Method to determine which queue a process enters on arrival.
        
- **Example:**
    
    - 3 queues (0, 1, 2). Queue 0 highest priority.
        
    - Scheduler executes all in Q0, then Q1 (if Q0 empty), then Q2 (if Q0 & Q1 empty).
        
    - New process enters Q0. Given TQ (e.g., 8ms). If not finished, moved to Q1.
        
    - Process in Q1 given TQ (e.g., 16ms). If not finished, moved to Q2.
        
    - Processes in Q2 run on FCFS basis only when Q0 and Q1 are empty.
        

## 💬 Inter-Process Communication (IPC)

- **Independent Process:** Cannot affect or be affected by other executing processes. Does not share data.
    
- **Cooperating Process:** Can affect or be affected by other executing processes. Shares data.
    
- Cooperating processes require an IPC mechanism to exchange data and information.
    
- **Two Fundamental Models of IPC:**
    
    1. **Shared Memory 🤝💾:**
        
        - A region of memory is shared by cooperating processes.
            
        - Processes exchange information by reading and writing data to the shared region.
            
        - Typically, the shared region resides in the address space of the creating process.
            
        - Other processes must attach this shared segment to their address space.
            
        - Requires processes to agree to remove normal memory protection.
            
        - Processes are responsible for ensuring consistency (not writing to the same location simultaneously).
            
    2. **Message Passing 📨➡️📬:**
        
        - Communication takes place by exchanging messages between cooperating processes.
            
        - Allows processes to communicate and synchronize without sharing an address space.
            
        - The kernel is responsible for message transmission.
            
    
    _Both models are common, and many systems implement both._
    

## 🌐 Communication Over Network

Shared memory and message passing are typical for standalone systems. For processes on different machines in a network:

1. **Sockets 🔌:**
    
    - A pair of processes communicating over a network uses a pair of sockets (one for each).
        
    - A **socket** is an endpoint for communication.
        
    - Identified by an **IP address concatenated with a port number**.
        
    - Uses a **client-server architecture**.
        
    - Server waits for incoming client requests by listening to a specified port.
        
    - Once a request is received, the server accepts a connection from the client socket.
        
    - **Well-known ports:** Used by servers implementing specific services (e.g., Telnet: 23, FTP: 21, HTTP: 80).
        
    - **Client ports:** When a client initiates a connection, its host assigns an arbitrary port number (typically > 49151).
        
    - **Network Port Ranges:**
        
        - Well-known Ports: 0 - 1023
            
        - Registered Ports: 1024 - 49151
            
        - Dynamic Ports: 49152 - 65565
            
2. **Remote Procedure Call (RPC) 📞⚙️:**
    
    - Messages exchanged are well-structured (not just packets of data).
        
    - Each message is addressed to an RPC daemon listening on the remote system.
        
    - Message contains an identifier for the function to execute and its parameters.
        
    - The function is executed remotely, and output is sent back in a separate message.
        

## 🧵 Thread

- A **basic unit of CPU utilization**.
    
- It shares with other threads belonging to the same process its:
    
    - Code section
        
    - Data section
        
    - Other OS resources (open files, signals)
        
- A traditional (heavyweight) process has a single thread of control.
    
- If a process has multiple threads, it can perform more than one task at a time.
    
    - _Example:_ Web browser (one thread for display, another for network retrieval), Word processor (threads for graphics, keystrokes, spell check).
        
- **Single-threaded process vs. Multithreaded process:**
    
    - A multithreaded process has multiple threads, each with its own registers and stack, but sharing code, data, and files.
        
- **User Threads vs. Kernel Threads:**
    
    - Support for threads can be at the user level or kernel level.
        
    - **User Threads:** Supported above the kernel, managed without kernel support (by a thread library in user space).
        
    - **Kernel Threads:** Supported and managed directly by the OS.
        
- **Models for User-Kernel Thread Communication:**
    
    1. **Many-to-One Model 🧑‍🤝‍🧑➡️👤:**
        
        - Maps many user-level threads to one kernel thread.
            
        - Thread management by thread library in user space.
            
        - If one user thread makes a blocking system call, the entire process blocks.
            
        - Multiple threads cannot run in parallel on multicore systems because only one can be in the kernel at a time.
            
    2. **One-to-One Model 👤➡️👤:**
        
        - Maps each user thread to a kernel thread.
            
        - Provides more concurrency (another thread can run if one blocks).
            
        - Allows multiple threads to run in parallel on multiprocessors.
            
        - Overhead: Creating a user thread requires creating a corresponding kernel thread.
            
    3. **Many-to-Many Model 🧑‍🤝‍🧑➡️👥:**
        
        - Multiplexes many user-level threads to a smaller or equal number of kernel threads.
            
        - Number of kernel threads can be specific to the application or machine.
            
        - Allows developers to create as many user threads as necessary.
            
        - Corresponding kernel threads can run in parallel on a multiprocessor.
            
        - When a thread performs a blocking call, the kernel can schedule another thread for execution.




---


# Operating System - Unit 3: Process Synchronization 📄🔄🔒

## 🤔 Process Types (Recap)

- **Independent Process:** Cannot affect or be affected by other executing processes. Does not share data.
    
- **Cooperating Process:** Can affect or be affected by other executing processes. Shares data.
    
    - IPC approaches for cooperating processes: Shared Memory and Message Passing.
        

## 🔄 Process Synchronization

- **Need:** When using shared memory for IPC, we must prevent inconsistencies.
    
- **Definition:** The task of coordinating the execution of cooperating processes so that no two processes can access shared data and resources simultaneously in a way that causes inconsistencies.
    

## 🧺 Producer-Consumer Problem

A classic synchronization problem.

- **Scenario:**
    
    - A fixed-size buffer.
        
    - **Producer Process:** Creates items and adds them to the shared buffer.
        
    - **Consumer Process:** Takes items out of the shared buffer and "consumes" them.
        
- **Pseudocode Snippet (Illustrative):**
    
    - **Producer:**
        
        ```c
        while (true) {
            while (counter == BUFFER_SIZE); // Wait if buffer is full
            buffer[in] = nextProduced;
            in = (in + 1) % BUFFER_SIZE;
            counter++;
        }
        ```
        
    - **Consumer:**
        
        ```c
        while (true) {
            while (counter == 0); // Wait if buffer is empty
            nextConsumed = buffer[out];
            out = (out + 1) % BUFFER_SIZE;
            counter--;
        }
        ```
        
- **Concurrency Issue:**
    
    - If `counter++` (from producer) and `counter--` (from consumer) execute concurrently, the value of `counter` can be incorrect (e.g., 4, 5, or 6 when it should be 5).
        
    - **Example of Interleaving:**
        
        - `counter++` can be broken down: `register1 = counter`, `register1 = register1 + 1`, `counter = register1`.
            
        - `counter--` can be broken down: `register2 = counter`, `register2 = register2 - 1`, `counter = register2`.
            
        - If these instructions interleave, `counter` might end up as 4 (if consumer's final write happens last using an old value) or 6 (if producer's final write happens last using an old value).
            
- **Race Condition 🏁:**
    
    - A situation where several processes access and manipulate the same data concurrently, and the outcome of the execution depends on the particular order in which the access takes place.
        
    - To prevent race conditions, we need to ensure only one process manipulates the shared variable (e.g., `counter`) at a time via synchronization.
        

## Critical Section Problem 🚧

- **Critical Section:** A segment of code in a process where it may be changing common variables, updating a table, writing a file, etc.
    
- **Rule:** When one process is executing in its critical section, no other process should be allowed to execute in its critical section (for the same shared resource).
    
- **Problem:** To design a protocol that processes can use to cooperate.
    
- **Structure of a Process:**
    
    ```c
    do {
        entry section  // Request permission to enter CS
        critical section
        exit section   // Release CS
        remainder section
    } while (TRUE);
    ```
    
- The goal is to design protocols to ensure race conditions never arise.
    
- **Requirements for a Solution:**
    
    1. **Mutual Exclusion 🛡️:** If process Pi​ is in its critical section, no other processes can be in their critical sections.
        
    2. **Progress 🏃💨:** If no process is in its critical section and some processes wish to enter, then only those not in their remainder sections can participate in deciding who enters next. This selection cannot be postponed indefinitely.
        
    3. **Bounded Waiting ⏳🔢:** There's a limit on the number of times other processes are allowed to enter their critical sections after a process has requested entry and before its request is granted.
        

### 1. Peterson’s Solution (Software-based)

- Classic software solution for **two processes** (P0​ and P1​) alternating between critical and remainder sections.
    
- Let Pj​ be the _other_ process when discussing Pi​ (i.e., j=1−i).
    
- **Shared Data Items:**
    
    - `int turn;` (Indicates whose turn it is to enter CS. If `turn == i`, Pi​ can enter).
        
    - `boolean flag[2];` (Indicates if a process is ready. If `flag[i]` is true, Pi​ is ready).
        
- **Algorithm for Process** Pi​**:**
    
    ```c
    do {
        flag[i] = TRUE;
        turn = j;
        while (flag[j] && turn == j); // Busy wait
    
        critical section
    
        flag[i] = FALSE;
    
        remainder section
    } while (TRUE);
    ```
    
- **How it Works:**
    
    - To enter, Pi​ sets `flag[i] = TRUE` and `turn = j` (giving Pj​ a chance if it also wants to enter).
        
    - If both try simultaneously, `turn` is set to both `i` and `j` roughly at the same time, but only the last assignment sticks, deciding who enters first.
        
- **Verification:**
    
    - **Mutual Exclusion:** Yes. Pi​ enters CS only if `flag[j] == false` OR `turn == i`. If both are in CS, then `flag[0] == flag[1] == true`. This implies `turn` would have to be both 0 and 1, which is impossible.
        
    - **Progress:** Yes. After exiting, Pi​ sets `flag[i] = false`, which doesn't block Pj​.
        
    - **Bounded Waiting:** Yes. If Pj​ resets `flag[j] = true`, it must also set `turn = i`. Since Pi​ doesn't change `turn` in its `while` loop, Pi​ will enter after at most one entry by Pj​.
        

### 2. Bakery Algorithm (Software-based for N processes) 🥖🔢

- Proposed by Lamport for **n processes**.
    
- Follows a "first-come, first-served" principle, like a bakery issuing token numbers.
    
- Process with the lowest token number enters the critical section.
    
- If two processes have the same token number, the one with the lower process ID enters.
    
- **Shared Data:**
    
    - `boolean entering[n];` (Initialized to `false`. `entering[i] = true` means Pi​ is choosing a token).
        
    - `int number[n];` (Initialized to `0`. Stores token numbers).
        
- **Algorithm for Process** Pi​**:**
    
    ```c
    do {
        entering[i] = true; // Show interest
        number[i] = 1 + max(number[0], ..., number[n-1]); // Get a token
        entering[i] = false;
    
        for (j = 0; j < n; j++) {
            // Busy wait until process Pj receives its token number
            while (entering[j]) { /* do nothing */ }
            // Busy wait if Pj has a smaller token, or same token and smaller ID
            while (number[j] != 0 && (number[j], j) < (number[i], i)) { /* do nothing */ }
        }
    
        // critical section
    
        number[i] = 0; // Exit section: Reset token
    
        // remainder section
    } while(true);
    ```
    
    _(Note: `(a,b) < (c,d)` means `a < c` or (`a == c` and `b < d`))_
    
- **How it Works:**
    
    - Pi​ sets `entering[i] = true`, chooses a token number greater than any existing one, then sets `entering[i] = false`.
        
    - It then checks other processes Pj​:
        
        - Waits if Pj​ is currently choosing a token (`entering[j]`).
            
        - Waits if Pj​ has a token and has higher priority (smaller token, or same token with smaller process ID).
            
- **Verification:**
    
    - **Mutual Exclusion:** Yes. Only the process with the overall smallest `(number[i], i)` pair enters. Since process IDs are distinct, ties in numbers are broken.
        
    - **Progress:** Yes. A waiting process checks if others have higher priority. If not, it enters. Processes in remainder section (`number[i] == 0`) don't influence this.
        
    - **Bounded Waiting:** Yes. A process gets a token `1 + max_existing_token`. There's a finite number of processes with smaller tokens. New arrivals get larger tokens. FIFO-like.
        

## 🛠️ Synchronization Hardware

Software solutions like Peterson's and Bakery can be complex. Hardware support can simplify things. Solutions are often based on **locking**.

- **Locking:** Protecting critical regions using locks (special variables).
    
- Modern systems provide special **atomic hardware instructions** (executed as one uninterruptible unit).
    
    - `test_and_set()`
        
    - `swap()`
        

### 1. `test_and_set()` Instruction

- **Shared variable:** `boolean lock;` (initialized to `false`)
    
- **Instruction Logic (atomic):**
    
    ```c
    boolean TestAndSet(boolean *target) {
        boolean rv = *target;
        *target = TRUE;
        return rv;
    }
    ```
    
- **Usage for Critical Section:**
    
    ```c
    // Shared: boolean lock = false;
    do {
        while (TestAndSet(&lock)); // Busy wait if lock is true
    
        critical section
    
        lock = FALSE; // Release lock
    
        remainder section
    } while (true);
    ```
    
    - If `lock` is `false`, `TestAndSet` returns `false` (loop terminates), sets `lock` to `true`. Process enters CS.
        
    - If `lock` is `true`, `TestAndSet` returns `true` (loop continues), `lock` remains `true`. Process waits.
        

### 2. `swap()` Instruction

- **Shared variable:** `boolean lock;` (initialized to `false`)
    
- **Individual variable per process:** `boolean key;`
    
- **Instruction Logic (atomic):**
    
    ```c
    void Swap(boolean *a, boolean *b) {
        boolean temp = *a;
        *a = *b;
        *b = temp;
    }
    ```
    
- **Usage for Critical Section:**
    
    ```c
    // Shared: boolean lock = false;
    // Process Pi: boolean key;
    do {
        key = TRUE;
        while (key == TRUE) { // Busy wait
            Swap(&lock, &key);
        }
    
        critical section
    
        lock = FALSE; // Release lock
    
        remainder section
    } while (true);
    ```
    
    - Process sets its `key = TRUE`.
        
    - It repeatedly swaps `lock` and `key`.
        
    - If `lock` was `FALSE` (available), `key` becomes `FALSE` after swap, loop terminates. `lock` becomes `TRUE`. Process enters CS.
        
    - If `lock` was `TRUE` (unavailable), `key` remains `TRUE` after swap. Loop continues.
        

## 🔧 Synchronization Software Tools

Hardware solutions are often complex and not directly accessible to application programmers. OS designers build software tools.

### 1. Mutex Lock (Mutual Exclusion) 🗝️

- Simplest software tool.
    
- Used to protect critical regions and prevent race conditions.
    
- Process must **acquire** the lock before entering CS and **release** it when exiting.
    
- **Functions:**
    
    - `acquire()`
        
    - `release()`
        
- **Internal:**
    
    - A `boolean` variable `available` indicates if the lock is available.
        
    - `acquire()`: If lock is available, it succeeds, and lock becomes unavailable. If unavailable, process blocks (or busy waits) until released.
        
    - `release()`: Makes the lock available.
        
- `acquire()` and `release()` must be **atomic** (often implemented using atomic hardware instructions).
    
- **Structure:**
    
    ```c
    // Mutex lock: boolean available = true; (initially)
    
    acquire() {
        while (!available); // Busy wait
        available = false;
    }
    
    release() {
        available = true;
    }
    
    // Process code:
    do {
        acquire_lock();
        critical section
        release_lock();
        remainder section
    } while (true);
    ```
    
    - The `acquire()` shown uses **busy waiting** (also called a spinlock), which can waste CPU cycles. Alternatives involve putting the process to sleep and waking it up.
        

### 2. Semaphore 🚦

- More robust software tool than mutex locks.
    
- An integer variable `S`.
    
- Accessed only through two standard **atomic operations**:
    
    - `wait(S)` (sometimes called `P(S)` or `down(S)`)
        
    - `signal(S)` (sometimes called `V(S)` or `up(S)`)
        
- **Classical Definitions:**
    
    ```c
    wait(S) { // P(S)
        while (S <= 0); // Busy wait or block
        S--;
    }
    
    signal(S) { // V(S)
        S++;
    }
    ```
    
    _(Note: Modern implementations of `wait` usually block the process if `S <= 0` instead of busy waiting, placing it in a waiting queue associated with the semaphore.)_
    
- **Types of Semaphores:**
    
    1. **Counting Semaphore:** Value can range over an unrestricted domain.
        
        - Used to control access to a resource with a finite number of instances.
            
        - Initialized to the number of available resources.
            
        - `wait()`: Decrements count (acquires a resource). If count is 0, process blocks.
            
        - `signal()`: Increments count (releases a resource). Wakes up a blocked process if any.
            
    2. **Binary Semaphore (Mutex Semaphore):** Value can range only between 0 and 1.
        
        - Similar to a mutex lock.
            
        - Used for mutual exclusion.
            
        - Initialized to 1.
            
        - **Critical Section Usage (n processes):**
            
            ```c
            // Semaphore mutex initialized to 1;
            do {
                wait(mutex);
                // critical section
                signal(mutex);
                // remainder section
            } while (TRUE);
            ```
            
- **Using Semaphores for Synchronization:**
    
    - To ensure statement `S2` in process `P2` executes only after `S1` in `P1`:
        
        - Share a common semaphore `synch`, initialized to `0`.
            
        - **P1:**
            
            ```c
            S1;
            signal(synch);
            ```
            
        - **P2:**
            
            ```c
            wait(synch);
            S2;
            ```
            
        - Since `synch` is 0, `P2` will wait at `wait(synch)` until `P1` executes `S1` and then `signal(synch)`.
            

## 🧺 Producer-Consumer Problem with Semaphores

- **Semaphores Used:**
    
    - `mutex`: Binary semaphore for mutual exclusion when accessing the buffer. Initialized to `1`.
        
    - `empty`: Counting semaphore representing the number of empty slots in the buffer. Initialized to `BUFFER_SIZE` (n).
        
    - `full`: Counting semaphore representing the number of full slots in the buffer. Initialized to `0`.
        
- **Producer Process:**
    
    ```c
    do {
        // produce an item
        wait(empty);    // Wait if buffer is full (empty slots = 0), then decrement empty
        wait(mutex);    // Acquire lock for buffer access
    
        // add item to buffer
    
        signal(mutex);  // Release lock
        signal(full);   // Increment count of full slots (wake up consumer if waiting)
    } while (TRUE);
    ```
    
- **Consumer Process:**
    
    ```c
    do {
        wait(full);     // Wait if buffer is empty (full slots = 0), then decrement full
        wait(mutex);    // Acquire lock for buffer access
    
        // remove item from buffer
    
        signal(mutex);  // Release lock
        signal(empty);  // Increment count of empty slots (wake up producer if waiting)
    
        // consume the item
    } while (TRUE);
    ```
    

## 🍽️ Classical Inter-Process Communication Problems

### 1. The Dining Philosophers Problem 🍝🤔

- **Scenario:**
    
    - Five philosophers seated around a circular table.
        
    - Each has a plate of spaghetti.
        
    - Needs two forks to eat (one from left, one from right).
        
    - One fork between each pair of plates.
        
- **Life Cycle:** Alternating periods of thinking and eating.
    
- **To Eat:** Tries to acquire left and right forks (one at a time, any order). If successful, eats, then puts down forks and thinks.
    
- **Problem:** Write a program for each philosopher that works correctly and never gets stuck (deadlock or starvation).
    
- **Initial (Flawed) Approach:**
    
    ```c
    #define N 5 // number of philosophers
    
    void philosopher(int i) { // i is philosopher number 0 to 4
        while (TRUE) {
            think();
            take_fork(i);             // Take left fork
            take_fork((i + 1) % N);   // Take right fork
            eat();
            put_fork(i);
            put_fork((i + 1) % N);
        }
    }
    ```
    
    - **Deadlock:** If all five philosophers take their left forks simultaneously, none can get their right fork.
        
- **Second (Also Flawed) Approach:**
    
    - After taking the left fork, check if the right is available. If not, put down the left, wait, and repeat.
        
    - **Starvation/Livelock:** All philosophers could repeatedly pick up left forks, find right unavailable, put left down, wait, and repeat in lockstep indefinitely without making progress.
        
    - Waiting a _random_ time can reduce the chance of indefinite lockstep.
        
- **A Semaphore-based Solution (Dijkstra/Hoare):**
    
    - `#define N 5`
        
    - `#define LEFT (i + N - 1) % N`
        
    - `#define RIGHT (i + 1) % N`
        
    - `#define THINKING 0`
        
    - `#define HUNGRY 1`
        
    - `#define EATING 2`
        
    - `int state[N];` (Keeps track of philosopher's state: THINKING, HUNGRY, EATING. Initialized to THINKING or -1 as per slide)
        
    - `semaphore mutex = 1;` (For mutual exclusion on `state` array access)
        
    - `semaphore S[N];` (One semaphore per philosopher, initialized to 0. Used to block philosophers if forks aren't available)
        
    - **`philosopher(int i)`:**
        
        ```c
        void philosopher(int i) {
            while (TRUE) {
                think();
                take_forks(i); // Acquire two forks or block
                eat();
                put_forks(i);  // Put both forks back
            }
        }
        ```
        
    - **`take_forks(int i)`:**
        
        ```c
        void take_forks(int i) {
            down(&mutex);       // Enter critical region for state
            state[i] = HUNGRY;
            test(i);            // Try to acquire 2 forks
            up(&mutex);         // Exit critical region
            down(&S[i]);        // Block if forks not acquired (S[i] was 0)
        }
        ```
        
    - **`put_forks(int i)`:**
        
        ```c
        void put_forks(int i) {
            down(&mutex);       // Enter critical region
            state[i] = THINKING;
            test(LEFT);         // See if left neighbor can now eat
            test(RIGHT);        // See if right neighbor can now eat
            up(&mutex);         // Exit critical region
        }
        ```
        
    - **`test(int i)`:** (Called within mutex protection)
        
        ```c
        void test(int i) {
            if (state[i] == HUNGRY &&
                state[LEFT] != EATING &&
                state[RIGHT] != EATING) {
                state[i] = EATING;
                up(&S[i]); // Signal philosopher i they can eat (if they were waiting)
            }
        }
        ```
        
    - **Explanation:** A philosopher `i` can only eat if they are `HUNGRY` and their `LEFT` and `RIGHT` neighbors are not `EATING`. `S[i]` is used to block a philosopher if they cannot get both forks. When forks are put down, neighbors are tested to see if they can now eat.
        

### 2. The Readers and Writers Problem 📖✍️

- Models access to a database or shared data structure.
    
- **Rules:**
    
    - Multiple processes (readers) can read the data simultaneously.
        
    - If one process (writer) is updating the data, no other process (reader or writer) may access it.
        
- **A Semaphore-based Solution (First Readers-Writers Problem - favors readers):**
    
    - `semaphore mutex = 1;` (Controls access to `rc` - reader count)
        
    - `semaphore db = 1;` (Controls access to the database. Acts as a lock for writers, and for the first/last reader)
        
    - `int rc = 0;` (# of processes currently reading)
        
    - **`reader()`:**
        
        ```c
        void reader(void) {
            while (TRUE) {
                down(&mutex);       // Exclusive access to rc
                rc = rc + 1;
                if (rc == 1) {      // If this is the first reader
                    down(&db);      // Lock the database for writers
                }
                up(&mutex);         // Release exclusive access to rc
        
                read_data_base();   // Read data
        
                down(&mutex);       // Exclusive access to rc
                rc = rc - 1;
                if (rc == 0) {      // If this is the last reader
                    up(&db);        // Release database lock for writers
                }
                up(&mutex);         // Release exclusive access to rc
        
                use_data_read();    // Non-critical section
            }
        }
        ```
        
    - **`writer()`:**
        
        ```c
        void writer(void) {
            while (TRUE) {
                think_up_data();    // Non-critical section
                down(&db);          // Get exclusive access to database
                write_data_base();  // Update data
                up(&db);            // Release exclusive access
            }
        }
        ```
        
    - **Behavior:**
        
        - First reader locks `db`. Subsequent readers just increment `rc`.
            
        - Last reader unlocks `db`.
            
        - Writers must wait for `db` to be free.
            
        - **Problem (Reader Priority):** If there's a steady supply of readers, they can continuously enter, and a writer might be kept suspended (starvation of writers).
            
- **Alternative (Writer Priority):**
    
    - To avoid writer starvation, when a reader arrives and a writer is waiting, the reader is suspended behind the writer instead of being admitted immediately.
        
    - A writer only has to wait for readers that were active when it arrived, not for readers that came after it. (This solution is more complex and not fully detailed in the provided PDF slides).



---



# Operating System - Unit 4: Deadlock🚦

## 🧐 What is a Deadlock?

A **deadlock** is a situation where a set of processes are blocked because each process is holding a resource and waiting for another resource acquired by some other process. 🛑

Imagine two cars 🚗🚕 on a narrow one-way bridge, each wanting to cross but blocked by the other. Neither can move forward!

**Example:**

- Process A requests and gets the Scanner 📠.
    
- Process B requests and gets the CD Recorder 💿.
    
- Now, Process A needs the CD Recorder (held by B).
    
- And Process B needs the Scanner (held by A).
    
- Both are stuck waiting for each other indefinitely! This is a deadlock.
    

A resource can be a hardware device (e.g., printer 🖨️, tape drive 📼) or a piece of information (e.g., a locked record in a database 💾). It's anything that can be used by only a single process at any instant of time.

## 📋 Necessary Conditions for Deadlock

For a deadlock to occur, **all four** of these conditions must hold simultaneously (Coffman et al., 1971):

1. **Mutual Exclusion Condition** 🛡️:
    
    - At least one resource must be held in a non-sharable mode. That is, only one process at a time can use the resource. If another process requests that resource, the requesting process must be delayed until the resource has been released.
        
    - _Example:_ A printer cannot be shared by two processes simultaneously.
        
2. **Hold and Wait Condition** ⏳:
    
    - A process must be holding at least one resource and waiting to acquire additional resources that are currently being held by other processes.
        
    - _Example:_ Process A holds a scanner and is waiting for a CD recorder.
        
3. **No Preemption Condition** 🚫➡️:
    
    - Resources cannot be preempted. A resource can be released only voluntarily by the process holding it, after that process has completed its task.
        
    - _Example:_ If a process has a file open, the OS cannot just take it away.
        
4. **Circular Wait Condition** 🔄:
    
    - There must exist a set {P0, P1, ..., Pn} of waiting processes such that P0 is waiting for a resource held by P1, P1 is waiting for a resource held by P2, ..., Pn-1 is waiting for a resource held by Pn, and Pn is waiting for a resource held by P0.
        
    - _Example:_ Process A waits for Process B, and Process B waits for Process A.
        

## 📊 Resource Allocation Graph (RAG)

This is a directed graph used to describe deadlocks.

- **Circles (O)** represent processes.
    
- **Squares (□)** represent resources.
    
- **Arc from resource to process (□ → O):** Resource is held by the process.
    
- **Arc from process to resource (O → □):** Process is requesting/waiting for the resource.
    

**A cycle in the RAG indicates a deadlock** (if there's only one instance of each resource type).

(a) Holding a resource: R → P

(b) Requesting a resource: P → R

(c) Deadlock: P1 → R1, R1 → P2, P2 → R2, R2 → P1 (Cycle!)

## 🤔 How to Deal with Deadlocks?

There are four main approaches:

1. **The Ostrich Algorithm (Ignore the Problem) 🙈**:
    
    - Pretend deadlocks don't exist. If they happen rarely and the cost of prevention/avoidance is high, this might be chosen. (Not generally a good idea for critical systems!)
        
    - _Analogy:_ Sticking your head in the sand.
        
2. **Detection and Recovery 🔎🛠️**:
    
    - Let deadlocks occur, then detect them. Once detected, take action to recover.
        
    - This involves algorithms to check for cycles in resource allocation graphs or wait-for graphs.
        
    - Recovery might involve:
        
        - Aborting one or more deadlocked processes.
            
        - Preempting resources from some processes.
            
3. **Dynamic Avoidance (Careful Resource Allocation) 🚦**:
    
    - The system makes decisions on resource allocation dynamically to ensure it never enters an unsafe state (a state that _could_ lead to a deadlock).
        
    - Requires prior information about resource needs.
        
    - Key concept: **Safe State**.
        
4. **Prevention (Negate a Necessary Condition) 🧱**:
    
    - Structurally negate one of the four necessary conditions for deadlock, making deadlocks impossible.
        

## 🛡️ Deadlock Prevention

Goal: Ensure at least one of the four necessary conditions cannot hold.

1. **Addressing Mutual Exclusion**:
    
    - Make resources sharable. However, some resources are inherently non-sharable (e.g., a printer). So, this isn't always feasible.
        
2. **Addressing Hold and Wait**:
    
    - **Strategy 1:** Require processes to request ALL their resources _before_ starting execution.
        
        - _Problem:_ Processes often don't know all future needs. Resources might be held unnecessarily long, reducing utilization.
            
    - **Strategy 2:** Require a process to release all currently held resources before requesting new ones. Then, it tries to get everything it needs at once.
        
        - _Problem:_ Inefficient, may lead to starvation.
            
3. **Addressing No Preemption**:
    
    - **Strategy 1:** If a process holding resources requests another resource that cannot be immediately allocated, all currently held resources are preempted (released). The process restarts when it can get all old and new resources.
        
    - **Strategy 2:** If a requested resource is held by _another waiting_ process, preempt it. If held by a running process (not waiting), the requesting process must wait. While waiting, its resources can be preempted if requested by another process.
        
        - _Problem:_ Complex to implement, can be costly.
            
4. **Addressing Circular Wait**:
    
    - **Strategy:** Impose a total ordering (global numbering) of all resource types. Require that each process requests resources in an increasing order of enumeration.
        
        - _Example:_ Resources: 1. Scanner, 2. Plotter, 3. Tape Drive. A process can request Scanner then Tape Drive, but NOT Plotter then Scanner.
            
        - _Benefit:_ This prevents cycles in the RAG.
            
        - _Problem:_ Finding a suitable order can be difficult. May lead to inefficient resource utilization if a needed lower-numbered resource is available but cannot be requested because a higher-numbered one is already held.
            

## 🚦 Deadlock Avoidance

Goal: Make decisions dynamically to ensure the system never enters an unsafe state.

**Safe State Concept 🌟**:

- A state is **safe** if the system can allocate resources to each process (up to its maximum) in some order and still avoid a deadlock. There exists a **safe sequence** of processes <P1, P2, ..., Pn> such that for each Pi, the resources that Pi can still request can be satisfied by the currently available resources plus the resources held by all Pj, where j < i.
    
- A safe state is not a deadlocked state.
    
- A deadlocked state is an unsafe state.
    
- Not all unsafe states are deadlocks, but an unsafe state _may lead_ to a deadlock.
    
- The system grants a resource request only if the allocation leaves the system in a safe state.
    

**Example of Safe State:**

- System has 12 tape drives 📼.
    
- Processes:
    
    - P0: Max needs 10, Currently holds 5
        
    - P1: Max needs 4, Currently holds 2
        
    - P2: Max needs 9, Currently holds 2
        
- Available tape drives = 12 - (5+2+2) = 3.
    
- **Is this state safe?** Yes.
    
    - Sequence <P1, P0, P2> is a safe sequence:
        
        1. P1 needs 4-2=2 more. Available=3. Grant to P1. P1 finishes.
            
            Available = 3-2 (to P1) + 4 (P1 releases) = 5.
            
        2. P0 needs 10-5=5 more. Available=5. Grant to P0. P0 finishes.
            
            Available = 5-5 (to P0) + 10 (P0 releases) = 10.
            
        3. P2 needs 9-2=7 more. Available=10. Grant to P2. P2 finishes.
            
            Available = 10-7 (to P2) + 9 (P2 releases) = 12.
            
    - All processes can finish. ✅
        

**If P2 then requests 1 more tape drive (holds 3, needs 6 more):**

- Available = 3 - 1 = 2.
    
- P1 needs 2. Available=2. Grant to P1. P1 finishes.
    
    Available = 2-2 + 4 = 4.
    
- Now, P0 needs 5, P2 needs 6. Available=4. Neither can be satisfied.
    
- This is an **unsafe state**. ⚠️ The request from P2 should not be granted.
    

**Algorithms for Deadlock Avoidance:**

1. **Resource Allocation Graph Algorithm (Single Instance of Each Resource Type)**
    
    - Introduces a **claim edge** (dashed line Pᵢ → Rⱼ) indicating process Pᵢ _may_ request resource Rⱼ in the future.
        
    - When Pᵢ requests Rⱼ, the claim edge Pᵢ → Rⱼ becomes a request edge.
        
    - When Rⱼ is allocated to Pᵢ, the request edge becomes an assignment edge Rⱼ → Pᵢ.
        
    - A request is granted ONLY if converting the request edge to an assignment edge does NOT form a cycle in the RAG (including claim edges for unallocated resources).
        
    - _Example:_ If allocating R2 to P2 would create a cycle (even if R2 is free), the allocation is denied.
        
2. **Banker's Algorithm (Multiple Instances of Each Resource Type) 🏦**
    
    - Named because it's like a banker ensuring they don't allocate cash such that they can't satisfy all customers' needs.
        
    - Processes must declare their **maximum** resource needs in advance.
        
    - When a process requests resources, the system checks if granting the request will leave the system in a safe state. If yes, allocate; otherwise, wait.
        
    
    **Data Structures for Banker's Algorithm:**
    
    - `n`: number of processes, `m`: number of resource types.
        
    - `Available[m]`: Vector of available resources of each type. `Available[j] = k` means k instances of resource Rⱼ are available.
        
    - `Max[n][m]`: Matrix of maximum demand of each process. `Max[i][j] = k` means Pᵢ may request at most k instances of Rⱼ.
        
    - `Allocation[n][m]`: Matrix of resources currently allocated. `Allocation[i][j] = k` means Pᵢ is allocated k instances of Rⱼ.
        
    - `Need[n][m]`: Matrix of remaining resource needs. `Need[i][j] = Max[i][j] - Allocation[i][j]`.
        
    
    **Banker's Safety Algorithm (Checks if system is in a safe state):**
    
    1. Initialize `Work[m] = Available`, `Finish[n]` to `false` for all `i`.
        
    2. Find an index `i` such that:
        
        - `Finish[i] == false`
            
        - Needᵢ <= Work (Pᵢ's needs can be met by current Work resources)
            
            If no such i exists, go to step 4.
            
    3. Work = Work + Allocationᵢ (Assume Pᵢ finishes and releases its resources)
        
        Finish[i] = true
        
        Go to step 2.
        
    4. If Finish[i] == true for all i, the system is in a safe state. ✅ Otherwise, it's unsafe. ❌
        
        (This may take O(mn²) operations)*
        
    
    **Banker's Resource-Request Algorithm (Handles a request from Pᵢ for `Requestᵢ` resources):**
    
    5. If `Requestᵢ <= Needᵢ`, go to step 2. Otherwise, error (process exceeded max claim).
        
    6. If `Requestᵢ <= Available`, go to step 3. Otherwise, Pᵢ must wait (resources not available).
        
    7. **Pretend** to allocate:
        
        - `Available = Available - Requestᵢ`
            
        - `Allocationᵢ = Allocationᵢ + Requestᵢ`
            
        - `Needᵢ = Needᵢ - Requestᵢ`
            
    8. Run the **Safety Algorithm** on this new (pretend) state.
        
    9. If the new state is safe, complete the allocation. ✅
        
        If the new state is unsafe, Pᵢ must wait, and the old resource-allocation state is restored. ❌
        

## 🔎🛠️ Deadlock Detection and Recovery

If no prevention or avoidance is used, deadlocks can occur. The system needs:

1. An algorithm to determine if a deadlock has occurred.
    
2. An algorithm to recover from the deadlock.
    

**Detection Methods:**

1. **Wait-For Graph (Single Instance of Each Resource Type)**
    
    - Derived from the RAG by removing resource nodes and collapsing edges.
        
    - An edge Pᵢ → Pⱼ exists if Pᵢ is waiting for Pⱼ to release a resource.
        
    - A **cycle** in the wait-for graph indicates a deadlock.
        
    - Periodically invoke a cycle-detection algorithm (O(n²) operations, where n is #processes).
        
2. **Algorithm for Multiple Instances of Each Resource Type**
    
    - Similar to Banker's Safety Algorithm but uses `Request` matrix instead of `Need`. `Request[i][j]` is the current request of Pᵢ for Rⱼ.
        
    
    1. Initialize Work[m] = Available.
        
        For i = 0 to n-1: if Allocationᵢ != 0, Finish[i] = false. Else, Finish[i] = true.
        
        (Slight variation in PDF: if Requestᵢ != 0, then Finish[i]=false; otherwise, Finish[i]=true. This seems more aligned with detecting if a waiting process can proceed).
        
        Let's use the PDF's version for detection:
        
        Initialize Work[m] = Available.
        
        For i = 0 to n-1: if Allocationᵢ != 0, Finish[i] = false. Else, Finish[i] = true.
        
        (The PDF actually states: if Requesti != 0, then Finish[i]=false; otherwise, Finish[i]=true. This seems more logical for detection, as we're interested in processes that are actually requesting something. However, the standard detection algorithm often initializes Finish[i] = false if Allocation[i] is not zero, meaning the process is active and holding resources, and then checks if its Request can be satisfied.)
        
        Let's use a common version of the detection algorithm:
        
    2. Initialize Work[m] = Available.
        
        Finish[n] to false for all i.
        
        (For processes with no allocations, Allocationᵢ is zero. If Allocationᵢ is zero, they aren't part of a potential deadlock cycle in the same way, but the algorithm typically checks if any process can finish).
        
        Let's refine based on typical detection:
        
    3. Work = Available
        
        Finish[i] = false for all i.
        
        Let Request[n][m] be the current outstanding requests.
        
    4. Find an i such that Finish[i] == false AND Requestᵢ <= Work.
        
        If no such i, go to step 4.
        
    5. Work = Work + Allocationᵢ
        
        Finish[i] = true
        
        Go to step 2.
        
    6. If Finish[i] == false for some i, then the system is in a deadlocked state. 💀
        
        Processes Pᵢ for which Finish[i] == false are deadlocked.
        
        (This may take O(mn²) operations)*
        

**When to Invoke Detection?**

- Every resource request? (High overhead 💸)
    
- Less frequently? (e.g., once per hour, or when CPU utilization drops below a threshold like 40% 📉).
    

**Recovery from Deadlock:**

- **Process Termination:**
    
    - Abort all deadlocked processes (drastic! 💥).
        
    - Abort one process at a time until the deadlock cycle is eliminated (difficult choice of victim 🤔). Factors for victim selection: priority, how long executed, resources held, resources needed, how many other processes will be affected.
        
- **Resource Preemption:**
    
    - Forcibly take resources from some processes and give them to others until the deadlock is broken.
        
    - Issues:
        
        - **Victim selection:** Which resource from which process? Minimize cost.
            
        - **Rollback:** What to do with the process that lost a resource? Often requires rolling back to a safe state and restarting.
            
        - **Starvation:** Ensure the same process isn't always picked as a victim.