= COMMANDS =

- Seeing tree:
    - Show only directories: tree -d

    - Limit depth (e.g., 2 levels): tree -L 2

    - Show hidden files: tree -a

    - Show full path: tree -f

    - Show with color: tree -C

 
- Exctrating files:
    - .tar: *tar -xvf* file.tar

    - .tar.gz or .tgz: *tar -xzvf* file.tar.gz

    - .tar.bz2: *tar -xjvf* file.tar.bz2

    - .tar.xz: *tar -xJvf* file.tar.xz

    - .zip: *unzip* file.zip

    - .rar: *unrar x* file.rar

    - .7z: *7z x* file.7z
    
    - .gz (single): *gunzip* file.gz
    
    - .bz2 (single): *bunzip2* file.bz2

    - .xz (single): *unxz* file.xzvf

    - tar -xzvf file.tar.gz *-C* /target/directory (use -C to target directories)

 
- Giving permission to other users to read and access a foler or files:
    - *chmod -R o+rx* | e.g. chmod -R o+rx /home/DROS/dotfiles/slashConfs/*

- Vimwiki help:
    - *:h vimwiki-syntax*

- Clean clipboard: 
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
    - Create a numbered list: <leader>ne 
      
    - renumber a list: *<leader>rn*

    - Redo a list: *<leader>rl*

- Find files with fzf:
    - to preview files use: *fzf --preview="cat {}"*

    - preview with syxtax highlight: *fzf --preview="bat --color=always {}"*
