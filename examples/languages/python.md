---
runme:
  id: 01JC6RWPJ7W7HKQ1XHT2C5V3A5
  version: v3
---

## Python

You can run Python code by setting the language of the cell to `Python`. To set the binary manually, click `Configure`, goto the `Advanced` tab and set the interpreter to whatever you want, `/usr/bin/python3` for example.

```python {"id":"01JC6RX7NJSEA7XPBPW78Z88BC","interpreter":"/usr/bin/python3","name":"python-greeting"}
import datetime

# Define a variable for the greeting
greeting = "Hello, World!"

# Get the current date and time
currentDateTime = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')

# Concatenate the greeting with the current date and time
fullGreeting = greeting + " It's now " + currentDateTime

# Output the full greeting
print(fullGreeting)
```
