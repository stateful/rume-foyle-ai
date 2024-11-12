---
runme:
  id: 01JC6VXZ7F7Z5PMKK3CXGEW4T9
  version: v3
---

## Envirment variables

Explore how to work with environment variables inside Notebook cells.

```bash {"id":"01HW167A4SWNJ0AQZGNZ1Z38XZ","name":"vars","promptEnv":"auto"}
$ export VAR_NAME1='Placeholder 1'
$ export VAR_NAME2="Placeholder 2"
$ export VAR_NAME3=""
$ export VAR_NAME4=Message

$ echo "1. ${VAR_NAME1}"
$ echo "2. ${VAR_NAME2}"
$ echo "3. ${VAR_NAME3}"
$ echo "4. ${VAR_NAME4}"
```

```bash {"id":"01HW1B541A9P8BVBJZJ4E1XV1F","name":"vars2","promptEnv":"no"}
$ export VAR_NAME5='Placeholder 5'
$ export VAR_NAME6='Placeholder 6'

$ echo "1. ${VAR_NAME1}"
$ echo "2. ${VAR_NAME2}"
$ echo "3. ${VAR_NAME3}"
$ echo "4. ${VAR_NAME4}"
$ echo "5. ${VAR_NAME5}"
$ echo "6. ${VAR_NAME6}"
```

Non-shell scripts can also access environment variables, and are run from the current working directory:

Export the following environment variable called **YOUR_NAME**

```sh {"id":"01HTZB059ZFK301922YMJNQ6RH","interactive":"false","promptEnv":"yes"}
export YOUR_NAME=enter your name
```

Run the following python script that reads the environment variable specified in the previous step:

```python {"id":"01HTZB059ZFK301922YNN12VKZ","interpreter":"/usr/bin/python3"}
import os

def main():
    your_name = os.environ.get("YOUR_NAME")
    print(f"Hello, {your_name}, welcome to Runme!")

if __name__ == "__main__":
    main()

```
