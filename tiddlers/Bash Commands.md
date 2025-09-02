
## Tree Command
https://www.geeksforgeeks.org/tree-command-unixlinux/

List only PWD
```bash
tree --dirsfirst -L 1
```

## History Command

List of the top 10 commands you run most.
```bash
$ history | awk '{cmd[$2]++} END {for(elem in cmd) {print cmd[elem] " " elem}}' | sort -n -r | head -10
```