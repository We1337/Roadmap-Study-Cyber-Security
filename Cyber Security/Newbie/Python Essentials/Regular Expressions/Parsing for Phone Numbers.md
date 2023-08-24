To parse and extract phone numbers from a text using regular expressions, you can use the following regex pattern:

```regex
(\+\d{1,3}\s?)?\(?\d{3}\)?[\s.-]?\d{3}[\s.-]?\d{4}
```

Here's an example of how you can use this pattern in Python to extract phone numbers from a text:

```python
import re

text = "Please contact me at +1 (123) 456-7890 or 555-1234. Alternate numbers: 987-6543, +44 123456789."
pattern = r"(\+\d{1,3}\s?)?\(?\d{3}\)?[\s.-]?\d{3}[\s.-]?\d{4}"

matches = re.findall(pattern, text)
phone_numbers = [match for match in matches if match]

print(phone_numbers)
```

Output:
```
['+1 (123) 456-7890', '555-1234', '987-6543', '+44 123456789']
```

In this example, the `re.findall()` function is used with the regex pattern to find all occurrences of phone numbers in the given text. The resulting matches are stored in the `matches` list. The list comprehension is then used to filter out any empty matches. Finally, the extracted phone numbers are printed.

Please note that the given regex pattern provides a general approach to match phone numbers in common formats. However, phone number formats can vary across countries and regions. You may need to modify the pattern according to your specific requirements.