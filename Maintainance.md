=== Maintainance ===

- showing fails:
    - systemctl --failed: show failed units

    - sudo journalctl -p 3 -xb: show fails in lockfiles

- Cleaning:
    - yay -Sc: remove pacman and aur packages from cache

    - sudo pacman -Sc: remove packages from cache (you don't need to run it if you ran yay -Sc)

    
