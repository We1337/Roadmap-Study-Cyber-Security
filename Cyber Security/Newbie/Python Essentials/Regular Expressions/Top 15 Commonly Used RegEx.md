Sure! Here are 15 commonly used regular expressions (regex) patterns:

1. Email Validation:
```regex
^[\w.-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$ 
```

2. URL Validation:
```regex
^(https?|ftp):\/\/[^\s/$.?#].[^\s]*$ 
```

3. Password Validation (requires at least 8 characters with at least one uppercase letter, one lowercase letter, one digit, and one special character):
```regex
^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,}$ 
```

4. Numeric Input:
```regex
^[0-9]+$ 
```

5. Alphabetic Input:
```regex
^[A-Za-z]+$ 
```

6. Alphanumeric Input:
```regex
^[A-Za-z0-9]+$ 
```

7. Phone Number Validation (supports various formats):
```regex
^(\+\d{1,3}\s)?\(?\d{3}\)?[\s.-]?\d{3}[\s.-]?\d{4}$ 
```

8. Date Validation (matches dates in the format yyyy-mm-dd):
```regex
^\d{4}-\d{2}-\d{2}$ 
```

9. Time Validation (matches time in the format hh:mm:ss):
```regex
^([0-1]\d|2[0-3]):([0-5]\d):([0-5]\d)$ 
```

10. IP Address Validation:
```regex
^(?:[0-9]{1,3}\.){3}[0-9]{1,3}$ 
```

11. HTML Tag Matching (matches opening and closing HTML tags):
```regex
<([a-zA-Z][a-zA-Z0-9]*)\b[^>]*>(.*?)<\/\1> 
```

12. Credit Card Number Validation (supports major card types):
```regex
^(?:4[0-9]{12}(?:[0-9]{3})?|5[1-5][0-9]{14}|6(?:011|5[0-9][0-9])[0-9]{12}|3[47][0-9]{13}|3(?:0[0-5]|[68][0-9])[0-9]{11}|(?:2131|1800|35\d{3})\d{11})$ 
```

13. Social Security Number Validation (matches the format xxx-xx-xxxx):
```regex
^\d{3}-\d{2}-\d{4}$ 
```

14. ZIP Code Validation (supports both 5-digit and 5-digit+4 formats):
```regex
^\d{5}(?:[-\s]\d{4})?$ 
```

15. Username Validation (allows letters, numbers, underscores, and dots, between 3 and 20 characters):
```regex
^[a-zA-Z0-9_.]{3,20}$ 
```

Please note that regex patterns can vary depending on the specific requirements and constraints of your use case. It's recommended to test and adapt the patterns as needed.