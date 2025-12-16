=== Solved problems ===

- Firefox based apps not showing tabs in fullscreen in hyprland:
    -URL: about:config 
    - browser.fullscreen.autohide true to false

- Chromium bases browsers not showing the tabs in fullscreen:
    - go to the <app>.desktop file
    - change the exec line to <app> --ozone-platform=x11

- "Failed to install the following packages. Manual intervention is required":
    - cd ~/.cache/yay/<name-of-package>
    - sha256sum <name-of-installer>
    - yay -S <name-of-package> --mflags "--skipchecksums"

- Sddm screen tearing glitch:
    - nvims /etc/default/grub
    - Remove radeon.si_support=0 from "GRUB_CMDLINE_LINUX_DEFAULT=" line. 
 
- Firefox not showing bookmarks after arch maintainance:

    - Maybe opening this folder will fix firefox bookmarks:
        - ~/.mozilla/firefox/izj5orrr.default-release/bookmarkbackups

- Minecraft pauses when lose focus:
    - nvim ~/.minecraft/options.txt
    - change "pauseOnLostFocus:false" to "pauseOnLostFocus:true"

- Pacman failed to syncronize all databases:
    - sudo rm /var/lib/pacman/db.lck

- Bluetooth not working (SetDiscoveryFilter failed: org.bluez.Error.NotReady 
    Failed to start discovery: org.bluez.Error.NotReady):
    - Bluetoothctl
    - sudo rfkill unblock Bluetooth

- cannot open shared object file: No such file or directory:
    - use which -a <app>
    - Make sure you have the not working app in /usr/bin/<app>
    - then remove the app in ~/.local/bin/<app>

- flatpak error: qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "" even though it was found. This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.
    - flatpak override --user --env=QT_QPA_PLATFORM=wayland <com.stremio.Stremio(link you used to download)>

- Steam opens a black screen and closes afterwords:
    - make sure there is only one exec= in steam.desktop 
