My dotfiles::

    sudo apt-get install exuberant-ctags 
    mkdir -p ~/.vimtmp/backups
    mkdir ~/.vimtmp/swap
    mv ~/.vim ~/vim-old
    mv ~/.vimrc ~/vimrc-old
    cd ~
    ln -s dotfiles/vim/ .vim
    ln -s dotfiles/vim/vimrc .vimrc
    mv ~/.bashrc ~/.bashrcold
    ln -s dotfiles/bashrc .bashrc

    # Download all the bundles
    cd dotfiles
    git submodule sync
    git submodule update

    cd vim/bundle/command-t
    rake make
    cd ../../../

    mkdir -p ~/.vimtmp/swap
    mkdir -p ~/.vimtmp/backups
