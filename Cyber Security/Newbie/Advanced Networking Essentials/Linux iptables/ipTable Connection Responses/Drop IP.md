To drop or block an IP address using iptables, you can add a rule to the appropriate chain (such as INPUT, FORWARD, or OUTPUT) that matches the IP address and uses the DROP target. This will cause any packets from or to that IP address to be silently dropped without any response.

Here's an example of an iptables rule to drop packets from a specific IP address:

```
iptables -A INPUT -s 192.168.0.10 -j DROP
```

In this rule, `-A INPUT` appends the rule to the INPUT chain. `-s 192.168.0.10` matches packets with a source IP address of 192.168.0.10. `-j DROP` specifies the DROP target, which drops the matched packets.

Similarly, if you want to drop packets to a specific IP address, you can use the `-d` option instead:

```
iptables -A OUTPUT -d 192.168.0.10 -j DROP
```

This rule appends the rule to the OUTPUT chain and drops packets with a destination IP address of 192.168.0.10.

Remember to adjust the IP address and the appropriate chain according to your specific needs. Additionally, be cautious when blocking IP addresses, as incorrect configuration can result in unintended consequences or blocking legitimate traffic.