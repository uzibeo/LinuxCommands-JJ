## Linux Commands Cheat Sheet

### Simple Commands
|Command|Description|
|---|---|
|`ll`|list files & directories, "long list", same as ls -l|
|`mv`|move file|
|`cp`|copy file|
|`mkdir`|create new directory/folder|
|`chmod`|change file/folder permissions|
|`chown`|change file/folder owner|
|`pwd`|print present working directory|
|`whoami`|print current user|
|`cd`|change directory|
|`cd ~/my_dockers`|`~` is a shortcut for the users home directory|
---
### System Interaction Commands
|Command|Description|
|---|---|
|`sudo`|super user do.  Basically run a command with elevated permissions|
|`su`|switch user ex: `sudo su - pi`|
|`man ` _command_|returns documentation for specific command. ex: `man chmod`|
|`systemctl start\|stop\|restart` _service-name_|start/stop/restart a service. ex: `systemctl restart docker.service`|
|`cat`|used to print the content of a file|
|`\| grep` _search-text_|pass the output of one command into a text filter. ex: `cat config.yaml \| grep username`|
|`lsof`|List open file, lots of uses (check out `man lsof`).  My favorite use is looking at what ports are "listening". ex: `lsof -i -P -n \| grep LISTEN`|
|`ps`|used view running processes. ex: `ps -ef \| grep docker`
|`top`|also used to view running processes and the resouces it is consuming|
|`vi` or `vim`|my text editor of choice, most distros ship with this. ex: `vi config.yml`|
|`nano`|another text editor you might like better|
|`history`|view bash history, VERY useful, IMO. ex: `history \| grep docker`|
---
### Docker Commands
|Command|Description|
|---|---|
|`docker start`|start a container by its name or id ex: `docker start mealie`|
|`docker-compose up`|Builds, (re)creates, starts, and attaches to containers for a service. ex: `docker-compose up -d --force-recreate homeassistant`|
|`docker build`|used to build custom docker image|
|`docker logs`|used to view logs a specific container|
---
### Directory Structure
|directory|description|
|---|---|
|/bin|binary or executable programs.|
|/etc|system configuration files.|
|/home|home directory. It is the default current directory.|
|/opt|optional or third-party software.|
|/tmp|temporary space, typically cleared on reboot.|
|/usr|User related programs.|
|/var|log files.|
