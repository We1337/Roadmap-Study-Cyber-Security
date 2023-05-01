`ltrace` is a command-line utility in Unix and Unix-like operating systems that is used to trace library calls made by a running program. It works by intercepting and logging the library calls made by a program and displaying them in a human-readable format.

When run on a program, the `ltrace` utility logs every library call made by the program, along with any associated arguments and return values. This can be useful for debugging programs, as it allows developers to see exactly which library functions a program is calling and how it is using them.

In addition to logging library calls, `ltrace` also includes a number of options that can be used to control its behavior. For example, the `-c` option can be used to generate a summary of library calls made by a program, and the `-e` option can be used to filter the library calls that are logged.

Overall, `ltrace` is a powerful tool for working with library calls in Unix and Unix-like systems, and it is commonly used by system administrators, developers, and security professionals. However, it should be used with caution, as tracing library calls can have a performance impact on running programs.