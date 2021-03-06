# Bash Scripting Notes

## Special Variables
```bash
$0 - The name of the Bash script.
$1 - $9 - The first 9 arguments to the Bash script. (As mentioned above.)
$# - How many arguments were passed to the Bash script.
$@ - All the arguments supplied to the Bash script.
$? - The exit status of the most recently run process.
$$ - The process ID of the current script.
$USER - The username of the user running the script.
$HOSTNAME - The hostname of the machine the script is running on.
$SECONDS - The number of seconds since the script was started.
$RANDOM - Returns a different random number each time is it referred to.
$LINENO - Returns the current line number in the Bash script.
```

## Various notes
### Give execute permission to bash script
```bash
chmod 755 myscript.sh
```

### Quotes
Single quotes will treat every character literally
Double quotes will allow you to do substitution (that is include variables within the setting of the value)

```bash
myvar=$( ls /etc | wc -l )
echo $myvar
```