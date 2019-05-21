# cc-packages

## How to install

### packman

You need to install `packman` (https://github.com/lyqyd/cc-packman#12---automatic-pastebin-installation)

Currently the command to run on you ComputerCraft PC is: `pastebin run 4zyreNZy`



### Install nsh

Now you can reboot you ComputerCraft PC and run `packman install nsh`

It will ask you to confirm, type Y then enter


You need to add a label to you computer: `label set <your_computer_name>`



### Install secure-nsh

After installing nsh, you can install secure-nsh by typing `packman install secure-nsh`

It will ask you to confirm, type Y then enter



### Start nsh at startup

You need to modify the startup script to add nsh at startup.

First, backup the script `cp /startup /startup.backup` then open the file by typing `edit /startup`

Add this line **at the end**: `shell.run("/usr/bin/nsh host /usr/bin/secure-nsh")` (https://i.imgur.com/89rUvis.png)

Then reboot the computer by typing `reboot` and nsh is installed



### Default credentials

The default user is `root` and is password is `root`



### Add, remove or modify a user

The help is available by typing `secure-nsh help`
