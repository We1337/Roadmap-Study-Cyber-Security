Inspecting logs is an important task for troubleshooting and monitoring system behavior in Linux. Logs provide valuable information about various system activities, errors, and events. Here are some commonly used log inspection methods and tools in Linux:

1. Log File Locations:
   - `/var/log`: Most log files are stored in this directory.
   - `/var/log/syslog` or `/var/log/messages`: General system log files containing messages from different services and applications.
   - `/var/log/auth.log` or `/var/log/secure`: Authentication-related logs, including login attempts and authentication failures.
   - `/var/log/dmesg`: Kernel ring buffer containing information about hardware, device drivers, and system boot messages.
   - Application-specific log files: Many applications maintain their own log files in locations such as `/var/log/<application_name>`.

2. Viewing Log Files:
   - `cat <log_file>`: Display the entire content of a log file.
   - `less <log_file>`: View log files page by page, allowing scrolling and searching.
   - `tail <log_file>`: Display the last few lines of a log file.
   - `tail -f <log_file>`: Monitor a log file in real-time, showing new lines as they are appended.

3. Filtering Log Entries:
   - `grep <pattern> <log_file>`: Search for specific patterns or keywords within a log file.
   - `egrep "<pattern1>|<pattern2>" <log_file>`: Search for multiple patterns using regular expressions.
   - `zgrep <pattern> <compressed_log_file>`: Search within compressed log files (e.g., `.gz` files).

4. Log Analysis Tools:
   - `journalctl`: Query and view logs from the systemd journal.
   - `dmesg`: Display kernel ring buffer messages.
   - `tail` and `grep` combinations: Combine these commands to filter log entries in real-time or from log files.

5. Log Rotation and Archiving:
   - Log files are often rotated and compressed to conserve disk space. Compressed log files may have a `.gz` or `.bz2` extension. The original log file is typically renamed or moved to a new location.
   - Use the `logrotate` tool to manage log rotation policies and configuration.

6. System Log Monitoring Tools:
   - `rsyslog`: A system logging daemon that can forward logs to remote systems and provides advanced log management capabilities.
   - `syslog-ng`: Another popular system logging daemon with enhanced features for log collection and distribution.

7. Graphical Log Viewers:
   - Linux distributions may provide graphical log viewer applications, such as GNOME Logs or KSystemLog, which offer a user-friendly interface for browsing and searching log files.

Remember, log files can contain sensitive information, so it's crucial to consider security and access controls when inspecting log files. It's recommended to review log files with appropriate permissions and only grant access to trusted users or administrators.

Additionally, the specific log files and their locations may vary depending on your Linux distribution and the services installed on your system. It's always a good idea to refer to the documentation or manual pages specific to your distribution for more detailed information about log files and their locations.