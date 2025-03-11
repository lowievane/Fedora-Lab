# Minecraft server

> [Docker Compose file](../stacks/minecraft.yaml)

I run this Minecraft server for a select group of friends. In the future probably more servers will be hosted, each in it's seperate Docker container. For these containers, the directory is exceptionally set to the Data SMB share. This way I have access to the Minecraft server files from every device on my network, and I can easily put new mods in for example.

I use this batch script on Windows to remote into the server and Docker container, to get access to the Minecraft server control panel.
```
@echo off
ssh <user>@<server> -t "bash -l -c 'docker attach minecraft-mc-1'"
BREAK
```
This process can be exited by pressing `Control-p` `Control-q`.

Mods currently running:
- Dungeon Crawl
- Geckolib
- Inventory View (only for admin)
- Jade
- Just Enough Items
- ModernFix
- Mowzies Mobs
- PlayIT.GG (for tunneling the server to the outside world)
- Prometheus Exporter (to give Prometheus access to metrics)
- Skin Restorer (because server runs in offline mode)
- ...

Server properties [here](../configs/server.properties).
