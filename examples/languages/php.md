---
runme:
  id: 01JC6V65TAV0EXKYSS511GK09X
  version: v3
---

## PHP

You can run Node code by setting the language of the cell to `PHP`. To set the binary manually, click `Configure`, goto the `Advanced` tab and set the interpreter to whatever you want, `/opt/homebrew/bin/php` for example.

```php {"id":"01JC6RX7NJSEA7XPBPW78Z88BC","interpreter":"","name":"php-greeting"}
<?php
// PHP Script Example: Greeting with Date and Time

// Define a variable for the greeting
$greeting = "Hello, World!";

// Get the current date and time
$currentDateTime = date('Y-m-d H:i:s');

// Concatenate the greeting with the current date and time
$fullGreeting = $greeting . " It's now " . $currentDateTime;

// Output the full greeting
echo $fullGreeting;
?>
```
