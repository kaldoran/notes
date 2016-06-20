# Colon commands

    :Ex                 Browse file directory & show what you edited but didn't save
    :'[id]              Jump among recently edited files located in ~/.viminfo
    :browse old         Get a menu with the Recently edited files numbers
    :retab              Replace tabs according to your settings
    :e ++ff=unix        Display CRLF as ^M
    :%s/\r//g           Remove ^M

    :set background=light
    :python import sys; print(sys.version)      Get the compiled python version

# Keyboard shortcuts

    $   go to the end of the line
    A   go to the end of the line and switch to editing mode
    0   go to the beginning of the line incl. whitespace
    ^   go to the first non-whitespace character in the line

    q:  list commands history
    q/  list searches history
    
# Keys

    ctrl + v, tab       insert tab in insert mode

# Show

    /\t                 show all interpreted tabs (if spaces set then spaces)
    /\s\+$              trailing whitespaces
    /\S\zs\s\+$         trailing whitespaces + ignore empty lines
    / \+\ze\t           spaces before tabs

# Vim clipboard

> You do need to install the gvim package to get a Vim linked to libX11; but you don't need to use gvim. --Carpetsmoker

