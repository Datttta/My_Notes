=== Solved problems ===

- Firefox based apps not showing tabs in fullscreen in hyprland:
    -URL: about:config 
    - browser.fullscreen.autohide true to false

- "Failed to install the following packages. Manual intervention is required":
    - cd ~/.cache/yay/<name-of-package>
    - sha256sum <name-of-installer>
    - yay -S <name-of-package> --mflags "--skipchecksums"

- Sddm glitched screen (splintered strips):
    - nvims /etc/sddm.conf
    - add this to the file:
        [General]
        DisplayServer=wayland

        [Wayland]
        CompositorCommand="Hyprland"

- Firefox not showing bookmarks after arch maintainance:

    - Maybe opening this folder will fix firefox bookmarks:
        - ~/.mozilla/firefox/izj5orrr.default-release/bookmarkbackups   
