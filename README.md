# mullvad-runit
Mullvad service file for the Runit init system.
## Why
Mullvad only officially supports the systemd init system. And for those of us who like to use different init systems, this can be a problem.
To save you the 2 minutes it would take to whip this up, I decided to put this on github.

## Script
The actual service file is so small that I can fit it in the readme..

```
#!/bin/sh

exec '/opt/Mullvad VPN/resources/mullvad-daemon' -v --disable-stdout-timestamps
```

like seriously i learned how to do this with one duckduckgo search...
