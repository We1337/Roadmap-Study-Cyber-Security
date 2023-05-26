In computer programming, a system call, often abbreviated as SYSCALL, is a mechanism that allows a program to request services from the operating system kernel. It acts as an interface between user-level processes and the underlying operating system, providing a way to perform privileged operations and access system resources.

System calls are typically used for tasks that require elevated privileges or interactions with the underlying hardware and operating system. Some common examples of system calls include:

1. File system operations: System calls like open, read, write, and close are used to interact with files and directories.

2. Process management: System calls such as fork, exec, and exit are used to create and manage processes.

3. Network operations: System calls like socket, bind, connect, and send are used for network communication.

4. Interprocess communication (IPC): System calls like pipe, message queues, and shared memory allow processes to communicate with each other.

5. Memory management: System calls like malloc and free allocate and deallocate memory for programs.

6. Device control: System calls like ioctl allow programs to control and configure devices such as printers, sound cards, and network interfaces.

The specific set of system calls available depends on the operating system being used. Different operating systems have their own system call interfaces and conventions. The details of how system calls are invoked, the parameters they accept, and the values they return are defined by the operating system's application programming interface (API).