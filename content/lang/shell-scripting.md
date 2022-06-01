# shell scripting

because i always forget these things.

most of these maybe arent posix shell compatible.

## script options
* `set -u` catch unbound variables
* `set -e` exit on error
* `set -x` verbose 'debug' output
* `set -o pipefail` exit when theres an error in a pipe
* i mostly use `set -eu -o pipefail`

by default bash doesnt expand aliases in scripts. fix:
```sh
shopt -s expand_aliases
alias sed=/usr/local/bin/sed-v48
# you can now just write sed instead of the full path to sed-v48
```

## special variables
* `$1,$2,...$N` the n-th cli argument. `$0` is program name
* `$@` cli args as array
* `$?` exit code of last command

## templates
switch case based on cli args
```sh
case $1 in
  ab)
    echo ab
    ;;
  bc)
    echo bc
    ;;
  *)
    echo default
    ;;
esac
```

for each loop
```sh
for elem in "${ARRAY[@]}"; do
  if XYZ; then
    echo hello
  fi
done
```

c style for loop
```sh
for (( i=0; i<${#ARRAY[@]}; i++ )); do
	printf "[%d] %s\n" "$i" "${ARRAY[$i]}"
done
```

map something to an array
```sh
mapfile -t results <<< $(curl domain.tld | grep | sed | sort)
```

## bashisms

until service restart loop

TODO

