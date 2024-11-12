---
runme:
  id: 01JC6TNBFG5HPJEV6Z86R4FVSG
  version: v3
---

## Ruby

You can run Ruby code by setting the language of the cell to `Ruby`. To set the binary manually, click `Configure`, goto the `Advanced` tab and set the interpreter to `/usr/bin/ruby` for example.

```ruby {"id":"01JC6RX7NJSEA7XPBPW78Z88BC","name":"ruby-greeting"}
# Define a variable for the greeting
greeting = "Hello, World!"

# Get the current date and time
currentDateTime = Time.now.strftime("%Y-%m-%d %H:%M:%S")

# Concatenate the greeting with the current date and time
fullGreeting = "#{greeting} It's now #{currentDateTime}"

# Output the full greeting
puts fullGreeting
```
