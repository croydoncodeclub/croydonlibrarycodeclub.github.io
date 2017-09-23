## Respository for the web site

Add HTML and other files to show up on the https://croydonlibrarycodeclub.github.io website.

# Library laptop notes

After a default Manjaro installation, the laptop will beep on boot, to prevent this, add a file `/etc/modprobe.d/nobeep.conf`:
```
blacklist pcspkr
```

Hibernate does not currently work, so to force a shutdown when the lid is closed, in file `/etc/systemd/logind.conf` add the line:
```
HandleLidSwitch=poweroff
```

# Setting up git

Cloning StudentFiles in the home directory, enter:
```
git clone git://github.com/CroydonLibraryCodeClub/StudentFiles.git
```

If git has already been cloned using http, you can reconfigure it to use ssh with the command:
```
git remote set-url origin git@github.com:CroydonLibraryCodeClub/StudentFiles.git
```
