# Setup

1) Execute setup script:
    ```bash
    sudo pacman -S git
    git clone https://github.com/SmirnovAlexander/DotFiles.git
    cd DotFiles
    ./setup.sh
    ```
2) Reboot in case of desktop and relogin in case of server
3) Execute post setup script if on desktop:
    ```bash
    ./post_setup.sh
    ```
4) Install vim plugins:
    ```
    :PlugInstall
    ```
5) Install tmux plugins:
    ```
    <C-b> + I
    ```
6) Brave settings
    - [disable password savings](brave://settings/passwords)
    - [change search engine to Google](brave://settings/search)
        * [enable autocomplete searches option](brave://settings/privacy)
    - [vimium extension](https://chrome.google.com/webstore/detail/vimium/dbepggeogbaibhgnhhndojpepiihcmeb?hl=en)
    - [workspaces extension](https://chrome.google.com/webstore/detail/workspaces/hpljjefgmnkloakbfckghmlapghabgfa?hl=en)
    - [grammarly extension](https://chrome.google.com/webstore/detail/grammarly-grammar-checker/kbfnbcaeplbcioakkpcpgfkobkghlhen)

## TODO

- open all terminal windows at tmux
    * tmux attach-session -t random \; new-window ranger
- solution for notes management
- rewrite mute script to iterate through all sources and mute/unmute them
    * display muted status as **every** output is muted
- add st plugins patches
    * [scrollback](https://st.suckless.org/patches/scrollback/)
    * [alpha](https://st.suckless.org/patches/alpha/)
    * [copyurl](https://st.suckless.org/patches/copyurl/)
    * [open_copied_url](https://st.suckless.org/patches/open_copied_url/)

## Known issues

- tmux is not loading config from `$XDG_CONFIG_HOME/tmux/tmux.conf` on old versions
