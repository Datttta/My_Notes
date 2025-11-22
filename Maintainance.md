=== Maintainance ===

- showing fails:
    - systemctl --failed: show failed units

    - sudo journalctl -p 3 -xb: show fails in lockfiles

- Cleaning:
    - Yay and pacman:
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

    - journalctl (Clean this only if it's taking to much space, cleaning it it's not that necessary):
        - du -sh /var/log/journal/: run it to see the amount of space journalctl is taking

        - man journalctl: you can see the manual page 
        
        - sudo journalctl --vacuum-time-2weeks: it removes all files older than 2 weeks, you can see on manual page other ways to remove files, like using size for example

- Update mirror-list:
    - Current: sudo reflector --protocol https --latest 50 --sort rate --fastest 15 --download-timeout 20 --save /etc/pacman.d/mirrorlist

    - old (not working I think): sudo reflector -c Brazil --download-timeout 60 -a 6 --sort rate --save /etc/pacman.d/mirrorlist;
