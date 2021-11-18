# Supporting Drauger OS
All Drauger OS systems are supported, regardless of Xfce panel settings, other system settings, installed apps, Flatpak Remotes, or additional apt repositories (when added to provide easy access to more apps).

The below details situations which Drauger OS systems may be found in that **ARE NOT** supported.

## Changes to the system
Not all changes to the Drauger OS System can be supported. Otherwise, support requests would be innumerable, and we would not have time to address them all with the attention and patience each and every one deserves.

Changes to the system can include changing, but are not limited to:
 * **init system** (systemd)
 * **desktop environment** (Xfce)
 * **window manager** (xfwm4)
 * **kernel** (Xanmod)
 * **display manger** (lightdm)
 * **display server** (X11)
 * **native package manager** (apt/dpkg)
 * **firewall** (ufw/gufw)
 * **shell** (BASH)
 * **and more ...**
 
If one of these, or any other part of the Drauger OS System, is changed without instruction from a Drauger OS Contributor, that part which was changed will not be supported by any Drauger OS Contributor. All other unchanged parts, however, will continue to be supported.

### Example

**A user is having issues with logging into their system. They attempt to log in, provide the correct password, and end up right back at the login screen. They have changed the desktop environment to Gnome. Xfce is still installed, and when logging into that DE, things work correctly.**

In this instance, there could be a number of reasons why this bug is occurring. We will gladly assist in tracking down where the bug is occurring.

**If the bug is from Gnome**, we will not assist in fixing this system as the desktop environment is not what is shipped with Drauger OS.

**If the bug is with the window manger**, we will not assist. Gnome does not use xfwm4 as the window manager. Instead, it uses Mutter. So, if the bug is resulting from Mutter, we will not assist in fixing this issue. However, if the user has somehow gotten Gnome to work using the xfwm4 window manager instead of Mutter, we will attempt to help as best we can.

**If the bug is with the login window**, this depends on whether GDM or LightDM are being used. Gnome depends on GDM, so if it is using it, we will not assist in fixing this bug. However if it is still LightDM, we will gladly assist.


## Previous Versions
As soon as a new version of Drauger OS is released, the previous version enters into the final stages of the Drauger OS Life Cycle, known as the "Death Throes". Which proceeds as follows:

### Stage 1 – Ceased updates and support
This stage takes affect on the same day the next version of Drauger OS is released. The previous version will no longer receive updates from the Drauger OS Team, and will no longer be supported. Any support requests for this release will be denied beyond this point. At this point, this version of Drauger OS is considered End-Of-Life (EOL).

### Stage 2 – apt repository shutdown
Taking place 4 weeks after Stage 1, the apt repository for the old version of Drauger OS will be taken offline. By this point, all users who wish to remain on this release must disable the Drauger OS apt repository in /etc/apt/sources.list if they wish to still be able to receive updates and install software from Ubuntu’s repositories, as apt will throw an error about the Drauger OS repos being offline.

This takes place to save space on our server.

### Stage 3 – ISO deletion
In the final death stroke for an old version of Drauger OS, the ISO for it will no longer be made available. This will be done when the version of Drauger OS that replaced the old version in question also gets replaced. So, for example: Drauger OS 7.4.1's ISO will be deleted when Drauger OS 7.5.1 meets EOL, and thus Drauger OS 7.6 is released.


## Remote Access
Remote access to a Users system through SSH, telnet, VNC, Spice, RDP, or any other of the numerous methods through which remote control of a system can be established is **STRICTLY PROHIBITED** to all Contributors. This is to ensure the security of Users systems at all times, and to encourage Users to become increasingly familiar with their system.