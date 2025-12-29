=== Things to remember ===

- When you get a better monitor (maybe a 4k), change theme scale:
    - change from calloid-grey-dark-xhdpi to calloid-grey-dark-hdpi

- Search on anki:
    - Specific field, exclude cards with a specific word (use the *): -back:*google*
    - Specific fild, show cards with a specific word: back:*google*
    - Specific deck: deck:<deck-name>
    - Specific word: re:\b<word>\b

- Exctrating files:
    - *.tar*: tar -xvf file.tar

    - *.tar.gz or .tgz*: tar -xzvf file.tar.gz

    - *.tar.bz2*: tar -xjvf file.tar.bz2

    - *.tar.xz*: tar -xJvf file.tar.xz

    - *.zip*: unzip file.zip

    - *.rar*: unrar x file.rar

    - *.7z*: 7z x file.7z
    
    - *.gz* (single): gunzip file.gz
    
    - *.bz2* (single): bunzip2 file.bz2

    - *.xz* (single): unxz file.xzvf

    - tar -xzvf file.tar.gz *-C* /target/directory (use -C to target directories)

- Compressing files:
    - .zip: zip -r <zip-name>.zip <folder-to-zip>

- Nvim:
    - Select everything betwwen space: *viW*

    - Select everything between "",'',()...: vi<object-surrouding the text>

    - Delete everything inside "", '', (), etc: *ci<object surrounding the text>*
    
    - Move cursor to the end of the line: *$*
    
    - "Clear" line: *cc*
    
    - Dark background with tokyo night - moon style colors: nvim /home/DROS/.local/share/nvim/lazy/tokyonight.nvim/lua/tokyonight/colors/night.lua
        - change the line "local ret = vim.deepcopy(require("tokyonight.colors.storm"))" to "local ret = vim.deepcopy(require("tokyonight.colors.moon"))" 
  
    - Search and replace: *:%s/<old_text>/<new_text>/g* (you don't need to use the 'g')
    
    - Format nvim code: *<leader>fm*
    
    - Update lazyvim plugins: *:Lazy update* on nvim
    
    - delete and Change mode to end of current word: ce

    - Delte everything after the cursor in the line: d$

- Kitty terminal:
    - Delete text on terminal: *Ctrl+u*
    - Move cursor to the begining of the line: *Ctrl+a*
    - Move cursor to the end of the line: *Ctrl+e*
    - Delete everything from the cursor's position to the end of the line: *Ctrl+k*
    - Delete word right behind the cursor: *Ctrl+w*

- Minecraft server
    - Open minecraft server:
        - go to your server's folder: cd ~/Games/Mcservers
        - java -Xmx2G -Xms1G -jar server.jar nogui

    - Restart the server:
        - cd ~/Games/Mcservers/
        - rm world/session.lock

    - Creating backups:
        - cd ~/Games/Mcservers/ 
        - zip -r <folder-name> <zip-name> or cp -r world world_backup

- anki background images folder:
    - /home/DROS/.local/share/Anki2/addons21/1210908941/user_files/background/

- Fzf history:
    - Alt + a

- Bluetooth:
    - Alt + <F1>: connect to you earbuds
    - Alt + <F2>: disconnect you device
    - Alt + <F3>: Show device info (including battery porcentage)
    - Alt + <F4>: Change audio profile to low latency
    - Alt + <F5>: Change audio profile to high quality

- Comment more than one line at the same time nvim:
    - Select the line and type *gc*

- Flatpak:
    - show flatpak apps: flatpak list
    - unistall: flatpak uninstall <app-name>
    - uninstall unused: flatpak uninstall --unused
    - flatpak .desktop folder: /var/lib/flatpak/exports/share/applications/

- Hibernation on terminal:
    - Hibernate for a specific time: sudo rtcwake -m disk -t $(date -d "2 minutes" +%s)
    - Awake from hibernation in a specific moment: sudo rtcwake -m disk -t $(date -d "today 10:50" +%s)

- Pacman:
    - Search packages: sudo pacman -Ss <package-name>

- Seeing tree:
    - Show only directories: tree -d

    - Limit depth (e.g., 2 levels): tree -L 2

    - Show hidden files: tree -a

    - Show full path: tree -f

    - Show with color: tree -C

- Giving permission to other users to read and access a foler or files:
    - *chmod -R o+rx* | e.g. chmod -R o+rx /home/DROS/dotfiles/slashConfs/*

- Vimwiki help:
    - *:h vimwiki-syntax*

- Clear clipboard: 
    - *cliphist wipe*

- Stow root files:
    - *sudo stow -t / fonts*

    - if you want restow it:
        - *sudo stow -R -t / slashConfs*

- How to preview markdown files vimwiki:
    - *:MarkdownPreview*

- Run app with amd/radeon driver:
    - *DRI_PRIME=1* 
      
- Lists:
    - *:'<,'>s/^\s*\%(\d\+\.\s*\)\?/\=line('.') - line("'<") + 1 . ". "/*

    - Create a numbered list: <leader>ne 
      
    - renumber a list: *<leader>rn*

    - Redo a list: *<leader>rl*

- Find files with fzf:
    - to preview files use: *fzf --preview="cat {}"*
    - preview with syxtax highlight: *fzf --preview="bat --color=always {}"*
    - look for a file a directory: fd <directory> <what-you-want-to-fint>
    - loof for a file in the current directory: fd . <what-you-want-to-fint>

- How to see hidden files with ls:
    - use: *ls -a*

- How to make a file executable:
    - use: *ls -l filename*

- Completly close an application:
    - use: *Super + X*

- Case WARNING: UNPROTECTED PRIVATE KEY FILE! Permissions 0605 for '/home/DROS/.ssh/id_MyArch' are too open.
    - use:
        - cd ~/.ssh
        - chmod 600 id_MyArch
        - chmod 700 ~/.ssh

- Star an app with xwayland/x11:
    - for gtk apps: *GDK_BACKEND=x11* <app>
    - for Chromium browsers: <app> *--ozone-platform=x11*

- Open swaync (Sway Notification Centre):
    - swaync-client -t

- Commands for desktop sreenshots:
    - cmatrix -b (b is to make some caracters bold)
    - asciiquarium (sea animation)
    - cava (bar spectrum audio visualizer)
    - tenki (clock with rain effect, you can use metoar effect with --mode metoar)
    - tty-clock -s -c (normal clock -s is for seconds and c is to center the clock)
    - pipe.sh -t 0 (0-9) (pipes running on the screen): https://github.com/pipeseroni/pipes.sh
    - nvim .cache/wal/colors-hyprland.conf

- Exec command firefox.desktop:
    - Exec=env MOZ_ENABLE_WAYLAND=1 MOZ_WEBRENDER=1 /usr/lib/firefox/firefox %u

- Hamachi:
    - start hamachi: sudo systemctl start logmein-hamachi.service
    - stop hamahci: sudo systemctl stop logmein-hamachi.service

- Storage:
    - check storage usage per folder: du -sh *
    - check only linux partition: df -h /
    - check overall disk usage: df -h

- Thunar:
    - open thuner in the current directory: thuner .

- Choose default app, works for nnn:
    - get the file type: -mime query filetype <PATH_TO_FILE>
    - then use: xdg-mime default <APPLICATION> <FILE_TYPE>
    - Exemple:
        - xdg-mime query filetype ~/Videos/Video_bueno.avi
        - the output will be: video/x-msvideo
        - xdg-mime default mpv.desktop video/x-msvideo

    - You can also access the file with the default apps: nvim ~/.config/mimeapps.list

- Yazi:
    - help: double press "~"
    - yazi mount plugin:
        -  

- Change current date/time:
    - sudo timedatectl set-ntp false
    - set the day and time your want to be in: *sudo date -s "2025-12-27 22:30:00"*

- Language apps:
    - Miraa app (for shadowing)
