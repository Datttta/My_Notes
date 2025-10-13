=== Things to remember ===

- Search on anki:
    - Specific field, exclude cards with a specific word (use the *): -back:*google*

    - Specific fild, show cards with a specific word: back:*google*

    - Specific deck: deck:<deck-name>

- Vim:
    - Select everything betwwen space: *viW*
    - Delete everything inside "", '', (), etc: *ci<object surrounding the text>*
    - Move cursor to the end of the line: *$*

- Nvim:
    - Search and replace: *:%s/<old_text>/<new_text>/g* (you don't need to use the 'g')
    - Format nvim code: *<leader>fm*

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
        - zip -r world world or cp -r world world_backup

- anki background images folder:
    - /home/DROS/.local/share/Anki2/addons21/1210908941/user_files/background/
