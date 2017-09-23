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
