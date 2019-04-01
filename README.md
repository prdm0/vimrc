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

# .vimrc file

" Colocando os numerações das linhas.
set number

" Desligando o som do beep.
set vb

" Busca não diferenciada entre maiusculas e minusculas.
set ic

" Ao criar nova linha, utiliza a identação da linha anterior.
set ai

" Tabs são de tamanho de 4 espaços.
set tabstop=4

" Mostra o título do arquivo no rodapé da tela.
set title

" Envia mais caracteres ao terminal, melhorando o redraw de janelas.
set ttyfast

" Usa cores que ficam melhor com fundo preto, quando utiliza-se cores 
" em identação de código fonte.
set background=dark

" Ativa as cores para edição de código fonte.
syntax on

" Identação automatica. As linhas herdam a identação
" das linhas anteriores.
set autoindent

" Sempre mostrará a posição do cursor.
set ruler

" Realça a linha atual do cursor.
set cursorline

" Ativa mouse e redimensionamento.
set mouse=a

" Ativar o realce de pesquisa.
set hlsearch

" Pesquisa incremental que mostra correspondências parciais.
set incsearch
