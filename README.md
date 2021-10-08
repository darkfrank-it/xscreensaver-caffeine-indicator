# xscreensaver-caffeine-indicator
Modification of caffeine-indicator for xscreensaver

Based on https://code.launchpad.net/caffeine

This script need the original project resource to work, so you have to download it under xscreensaver-caffeine folder inside your home. Put here this script too.

~~~
sudo apt-get install bzr
cd /home/$USER/xscreensaver-caffeine
bzr branch lp:caffeine
chmod +x xscreensaver-caffeine-indicator
sudo ln -s /home/$USER/xscreensaver-caffeine/xscreensaver-caffeine-indicator /usr/local/bin/xscreensaver-caffeine-indicator
~~~

You can make a desktop link

~~~
sudo nano /usr/share/applications/xscreensaver-caffeine-indicator.desktop
~~~

~~~
[Desktop Entry]
Icon=/home/nicola/laboratorio/xscreensaver-caffeine/caffeine/share/icons/ubuntu-mono-dark/status/scalable/caffeine-cup-full.svg
Name=XScreenSaver Caffeine Indicator
Comment=Manually control activation of the screensaver and sleep mode
Exec=/usr/local/bin/xscreensaver-caffeine-indicator
Terminal=false
Type=Application
Categories=Utility;TrayIcon;
Keywords=Screensaver,Power,Saving,Blank
OnlyShowIn=GNOME;KDE;LXDE;LXQt;MATE;Razor;ROX;TDE;Unity;XFCE;EDE;Cinnamon;Pantheon;
StartupNotify=false
~~~

And then you can make autostarting the script from the settings od your DE. 
