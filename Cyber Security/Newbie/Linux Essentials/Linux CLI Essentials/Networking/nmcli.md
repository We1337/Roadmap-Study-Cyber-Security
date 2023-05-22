`nmcli` is a command-line tool used for managing NetworkManager, which is a service that provides network connectivity and configuration on Linux systems. `nmcli` allows you to control and monitor network connections, wireless networks, IP addressing, DNS settings, and more. Here are some common uses of `nmcli`:

1. Viewing Network Connections:
   - `nmcli connection show`: Show all available network connections and their settings.
   - `nmcli connection show <connection-name>`: Show details of a specific network connection.

2. Creating and Modifying Network Connections:
   - `nmcli connection add`: Add a new network connection.
   - `nmcli connection modify <connection-name>`: Modify the settings of an existing network connection.
   - `nmcli connection delete <connection-name>`: Delete a network connection.

3. Managing Wireless Networks:
   - `nmcli device wifi list`: List available wireless networks.
   - `nmcli device wifi connect <SSID>`: Connect to a specific wireless network.
   - `nmcli device wifi connect <SSID> password <password>`: Connect to a password-protected wireless network.
   - `nmcli radio wifi on`: Enable Wi-Fi.
   - `nmcli radio wifi off`: Disable Wi-Fi.

4. Managing IP Addressing and DNS:
   - `nmcli connection modify <connection-name> ipv4.method <method>`: Set the IPv4 addressing method for a connection (e.g., "auto", "manual", "dhcp").
   - `nmcli connection modify <connection-name> ipv4.address <IP>/<subnet>`: Set a static IPv4 address and subnet mask for a connection.
   - `nmcli connection modify <connection-name> ipv4.gateway <IP>`: Set the IPv4 gateway for a connection.
   - `nmcli connection modify <connection-name> ipv4.dns <IP>`: Set the IPv4 DNS server(s) for a connection.

5. Managing Network Status:
   - `nmcli general status`: Display the overall NetworkManager status.
   - `nmcli device status`: Show the status of network devices (e.g., connected, disconnected).
   - `nmcli device reapply <device>`: Reapply the configuration for a specific network device.

6. Network Troubleshooting:
   - `nmcli device show <device>`: Show detailed information about a network device.
   - `nmcli connection down <connection-name>`: Take down a specific network connection.
   - `nmcli connection up <connection-name>`: Bring up a specific network connection.

These are just a few examples of what you can do with `nmcli`. The tool provides a wide range of options and commands to manage network connections, wireless networks, IP addressing, DNS, and more. For detailed usage instructions and additional options, you can refer to the `nmcli` manual page by running `man nmcli` in the terminal.