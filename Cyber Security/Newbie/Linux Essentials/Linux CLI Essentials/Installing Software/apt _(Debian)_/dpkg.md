`dpkg` is a low-level package management command-line tool in Debian-based Linux distributions. It is used to perform operations on individual Debian packages (`.deb` files) and manage the package database. Here are some commonly used commands and options with `dpkg`:

1. Installation and Removal:
   - `sudo dpkg -i <package.deb>`: Install a `.deb` package.
   - `sudo dpkg -r <package>`: Remove a package (leaving configuration files intact).
   - `sudo dpkg -P <package>`: Purge a package, removing it along with its configuration files.
   - `sudo dpkg --configure <package>`: Configure a partially installed package.

2. Querying and Listing:
   - `dpkg -l`: List all installed packages.
   - `dpkg -l <pattern>`: List packages matching a specific pattern.
   - `dpkg -s <package>`: Show information about a specific package.
   - `dpkg -L <package>`: List files installed by a package.
   - `dpkg -S <file>`: Find the package owning a specific file.

3. Package Information:
   - `dpkg -I <package.deb>`: Display information about a `.deb` package.
   - `dpkg -c <package.deb>`: List the contents of a `.deb` package.
   - `dpkg --contents <package.deb>`: List the contents of a `.deb` package (alternative option).

4. Package Database Maintenance:
   - `sudo dpkg --configure -a`: Configure all unpacked but unconfigured packages.
   - `sudo dpkg-reconfigure <package>`: Reconfigure an installed package.
   - `sudo dpkg --clear-avail`: Clear the available package database cache.
   - `sudo dpkg --clear-selections`: Clear the package selection states.

5. Troubleshooting:
   - `sudo dpkg --audit`: Perform a consistency check on the package system.
   - `sudo dpkg --get-selections`: Get the status of installed packages.

It's important to note that `dpkg` does not handle dependency resolution like higher-level package managers (`apt`, `apt-get`). Therefore, it is often recommended to use `dpkg` in conjunction with other package management tools for proper dependency handling.

When working with `dpkg`, using `sudo` is necessary to run commands with administrative privileges. Additionally, be cautious when removing or purging packages, as it may impact the functionality of your system.

For more details and options, you can refer to the `dpkg` manual page by running `man dpkg` in the terminal.