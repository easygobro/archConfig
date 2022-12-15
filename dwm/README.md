dwm - dynamic window manager
============================
dwm is an extremely fast, small, and dynamic window manager for X.

What is this???
---------------
This is simply a fork of the stock suckless build of DWM. If you are looking for stock, go to https://dwm.suckless.org/ . Otherwise, continue reading.

What does it add?
----------------
This build of DWM adds a couple of patches. It contains the systray patch, which allows applets such as nm-applet and enpass to sit to the right of the text status bar. It also contains the useless gap patch, which adds gaps between windows when there is more than 1 window on a tag.

In terms of the config.h file, many of the keybindings were changed. The mod key was switched from the alt key to the Windows key on the keyboard. Many of the keybindings were changed to be more similar to i3wm keybindings. Volume and brightness key support was also added, but you may need to configure the xbacklight & amixer commands to make sure it works on your system.

Some other changes to the config.h file include some basic color changes. The current color scheme is supposed to go with the Adapta GTK theme & Nord color scheme. I switched the current default terminal to URxvt from ST, but that can be easily changed back or to a different Terminal in the term variable.

Sounds cool! Install guide?
---------------------------
Just install it the same way you would install DWM.

    git clone https://github.com/tbilik/dwm
    cd dwm/
    sudo make clean install

Make sure you add the login entry to your display manager if you use one.
