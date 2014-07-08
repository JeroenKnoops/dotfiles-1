These are my personal dotfiles. Feel free to browse through them and copy whatever takes your fancy.

To use this:

## install rvm and compile a recent version of ruby
    \curl -sSL https://get.rvm.io | bash
    
    rvm requirements
    rvm install 2.1.0
    rvm use 2.1.0 --default

## install oh-my-zsh

    git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh

## Install zsh-syntax-highlighting

    cd ~/.oh-my-zsh/custom
    git clone git://github.com/zsh-users/zsh-syntax-highlighting.git

Source the the script *at the end* of `~/.zshrc`:

    source ~/.oh-my-zsh/custom/zsh-syntax-hightlighting/zsh-syntax-highlighting.zsh

## Clone dotfiles

    gem install homesick
    homesick clone jeroenknoops/dotfiles
    homesick symlink dotfiles

## Vim Setup

Vim plugins are managed using Vundle and installed in `~/.vundle.local`. 

To install the Vundle submodule and all plugins: 

    cd ~/.homesick/repos/dotfiles
    git submodule update --init --recursive
    vim +PluginInstall +qall
