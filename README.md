# xscreensaver-caffeine-indicator
Modification of caffeine-indicator for xscreensaver

Based on https://code.launchpad.net/caffeine

# Install

Donwload the file uder a folder of your choise, then make executable the python script and create a convenience shortcut to run directly.

~~~
chmod +x xscreensaver-caffeine-indicator
sudo ln -s /home/$USER/xscreensaver-caffeine/xscreensaver-caffeine-indicator /usr/local/bin/xscreensaver-caffeine-indicator
~~~

You can make a desktop link

~~~
sudo nano /usr/share/applications/xscreensaver-caffeine-indicator.desktop
~~~

~~~
[Desktop Entry]
Icon=caffeine-cup-full
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

And then you can make autostarting the script from the settings of your DE or by adding a link in autostart folder: 

~~~
ln -s /usr/share/applications/xscreensaver-caffeine-indicator.desktop /home/$USER/.config/autostart/xscreensaver-caffeine-indicator.desktop
~~~
