# Producer-Consumer Data Processing System in C

## Introduction
Welcome to the Producer-Consumer Data Processing System project! This system is an implementation of the classic Producer-Consumer problem, a fundamental concept in computer science, realized through inter-process communication in C. The project is designed to demonstrate efficient data exchange between a producer and a consumer using shared memory and semaphores for synchronization. It's an excellent showcase of practical system programming, concurrency control, and inter-process communication mechanisms.

## Features
- **Efficient Inter-Process Communication:** Utilizes shared memory for fast and effective data transfer between the producer and consumer processes.
- **Semaphore-Based Synchronization:** Ensures safe and synchronized access to the shared circular queue with semaphores, avoiding data corruption and race conditions.
- **Circular Queue Management:** Implements a circular queue for buffering data, demonstrating queue management and memory utilization.
- **System-Level Programming:** Offers a deep dive into system calls and low-level programming in C, providing a hands-on experience with operating system concepts.

## How It Works
- **Producer Module (`producer50.c`):** Reads data from a source file, processes it, and places it into a shared circular queue. It uses semaphores to manage access to the queue and ensure data isn't overwritten before consumption.
- **Consumer Module (`consumer50.c`):** Retrieves data from the circular queue, processes it, and writes it to a destination file. It also utilizes semaphores to ensure synchronized access.
- **Shared Resources & Synchronization (settings1.h):** The header file defines the structure of the circular queue, buffer sizes, semaphore keys, and file names for input and output. It plays a pivotal role in ensuring that both producer and consumer have a consistent view of the shared resources.


## Requirements
- C Compiler (e.g., GCC)
- Basic understanding of inter-process communication and semaphores in C.

## Setup and Execution
1. Clone the repository or download the source files.
2. Compile the source files using a C compiler. For example, `gcc producer50.c -o producer` and `gcc consumer50.c -o consumer`.
3. Run the compiled executables in your terminal or command prompt.

## Contributing
Feel free to fork this project, submit pull requests, or suggest improvements. Your contributions are highly appreciated!

## Technologies Used:
- Language: C
- IPC mechanisms: Shared memory, semaphores.
