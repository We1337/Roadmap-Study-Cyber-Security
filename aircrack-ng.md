`aircrack-ng` is a part of the Aircrack-ng suite, which is a set of tools used for auditing and testing the security of wireless networks. `aircrack-ng` is specifically focused on the task of cracking WEP and WPA/WPA2-PSK keys. It works by analyzing captured data packets and attempting to recover the original key used to encrypt the wireless network.

Here are some common commands and features associated with `aircrack-ng`:

1. **Crack WEP Key:**
   ```bash
   aircrack-ng -b <BSSID> -e <ESSID> <capture-file>
   ```
   Replace `<BSSID>` with the target AP's MAC address, `<ESSID>` with the network name, and `<capture-file>` with the name of the file containing the captured data packets.

2. **Crack WPA/WPA2-PSK Key:**
   ```bash
   aircrack-ng -w <wordlist-file> -b <BSSID> <capture-file>
   ```
   Replace `<wordlist-file>` with the path to a wordlist containing potential passwords, `<BSSID>` with the target AP's MAC address, and `<capture-file>` with the name of the file containing the captured data packets.

3. **Crack WPA/WPA2-PSK Key with a Specific Handshake:**
   ```bash
   aircrack-ng -w <wordlist-file> -b <BSSID> -e <ESSID> -l <output-file> <capture-file>
   ```
   This command is similar to the previous one but allows you to specify an output file for the key. Replace `<output-file>` with the desired filename.

4. **Crack WPA/WPA2-PSK Key Using PMKID:**
   ```bash
   aircrack-ng -w <wordlist-file> -b <BSSID> -e <ESSID> -K <PMKID-file>
   ```
   If you have a PMKID file obtained separately, you can use this command to attempt to crack the WPA/WPA2-PSK key.

Remember that using `aircrack-ng` to attempt to crack wireless keys should only be done on networks for which you have explicit authorization. Unauthorized access to networks or systems is illegal, and ethical considerations should always be a priority. Additionally, using strong and unique passwords for wireless networks is crucial to prevent unauthorized access and potential attacks.