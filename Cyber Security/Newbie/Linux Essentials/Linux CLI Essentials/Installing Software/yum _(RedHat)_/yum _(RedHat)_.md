`yum` (Yellowdog Updater, Modified) is the default package management tool used in Red Hat-based Linux distributions such as Red Hat Enterprise Linux (RHEL), CentOS, and Fedora. It is a high-level package management utility that simplifies the process of installing, updating, and removing software packages. Here are some commonly used `yum` commands:

1. Package Installation and Removal:
   - `sudo yum install <package>`: Install a package and its dependencies.
   - `sudo yum remove <package>`: Remove a package from the system.
   - `sudo yum erase <package>`: Remove a package and its dependencies.

2. Package Information and Querying:
   - `yum list`: List all available packages.
   - `yum info <package>`: Display detailed information about a specific package.
   - `yum search <keywords>`: Search for packages that match specified keywords.
   - `yum provides <file>`: Find the package that provides a specific file.

3. System Updates:
   - `sudo yum update`: Update all installed packages to their latest available versions.
   - `sudo yum upgrade`: Perform a system upgrade, including package installation, removal, and updates as necessary.
   - `sudo yum check-update`: Check for available package updates without installing them.

4. Repository Management:
   - `/etc/yum.repos.d/`: Directory containing repository configuration files. You can add or modify repository configurations in this directory.
   - `yum repolist`: List available repositories.
   - `yum-config-manager`: Manage repository configurations. Commands include enabling or disabling repositories, adding or removing repositories, etc.

5. Package Caching:
   - `yum clean packages`: Delete cached package files from the local repository cache.
   - `yum makecache`: Rebuild the local repository cache.

It's important to note that `yum` commands generally require administrative privileges, so `sudo` is typically used before executing `yum` commands. Additionally, the availability of certain commands and options may vary depending on the specific Red Hat-based distribution and version.

In recent versions of Red Hat-based distributions like Fedora 22 and CentOS/RHEL 8, `yum` has been replaced by `dnf` (Dandified Yum) as the default package manager. While `dnf` provides similar functionality to `yum`, it introduces some enhancements and improvements.

For more information and details on `yum` and its options, you can refer to the `yum` manual page by running `man yum` in the terminal.