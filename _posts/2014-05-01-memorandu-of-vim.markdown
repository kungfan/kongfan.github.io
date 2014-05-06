---
layout: post
---

There is a memorandum reminding me of vim 

    word movemnet
    (n)* b B e E w W ge gE  
    option : iskeyword
    
    moving to the end or start of a line
    ^ 0 (n)$
    
    moving to a character
    (n)* f F t T 
    
    matching a parenthesis
    %
    option : matchpairs
    
    moving to a special line
    (n)* gg G % H M L 
    
    where are you
    CTRL-G
    option : ruler number nonumber
    
    scrolling around
    CTRL-U CTRL-D 
    CTRL-E CTRL-Y
    CTRL+F CTRL-B
    zz zt zb
    
    search
    / ? 
    (n)* n N 
    /\> /\< /\< \>
    *
    ^ $ . \
    option : ignorecase noignorecase hlsearch  
              nohlsearch incsearch nowrapscan
    
    marks
    `` '' 
    CTRL-O CTRL-I TAB 
    m*
    ` " [ ]
    
    making changes
    d c dd cc
    C D s S x X 
    
    repeating a change
    .
    
    visual mode
    v V CTRL-V
    o
    
    textwidth wrap nowrap
    
    (n)* p P
    xp
    
    copying text
    y yy Y y$ yw ye (n)y(n)w 
    
    using the clipboard
    *yy *p
    
    text object
    aw is as daw cis dis dsa 
    
    replace mode
    r R <ESC> <Insert>
    
    I A ~
    
    edit another file
    edit! foo.txt hide edit foo.txt
    (n)next next! wnext
    :args
    :first :last :previous :wprevious
    option : autowrite noautowrite
    args a.file b.file c.file CTRL-^
    `" `.
    mA(uppercase letter,not a) `A
    option ：backup backupext patchmode
    
    copy text between files
    y p P 
    
    using registers
    "[register]y "[register]p
    :write >> logfile
    
    viewing a file (mode)
    vim -R file view file vim -M file 
    option : modifiable write
    :saveas filename file filename
    
    splitting windows
    :(n)split (n)vsplit:close :only ZZ :quit
    :new :vnew
    (height) CTRL-W +
    (height) CTRL-W -
    :qall :wall :wqall :qall! 
    
    vim -o file1 file2 file3
    
    viewing differences with vimdiff
    vimdiff file1 file2
    zo zc
    diffsplit
    optin : noscrollbind laststatus
    ]c [c
    :diffupdate :dp :do
    
    tab pages
    :tabedit filename
    :tab split
