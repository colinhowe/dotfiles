My dotfiles.

Install::
    mkdir -p ~/.vimtmp/backups
    mkdir ~/.vimtmp/swap
    mv ~/.vim ~/vim-old
    mv ~/.vimrc ~/vimrc-old
    ln -st vim/ ~/.vim
    ln ./vim/vimrc ~/.vimrc

