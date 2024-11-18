My dotfiles::

    mv ~/.bashrc ~/.bashrcold
    ln -s dotfiles/bashrc .bashrc
    ln -s dotfiles/zshrc .zshrc
    ln -s ~/dotfiles/vscode-settings.json ~/.config/Code/User/settings.json

    mkdir -p ~/.vimtmp/swap
    mkdir -p ~/.vimtmp/backups
