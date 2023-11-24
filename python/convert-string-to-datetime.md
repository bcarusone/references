# Convert String to Datetime

Source:: [How To Convert a String to a datetime or time Object in Python | DigitalOcean](https://www.digitalocean.com/community/tutorials/python-string-to-datetime-strptime)

- Monday is 0 and Sunday is 6

```python
from datetime import datetime

# strptime(date_string, format)
DATE = datetime.strptime("2022-09-14 15:03:17", '%Y-%m-%d %H:%M:%S')
```