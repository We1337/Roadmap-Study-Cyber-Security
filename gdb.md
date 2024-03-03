GDB (GNU Debugger) is a powerful and widely used debugger for debugging programs on Unix-like systems, including Linux. It is a command-line tool that allows developers and reverse engineers to inspect and control the execution of programs, analyze their behavior, and identify and fix bugs. Here are some common uses of GDB:

1. **Launching a Program:**
   ```bash
   gdb <executable>
   ```
   This command starts GDB with the specified executable.

2. **Setting Breakpoints:**
   ```bash
   break <function>
   ```
   or
   ```bash
   break <line-number>
   ```
   This sets a breakpoint at a specific function or line number in the source code.

3. **Running the Program:**
   ```bash
   run
   ```
   This command runs the program until a breakpoint or until it completes.

4. **Stepping Through Code:**
   ```bash
   step
   ```
   This command executes the current line of code and stops at the first instruction of any called function.

   ```bash
   next
   ```
   This command executes the current line of code but does not step into any called functions.

5. **Continuing Execution:**
   ```bash
   continue
   ```
   This command continues the execution until the next breakpoint or until the program completes.

6. **Inspecting Variables:**
   ```bash
   print <variable>
   ```
   or
   ```bash
   p <variable>
   ```
   This command prints the current value of a variable.

7. **Backtrace:**
   ```bash
   backtrace
   ```
   or
   ```bash
   bt
   ```
   This command shows the current call stack.

8. **Changing Values:**
   ```bash
   set <variable> = <value>
   ```
   This command changes the value of a variable during program execution.

9. **Displaying Memory Content:**
   ```bash
   x/<format> <address>
   ```
   This command displays the memory content at a specific address using a specified format.

10. **Detaching from a Running Process:**
    ```bash
    detach
    ```
    This command detaches GDB from a running process, leaving the process running independently.

GDB is a powerful and flexible tool, and its capabilities extend beyond these basic commands. It's commonly used for both software development and reverse engineering tasks on Linux systems. Additionally, many integrated development environments (IDEs) provide GDB integration, offering a graphical interface for debugging.