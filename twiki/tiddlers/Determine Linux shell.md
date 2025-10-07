You can type the following command in your terminal to see which shell you are using:   
```
echo $0
sh -c 'ps -p $$ -o ppid=' | xargs -I'{}' readlink -f '/proc/{}/exe'
```