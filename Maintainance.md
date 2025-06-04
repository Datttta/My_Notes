=== Maintainance ===

- showing fails:
    - systemctl --failed: show failed units

    - sudo journalctl -p 3 -xb: show fails in lockfiles

- Cleaning:
    - yay -Sc: remove pacman and aur installed packages from cache

    - yay -Scc: remove all pacman and aur installed packages from cache (Risky, do that if you dont't have disk space)

    - yay -Yc: remove all unneeded dependencies

    - sudo pacman -Sc: remove installed packages from cache (you don't need to run it if you ran yay -Sc)

    - sudo pacman -Scc: remove all pacman packages from cache(You don't need to run this if you ran yay -Scc)

    - Dealing with orphan packages:
        - pacman -Qtdq: show orphan packages

        - sudo pacman -Rns $(pacman -Qtdq): delete orphan packages

    - Cleaning ~/.cache/ directory:
        - du -sh .cache: show how much space .cache is taking

        - rm -rf .cache/* : remove all files inside .cache

    
