#xv6 Toy OS
This project is an enhanced version of the xv6 Toy OS, featuring multiple improvements and custom implementations designed to optimize synchronization, scheduling, and memory management.

Features
1. Thread Synchronization
Threads: Implemented support for threads within the OS.
Spinlocks: Used spinlocks to ensure mutual exclusion in critical sections.
Mutexes: Added mutexes to handle more complex synchronization scenarios, avoiding the pitfalls of spinlocks.
2. Process Information System Calls
Developed system calls to fetch detailed information about active processes running in the OS, improving the visibility and management of tasks.
3. Hybrid Scheduling Algorithm
Shortest Job First (SJF): Optimized CPU-bound tasks by implementing the SJF algorithm, minimizing the waiting time for processes.
Round Robin: Integrated a Round Robin scheduling mechanism for fair allocation of CPU time slices to processes, especially effective for I/O-bound tasks.
Hybrid Model: Combined SJF and Round Robin scheduling to create a balanced approach, suitable for both CPU and I/O-bound tasks.
4. Memory Management
Lazy Memory Allocation: Incorporated a lazy memory allocation strategy to delay allocation until necessary, reducing memory usage.
Dynamic Paging with LRU: Integrated dynamic paging with a Least Recently Used (LRU) page replacement mechanism, optimizing the management of active processes' memory.
Installation
Clone the repository:

sh
Copy code
git clone [your-git-link]
cd xv6-OS-main
Build the OS:

sh
Copy code
make
Run the OS in a QEMU emulator:

sh
Copy code
make qemu
Usage
After booting into the OS, you can test the various features like thread creation, scheduling, and memory management using the provided system calls and utilities.
Contributions
Feel free to contribute to this project by forking the repository, making changes, and submitting a pull request. All contributions are welcome!

License
This project is licensed under the MIT License. See the LICENSE file for details.
