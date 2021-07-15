# VIM

## Installation
* Google how to install Vundle (Pluging manager)
* Create `~/.vimrc`. Put there these rows:
    ```
    set rtp+=~/.vim/bundle/Vundle.vim
    call vundle#begin()
        Plugin 'VundleVim/Vundle.vim'
    call vundle#end()
    filetype plugin indent on
    ```
* Type in terminal `vim`, then `:PluginInstall`. Now you installed Vundle
* Finally, paste to `~/.vimrc` rows from `myvimrc.txt`. Then install new plugins by typing in terminal `vim`, then `:PluginInstall`

## My some usefull notes

### Navigation

You can navigate cursor in `NORMAL MODE`.
* `0` - move to the begin of line
* `w` - move to the next word
* `b` - move back to the last word
* `f` (then type char) will move to first math

* `<number> + direction` - move `<number>` steps in given diraction in {→,←,↑,↓}.
* `<number> + w`, e.g. `3w` - move to the next `3` words.
* `b` - move previous word
* `<number> + b` - go `<number>` words back
* `gg` - go to the top of file
* `G` - go to the end of file
* `$` - end of row
* `cntr + u` - fast scroll up
* `cntl + d` - fast scroll down

### Search
1. Press `/` then type word to search. Then press `ENTER`
2. Move to next math `n`
3. Move back to prev math press `N`

### DELETION
1. Press `d` (delete) + `a command`, for example:
    * `dw`- delete next word
    * `dd` - delete current line
    * `de` - delete last part of word
    * `db` - delete begin of word

### VISUAL MODE

Press `CTRL + v` to change `VISUAL MODE`. Using by navigations select rows, words.
Press `SHIFT + v` select current row. By selecting you can easy delete, copy data. For example:
* Press `CTRL + v` then `5w` - select 5 word. If then press `d` - delete, it will delete selected 5 words. In order to copy press `y` (yield).
* Press `SHIGT + V`, then `10↓` to select 10 rows down.


### Replace occurance
* `%s/<phrase>/<new phrase>/g` - repalce every where
* `%s/<phrase>/<new phrase>/gc` - replace by commition

### Comment block of code
* `CTRL + c` - change to `VISUAL MODE`
* Select by `↑` or `↓` need rows
* `SHIFT + i` - change to `INSERT MODE`
* Type `#` for python file, `//` for c++ files. Then press `Esc`.

### Uncomment givent block of code
* `CTRL + c` - change to visual mode
* Select by `↑` or `↓` rows        
* Press `x`

### Block tab
* Select need rows then press `>>` forward tabs.
* Select need rows then press `<<` for back tabs.

### Windows
1. `:new` - create horizontal window
2. `:vnew` - create verital window
3. `:split <file name>` - open `<file name>` in splitted window
4. `:vsplit <file name>` - open `<file name>` in vertiacally window

### NERDTRee (navigation tree)
* `Ctrl + w` - next window.
* If press `t` on file its create new tab
* Switch between tabs by `gt`
