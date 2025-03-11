# Minecraft server

> [Docker Compose file](../stacks/minecraft.yaml)

I run this Minecraft server for a select group of friends. In the future probably more servers will be hosted, each in it's seperate Docker container.

I use this batch script on Windows to remote into the server and Docker container, to get access to the Minecraft server control panel.
```
@echo off
ssh <user>@<server> -t "bash -l -c 'docker attach minecraft-mc-1'"
BREAK
```
This process can be exited by pressing `Control-p` `Control-q`.
