`rpm` (RPM Package Manager) is a command-line package management utility used in Red Hat-based Linux distributions, such as Red Hat Enterprise Linux (RHEL), CentOS, and Fedora. It is used for installing, querying, verifying, and managing software packages in RPM format. Here are some commonly used `rpm` commands:

1. Package Installation:
   - `rpm -i <package.rpm>`: Install a package from an RPM file.
   - `rpm -ivh <package.rpm>`: Install a package with verbose output and progress information.
   - `rpm --nodeps -i <package.rpm>`: Install a package ignoring dependencies.

2. Package Querying:
   - `rpm -q <package>`: Query if a package is installed.
   - `rpm -qi <package>`: Show information about an installed package.
   - `rpm -ql <package>`: List files installed by a package.
   - `rpm -qa`: List all installed packages.
   - `rpm -qf <file>`: Find the package that owns a specific file.

3. Package Removal:
   - `rpm -e <package>`: Remove an installed package.
   - `rpm -ev <package>`: Remove a package and its configuration files.
   - `rpm --nodeps -e <package>`: Remove a package ignoring dependencies.

4. Package Verification:
   - `rpm -V <package>`: Verify the integrity of an installed package.
   - `rpm -Va`: Verify all installed packages.
   - `rpm -Vp <package.rpm>`: Verify an RPM file before installation.

5. Package Information:
   - `rpm -qp <package.rpm>`: Show information about an RPM file without installing it.
   - `rpm -qa --last`: List recently installed packages.

6. Package Signing:
   - `rpm --import <keyfile>`: Import a GPG key for package verification.
   - `rpm --checksig <package.rpm>`: Check the signature of an RPM file.

It's important to note that `rpm` does not handle dependency resolution automatically like higher-level package managers (`yum`, `dnf`). Therefore, manually managing dependencies when using `rpm` can be complex and error-prone. It's generally recommended to use `yum` or `dnf` for package management in Red Hat-based distributions, as they handle dependencies and repository management more effectively.

When working with `rpm`, using the appropriate command-line options and ensuring administrative privileges (using `sudo`) is necessary to perform operations that modify the system.

For more information and details on `rpm` and its options, you can refer to the `rpm` manual page by running `man rpm` in the terminal.