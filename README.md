# vimrc
Settings for Vim


#  Install Vim-Plug

At the bash terminal, run the code:

```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

In the **.vimrc** file, add all plugins between `call plug#begin('~/.vim/plugged')` and `call plug#end()`. For example, we can consider the **julia-vim** plugin obtained from the GitHub of the user GitHub [**JuliaEditorSupport**](https://github.com/JuliaEditorSupport). Thus, we have:

```
call plug#begin('~/.vim/plugged')
Plug JuliaEditorSupport/julia-vim
call plug#end()
```
Then start a vim section and run `:PlugInstall!`.

**Note**: If there are no **autoload** and **plugged** directories in **.vim**, build them using `mkdir`.
