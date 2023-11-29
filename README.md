# apache-log-parser

This Bash script parses Apache access log files and provides information about unique IP addresses, URLs, and user agents.

## Usage

```bash
./parse_apache_logs.sh [options]
```

## Options
```
-ua: List all user-agents and the number of times they connected.
-ip: Show all unique IP addresses and the number of times they connected.
-urls: Show all unique URLs.
-a: Perform all of the above actions.
-f <file>: Specify the path to the Apache access log file. (Default: access.log)
-o <file>: Save the output to the specified file.
-h: Show help menu.
```

# Show user-agents and IPs from the default log file
./parse_apache_logs.sh -ua -ip

# Show all information from a specific log file and save to output.txt
./parse_apache_logs.sh -a -f /path/to/access.log -o output.txt
