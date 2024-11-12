---
runme:
  id: 01JC6XSJ7Y46M62NK7XXHKYDWF
  version: v3
---

## Shell scripts

Doing day to day ops tasks with Shell Scrips.

```sh {"id":"01HTZB059ZFK301922XBD5B88R","interpreter":"bash","name":"shell-script","terminalRows":"20"}
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

log_results() {
    echo "Log Timestamp: $(date)"
    echo "-----------------------------------------"
    check_disk_usage
    echo "-----------------------------------------"
    check_memory_usage
    echo "-----------------------------------------"
    check_cpu_load
    echo "-----------------------------------------"
    echo "Log Ended"
}

log_results

```
