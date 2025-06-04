=== Maintainance ===

- showing fails:
    - systemctl --failed: show failed units

    - sudo journalctl -p 3 -xb: show fails in lockfiles

- Cleaning:
    - sudo pacman -Sc: remove packages from cache

    - yay -Sc
