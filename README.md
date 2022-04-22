# xscreensaver-caffeine-indicator

Modification of caffeine-indicator for work with xscreensaver.
A desktop indicator ‘caffeine-indicator’ supplies a manual toggle to prevent xscreensaver to start.

Based on https://code.launchpad.net/caffeine

# Installation

~~~bash
sudo dpkg -i xscreensaver-caffeine-indicator-1.0.2-Linux.deb
~~~

## Manual run:

~~~bash
xscreensaver-caffeine-indicator
~~~

## To run automaticcally at boot
Add the from the `/usr/share/applications/xscreensaver-caffeine-indicator.desktop` to the settings of your DE or add a link in autostart folder es:
 
~~~bash
ln -s /usr/share/applications/xscreensaver-caffeine-indicator.desktop /home/$USER/.config/autostart/xscreensaver-caffeine-indicator.desktop
~~~

