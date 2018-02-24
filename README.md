
Yeah, this isn’t so obvious at the first glance. All the plugins in the vim/bundle/ directory are empty. This is because they are all git repositories themselves and as such, git doesn’t commit its contents.

You also have to symlink the contents of this repo to your dotfiles. For the VIM stuff to work, you have to at least link
.vimrc -> <path/to/repo>/vimrc
and
.vim -> <path/to/repo>/vim
Then, you have to
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
yourself. This being done, you can open Vim and :PluginInstall, to automatically install all the plugins in .vimrc.

This made it work for me, but it isn’t straight forward in any fashion for new comers. For more information look into https://github.com/VundleVim/Vundle.vim.


## Vim - Reference

### Utilities
#### scrooloose/nerdtree
##### Use
Nerdtree can be activated by pressing Ctrl+n in Normal mode

#### majutsushi/tagbar
##### Use
Tagbar can be activated by pressing Ctrl+m in Normal mode

#### ervandew/supertab
##### Use
Automatic tab completion under Inser Mode

#### wesQ3/vim-windowswap'
##### Use 
 - Navigate to the window you'd like to move
 - Press <leader>ww
 - Navigate to the window you'd like to swap with
 - Press <leader>ww again

#### SirVer/ultisnips'
#### junegunn/fzf.vim'
#### junegunn/fzf'
#### godlygeek/tabular'
#### ctrlpvim/ctrlp.vim'
#### benmills/vimux'
#### BufOnly.vim

### Generic Programming Support 
#### jakedouglas/exuberant-ctags'
#### honza/vim-snippets'
#### Townk/vim-autoclose'
#### tomtom/tcomment_vim'
#### tobyS/vmustache'
#### janko-m/vim-test'

### Inteface Improvements
#### ryanoasis/vim-devicons'
#### vim-airline/vim-airline'
#### vim-airline/vim-airline-themes'
#### sjl/badwolf'
#### tomasr/molokai'
#### morhetz/gruvbox'
#### zenorocha/dracula-theme', {'rtp': 'vim/'}
#### junegunn/limelight.vim'
#### mkarmona/colorsbox'
#### romainl/Apprentice'
#### Lokaltog/vim-distinguished'
#### chriskempson/base16-vim'
#### w0ng/vim-hybrid'
#### AlessandroYorba/Sierra'
#### daylerees/colour-schemes'
#### effkay/argonaut.vim'

### Markdown and Writing
#### reedes/vim-pencil'
#### tpope/vim-markdown'
#### jtratner/vim-flavored-markdown'
#### LanguageTool'

### Elixir Support
#### elixir-lang/vim-elixir'
#### avdgaag/vim-phoenix'
#### mmorearty/elixir-ctags'
#### mattreduce/vim-mix'
#### BjRo/vim-extest'
#### frost/vim-eh-docs'
#### slashmili/alchemist.vim'
#### tpope/vim-endwise'
#### jadercorrea/elixir_generator.vim'

### Erlang Support
#### vim-erlang/vim-erlang-tags'
#### vim-erlang/vim-erlang-runtime'
#### vim-erlang/vim-erlang-omnicomplete'
#### vim-erlang/vim-erlang-compiler'

### ELM Support
#### lambdatoast/elm.vim'

### PHP Support
#### phpvim/phpcd.vim'
#### tobyS/pdv'

### Git Support and Integration
#### kablamo/vim-git-log'
#### gregsexton/gitv'
#### tpope/vim-fugitive'
#### jaxbot/github-issues.vim'
