=== Solved problems ===

- Firefox based apps not showing tabs in fullscreen in hyprland:
    -URL: about:config 
    - browser.fullscreen.autohide true to false

- "Failed to install the following packages. Manual intervention is required":
    - cd ~/.cache/yay/<name-of-package>
    - sha256sum <name-of-installer>
    - yay -S <name-of-package> --mflags "--skipchecksums"

- Sddm screen tear glitch:
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
    - sudo rfkill unblock Bluetooth
    - sudo systemctl restart bluetooth

