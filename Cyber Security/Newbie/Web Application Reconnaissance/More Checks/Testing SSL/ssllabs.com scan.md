To perform a scan of an SSL/TLS configuration using SSL Labs' SSL Server Test, follow these steps:

1. **Access SSL Labs' SSL Server Test**: Visit the SSL Labs website at [https://www.ssllabs.com/ssltest/](https://www.ssllabs.com/ssltest/).
2. **Enter the target server**: In the "Hostname" field, enter the domain or IP address of the server you want to scan.
3. **Start the scan**: Click on the "Submit" button to start the scan. SSL Labs will initiate the scan and analyze the SSL/TLS configuration of the target server. 
4. **Monitor the scan progress**: SSL Labs will perform a series of tests on the target server's SSL/TLS implementation. The progress of the scan will be displayed, and you can see the different stages of the assessment being performed.
5. **Review the scan results**: Once the scan is complete, SSL Labs will generate a detailed report summarizing the SSL/TLS configuration and security assessment of the target server. The report provides an overall grade, along with detailed information about supported protocols, cipher suites, certificate details, and potential vulnerabilities. 
    -   The report will also include a summary of any security issues found, categorized by severity.
    -   Each section of the report provides additional details and recommendations for improving the SSL/TLS configuration.
6. **Interpret the results**: Carefully review the scan results to identify any security vulnerabilities, misconfigurations, or weak points in the SSL/TLS configuration. Pay attention to critical issues, such as the use of insecure protocols or cipher suites, weak key exchange algorithms, or expired certificates.    
7. **Act on the recommendations**: Follow the recommendations provided in the SSL Labs report to address the identified vulnerabilities or weaknesses in the SSL/TLS configuration. Implement necessary changes, such as updating server settings, patching software, or renewing certificates, based on the recommendations.
8. **Rerun the scan**: After making the necessary changes, rerun the SSL Labs scan to validate the improvements in the SSL/TLS configuration. Ensure that the scan results reflect the desired security posture and compliance with best practices.

SSL Labs' SSL Server Test is a valuable tool for assessing SSL/TLS security, identifying vulnerabilities, and obtaining insights into the overall strength of the configuration. Regularly perform scans and follow up with remediation actions to maintain a secure SSL/TLS implementation.