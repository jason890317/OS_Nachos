# Operating System- Nachos

This directory contains detailed reports documenting the implementation, design decisions, and verification for various assignments in the **Operating Systems** course. Below is an overview of each assignment report:

---

## **MP1 Report: System Call Implementation**
- **Focus**: Implementation of four I/O system calls (`Open`, `Read`, `Write`, `Close`).
- **Key Sections**:
  1. **Trace Codes**: Detailed execution flow for `SC_Halt`, `SC_Create`, and `SC_PrintInt` system calls.
  2. **Verification**: Demonstrated working test cases for `fileIO_test1` and `fileIO_test2`.
  3. **Implementation Details**:
     - Enhanced system call stubs (`Start.S`, `Syscall.h`).
     - Modified file system operations (`filesys.h`) to handle `OpenAFile`, `WriteFile`, `ReadFile`, and `CloseFile`.
     - Integrated system calls into `exception.cc` for handling I/O operations.
  4. **Difficulties**: Challenges in tracing NachOS codebase and debugging system call integration.

---

## **MP2 Report: Multiprogramming**
- **Focus**: Implementation of multiprogramming capabilities.
- **Key Sections**:
  1. **Trace Codes**: Explained the kernel and thread management processes, including:
     - `Kernel::ExecAll`, `AddrSpace::Load`, `Thread::Fork`, `Scheduler::Run`.
  2. **Verification**: Demonstrated simultaneous execution of multiple user programs.
  3. **Implementation Details**:
     - Introduced `UsedFrames` and `FreePages` in `Kernel` to manage physical memory frames.
     - Enhanced `AddrSpace::Load` to handle page table initialization and memory mapping dynamically.
     - Added exception handling for memory limit violations (`MemoryLimitException`).
  4. **Difficulties**: Addressed challenges in understanding and modifying thread, program, and memory interactions.

---

## **MP3 Report: Virtual Memory**
- **Focus**: Implementation of virtual memory management.
- **Key Sections**:
  1. **Trace Codes**: Explained memory page handling, page faults, and TLB operations.
  2. **Verification**: Tested virtual memory performance under different scenarios.
  3. **Implementation Details**:
     - Added a page replacement policy.
     - Integrated TLB handling for efficient memory access.
     - Enhanced exception handling for page faults.
  4. **Difficulties**: Overcame issues in synchronizing TLB and page table states.

---

## **MP4 Report: File System**
- **Focus**: Development of a file system to support basic file operations.
- **Key Sections**:
  1. **Trace Codes**: Explained how file metadata, directories, and disk space management are handled.
  2. **Verification**: Validated the file system through test cases involving multiple file operations.
  3. **Implementation Details**:
     - Designed data structures for file allocation tables and directory management.
     - Implemented space allocation and file recovery mechanisms.
  4. **Difficulties**: Debugged race conditions and ensured consistency during simultaneous file operations.

---

## **Pthreads Report**
- **Focus**: Implementation of threading using Pthreads.
- **Key Sections**:
  1. **Trace Codes**: Outlined thread creation, synchronization, and scheduling mechanisms.
  2. **Verification**: Validated thread synchronization through test cases involving mutexes and condition variables.
  3. **Implementation Details**:
     - Designed thread-safe data structures.
     - Enhanced performance with efficient thread pooling and resource allocation.
  4. **Difficulties**: Addressed deadlock scenarios and optimized thread management.

---

## **Usage**
- Each report provides an in-depth understanding of the design, implementation, and verification steps taken to accomplish specific objectives in the Operating Systems course.
- Use these reports as references for learning and for troubleshooting similar assignments.

## **Team Contributions**
- **Team Members**:
  - 許峻源 (111062649)  [Chun-Yuan Hsu]
  - 楊宗諺 (108022138)
  
- **Roles**:
  - Both members collaborated on all assignments, shared the workload evenly, and contributed to writing and debugging code.

---


