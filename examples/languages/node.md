---
runme:
  id: 01JC6V65TAV0EXKYSS511GK09X
  version: v3
---

## Node

You can run Node code by setting the language of the cell to `Babel JavaScript`. To set the binary manually, click `Configure`, goto the `Advanced` tab and set the interpreter to whatever you want, `/usr/bin/nodejs` for example.

```javascript {"id":"01JC6RX7NJSEA7XPBPW78Z88BC","name":"node-greeting"}
// Import the 'child_process' module
const { exec } = require('child_process');

// Define the command to execute (cross-platform)
const command = process.platform === 'win32' ? 'dir' : 'ls';

// Execute the command
exec(command, (error, stdout, stderr) => {
  if (error) {
    console.error(`Error executing command: ${error.message}`);
    return;
  }

  if (stderr) {
    console.error(`Standard error: ${stderr}`);
    return;
  }

  // Output the result of the command
  console.log(`Command output:\n${stdout}`);
});
```
