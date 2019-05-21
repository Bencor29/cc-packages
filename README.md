# cc-packages

## How to install

### packman

You need to install `packman` (https://github.com/lyqyd/cc-packman#12---automatic-pastebin-installation)
Currently the command to run on you ComputerCraft PC is: `pastebin run 4zyreNZy`

### Install nsh

Now you can reboot you ComputerCraft PC and run `packman install nsh`
It will ask you to confirm, type Y then enter
You need to add a label to you computer: `label set <your_computer_name>`

### Start nsh at startup

You need to replace the startup script by another.
First, backup the script `mv /startup /startup.backup` and run `pastebin get xbyCve2i /startup`
Then reboot the computer by typing `reboot` and nsh is installed

### Install secure-nsh

After installing nsh, you can install secure-nsh by typing `packman install secure-nsh`
It will ask you to confirm, type Y then enter

### Tell nsh to use secure-nsh

You have to do it manually ! Open the nsh file `edit /usr/bin/nsh`
Navigate to line 412 (https://i.imgur.com/WIZeoQX.png) 
Then replace `"/rom/programs/shell"` by `"/usr/bin/secure-nsh login"` (https://i.imgur.com/qqeApjr.png)

### Default credentials

The default user is `root` and is password is `root`

### Add, remove or modify a user

The help is available by typing `secure-nsh help`
