To parse and extract email addresses from a text using regular expressions, you can use the following regex pattern:

```regex
\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,}\b
```

Here's an example of how you can use this pattern in Python to extract email addresses from a text:

```python
import re

text = "Please contact me at john.doe@example.com or jane_smith123@gmail.com. Additional emails: info@example.com, support@company.com"
pattern = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,}\b"

matches = re.findall(pattern, text)
email_addresses = matches

print(email_addresses)
```

Output:
```
['john.doe@example.com', 'jane_smith123@gmail.com', 'info@example.com', 'support@company.com']
```

In this example, the `re.findall()` function is used with the regex pattern to find all occurrences of email addresses in the given text. The resulting matches are stored in the `matches` list, and then assigned to the `email_addresses` list for clarity. Finally, the extracted email addresses are printed.

Please note that the given regex pattern provides a basic approach to match email addresses in common formats. However, email address formats can vary, and the pattern may not capture all possible variations. It's important to keep in mind that fully validating an email address is a complex task that goes beyond the scope of regular expressions alone.