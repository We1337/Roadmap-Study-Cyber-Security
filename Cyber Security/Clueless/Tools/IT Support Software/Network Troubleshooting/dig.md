Dig (short for "Domain Information Groper") is a command-line utility that is commonly used in Linux and Unix systems to query the Domain Name System (DNS). Dig is similar to the nslookup command in Windows, but provides more detailed information and additional options.

Here are some common dig commands:

1. dig [domain name]: This command looks up the IP address associated with the specified domain name.
2. dig [IP address]: This command looks up the domain name associated with the specified IP address.
3. dig -t [record type] [domain name]: This command looks up the specified type of DNS record for the specified domain name, such as MX (mail exchange), NS (name server), or SOA (start of authority).
4. dig +trace [domain name]: This command performs a full DNS resolution for the specified domain name, displaying the path of queries and responses from the root servers to the authoritative name servers for the domain.

By using dig, you can obtain detailed information about DNS records and the DNS resolution process, such as the IP address associated with a domain name, the mail exchange server for a domain, or the name servers responsible for a domain's DNS records. This information can be helpful for diagnosing DNS-related issues, troubleshooting network connectivity problems, and verifying domain name resolution.