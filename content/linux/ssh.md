# ssh

## ssh_config

add host to ssh config to be able to use `ssh HOST`, `sftp HOST`, etc.

```sh
Host HOST
  HostName $hostname
  User $user
  Port $port
```
