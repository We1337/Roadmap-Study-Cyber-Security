`airodump-ng` is a part of the Aircrack-ng suite, a set of tools for auditing wireless networks. `airodump-ng` is specifically designed for capturing and displaying information about wireless networks, including details about nearby access points (APs) and connected clients.

Here are some common commands and features associated with `airodump-ng`:

1. **Capture Wireless Network Information:**
   ```bash
   airodump-ng <interface>
   ```
   Replace `<interface>` with the name of your wireless interface. This command captures and displays information about nearby wireless networks.

2. **Specify a Capture File:**
   ```bash
   airodump-ng -w <output-file> <interface>
   ```
   This command allows you to specify an output file for storing the captured data. Replace `<output-file>` with the desired filename.

3. **Filter by BSSID (AP MAC Address):**
   ```bash
   airodump-ng --bssid <BSSID> -c <channel> -w <output-file> <interface>
   ```
   This command filters the capture to a specific AP (access point) using its BSSID (MAC address). Replace `<BSSID>` with the target AP's MAC address, `<channel>` with the channel number, and `<output-file>` with the desired filename.

4. **Filter by ESSID (Network Name):**
   ```bash
   airodump-ng --essid <ESSID> -c <channel> -w <output-file> <interface>
   ```
   This command filters the capture to a specific network using its ESSID (name). Replace `<ESSID>` with the target network's name, `<channel>` with the channel number, and `<output-file>` with the desired filename.

5. **Filter by Both BSSID and ESSID:**
   ```bash
   airodump-ng --bssid <BSSID> --essid <ESSID> -c <channel> -w <output-file> <interface>
   ```
   This command allows you to filter the capture based on both BSSID and ESSID.

6. **Show Client Information:**
   ```bash
   airodump-ng --bssid <BSSID> -c <channel> --showack -w <output-file> <interface>
   ```
   This command displays information about associated clients for a specific AP.

`airodump-ng` is commonly used in combination with other tools from the Aircrack-ng suite, such as `aireplay-ng` for packet injection and `aircrack-ng` for cracking WEP or WPA/WPA2 keys. As with any security tool, it's crucial to use `airodump-ng` responsibly and legally, obtaining proper authorization before testing or auditing any wireless networks. Unauthorized access to networks or systems is illegal, and ethical considerations should always be a priority.