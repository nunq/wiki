# wifi auto signon

runs on my raspberry pi

### init.sh (@reboot in crontab)
```sh
/usr/bin/tmux new-session -d -s ENTER
/usr/bin/tmux detach -s ENTER
sleep 3
/usr/bin/tmux send-keys -t 0 "cd /home/alarm;./wifi.sh" ENTER
```

### wifi.sh
```sh
#!/bin/bash
set -eu -o pipefail

until sshpass [...] ; do
  echo -e "crashed $? at $(date)\n"
  sleep 5
done
```
