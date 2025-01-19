#### A music palyer that writen in shell scripting 

- This music palyer is bind of cava and mpg123 so for runing it you need this 2 tools

> [! note]
> If you dont have any other config for cava just copy until the 13 line of code 

```shell
#!/usr/bin/bash

cleanup() {
    killall mpg123 2>/dev/null
    clear
    exit 0
}

# Trap Ctrl+C to run cleanup
trap cleanup SIGINT

mpg123 -q -z ~/visk/* & 


option1="cava"
option2="cava -p ~/.config/cava/cyan"

random_number=$(( RANDOM % 2 ))

if [ $random_number -eq 0 ]; then
    eval $option1
else
    eval $option2
fi
```