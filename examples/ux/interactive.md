---
runme:
  id: 01JC6XYGC75BAS0VZ7SEYQ66YJ
  version: v3
---

### Interactive shell script

You can write interactive (Stdin) programs too without leaving your Markdown file!
Since this is a long running process, ensure we've marked the cell as a background process, otherwise the cell execution will block the Notebook UX, you can configure that at the cell level configuration section, check the background option from the advanced tab. [Learn more here](https://docs.runme.dev/configuration/cell-level#handle-long-running-processes).

Feel free to run the following shell script example, it's similar to the above example with the main difference is now interactive!, it will give you the following information about your system:

- Disk usage
- Memory usage
- CPU load

```sh {"background":"true","id":"01HTZB059ZFK301922XDGZZNQ0","interpreter":"bash","name":"interactive-shell-script","terminalRows":"25"}
check_disk_usage() {
    echo "Disk Usage:"
    df -h
}

check_memory_usage() {
    echo "Memory Usage:"
    top -l 1 -s 0 | grep PhysMem | sed 's/, /\n         /g'
}

check_cpu_load() {
    echo "CPU Load:"
    uptime
}

display_menu() {
  echo -e "_________________________________________________________________\n"
  echo "Hello! What operation you want to perform? (press ctrl+c to exit)"
  echo "1. Memory Usage"
  echo "2. Disk Usage"
  echo "3. CPU Load"
  echo -e "_________________________________________________________________\n"
  echo "Type the option number and hit enter"
}

# Function to handle Ctrl+C
ctrl_c_handler() {
    echo "Exiting..."
    exit 0
}

# Trap Ctrl+C signal
trap ctrl_c_handler SIGINT

while true; do
  display_menu
  read option

  case $option in
      1)
          echo " >> You selected: Memory Usage"
          check_memory_usage
          ;;
      2)
          echo " >> You selected: Disk Usage"
          check_disk_usage
          ;;
      3)
          echo " >> You selected: CPU Load"
          check_cpu_load
          ;;
      *)
          echo "Invalid option selected!"
          ;;
  esac
done
```
