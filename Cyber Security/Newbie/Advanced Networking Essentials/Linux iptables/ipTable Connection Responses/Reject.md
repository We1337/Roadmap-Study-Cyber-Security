To reject network connections using iptables, you can add a rule to the appropriate chain (such as INPUT, FORWARD, or OUTPUT) that matches the desired criteria and uses the REJECT target. This will send an error response back to the source, indicating that the connection is not allowed.

Here's an example of an iptables rule to reject incoming ICMP echo requests (ping) and send an ICMP "Destination Unreachable" response:

```
iptables -A INPUT -p icmp --icmp-type echo-request -j REJECT
```

In this rule, `-A INPUT` appends the rule to the INPUT chain. `-p icmp` matches ICMP packets. `--icmp-type echo-request` matches ICMP echo requests (ping). `-j REJECT` specifies the REJECT target, which rejects the matched packets and sends an ICMP "Destination Unreachable" response.

Similarly, you can reject other types of connections by modifying the protocol, port, or any other relevant criteria.

It's important to note that when configuring iptables rules, the rules are processed sequentially from top to bottom. Make sure to place your reject rules before any subsequent rules that might accept or drop the same packets.

Remember to consider the security implications and use rejection sparingly. It's generally recommended to use reject for specific cases where you want to inform the source about the connection rejection. For general blocking or dropping, the DROP target is often preferred.