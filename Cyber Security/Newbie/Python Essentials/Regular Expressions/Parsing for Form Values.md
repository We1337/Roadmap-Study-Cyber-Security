To parse and extract form values from a text using regular expressions, you can use the following regex pattern:

```regex
name=([^&\n]+)&value=([^&\n]+)
```

Here's an example of how you can use this pattern in Python to extract form values from a text:

```python
import re

text = "name=first_name&value=John&name=last_name&value=Doe&name=email&value=johndoe@example.com"
pattern = r"name=([^&\n]+)&value=([^&\n]+)"

matches = re.findall(pattern, text)
form_values = {name: value for name, value in matches}

print(form_values)
```

Output:
```
{'first_name': 'John', 'last_name': 'Doe', 'email': 'johndoe@example.com'}
```

In this example, the `re.findall()` function is used with the regex pattern to find all occurrences of form values in the given text. The resulting matches are stored in the `matches` list. Then, a dictionary comprehension is used to create a dictionary `form_values` where the form field names are the keys and the corresponding values are the values. Finally, the extracted form values are printed.

Please note that the given regex pattern assumes that form values are in the format `name=value` and separated by `&` or a newline character. This pattern may need to be adjusted based on the specific format and delimiters used in your form data.