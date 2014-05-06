---
layout: post
---

Bash, which is the default shell in Linux contains a whole lot of key bindings which makes it really easy to use.  The following [Bash](http://en.wikipedia.org/wiki/Bash_shell) shortcuts work when using default (Emacs) key bindings. Vi-bindings can be enabled by running set -o vi.

**Note** : For shortcuts involving ⎇ Alt, you may be able to use ⎋ Esc instead.
    Sometimes, you must use ⎋ Esc instead of ⎇ Alt, because the ⎇ Alt shortcut conflicts with another shortcut.

    Tab ↹    : Autocompletes from the cursor position.
    ^ Ctrl+a : Moves the cursor to the line start (equivalent to the key ⇱ Home).
    ^ Ctrl+b : Moves the cursor back one character (equivalent to the key ←).
    ^ Ctrl+c : Sends the signal SIGINT to the current task, which aborts and closes it.
    ^ Ctrl+d : Sends an EOF marker, which  closes the current shell . 
    ^ Ctrl+e : (end) moves the cursor to the line end (equivalent to the key ⇲ End).
    ^ Ctrl+f : Moves the cursor forward one character (equivalent to the key →).
    ^ Ctrl+g : Abort the research and restore the original line.
    ^ Ctrl+h : Deletes the previous character (same as backspace).
    ^ Ctrl+i : Equivalent to the tab key.
    ^ Ctrl+j : Equivalent to the enter key.
    ^ Ctrl+k : Clears the line content after the cursor and copies it into the clipboard.
    ^ Ctrl+l : Clears the screen content (equivalent to the command clear).
    ^ Ctrl+n : (next) recalls the next command (equivalent to the key ↓).
    ^ Ctrl+o : Executes the found command from history
    ^ Ctrl+p : (previous) recalls the prior command (equivalent to the key ↑).
    ^ Ctrl+r : (research) recalls the last command including the specified character(s). 
    ^ Ctrl+s : Go back to the next more recent command of the research .
    ^ Ctrl+t : Transpose the previous two characters.
    ^ Ctrl+u : Clears the line content before the cursor and copies it into the clipboard.
    ^ Ctrl+v : If the next input is also a control sequence, type it literally 
    ^ Ctrl+w : Clears the word before the cursor and copies it into the clipboard.
    ^ Ctrl+x ^ Ctrl+e : Edits the current line in the $EDITOR program, or vi if undefined.
    ^ Ctrl+x ^ Ctrl+r : Read in the contents of the inputrc file,
               and incorporate any bindings or variable assignments found there.
    ^ Ctrl+x ^ Ctrl+u : Incremental undo, separately remembered for each line.
    ^ Ctrl+x ^ Ctrl+v : Display version information about the current instance of bash.
    ^ Ctrl+x ^ Ctrl+x : Alternates the cursor with its old position. .
    ^ Ctrl+y : (yank) adds the clipboard content from the cursor position.
    ^ Ctrl+z : Sends the signal SIGTSTP to the current task, which suspends it. 
    ^ Ctrl+_ : Incremental undo, separately remembered for each line.
    ⎇ Alt+b : (backward) moves the cursor backward one word.
    ⎇ Alt+c : Capitalizes the character under the cursor and moves to the end of the word.
    ⎇ Alt+d : Cuts the word after the cursor.
    ⎇ Alt+f : (forward) moves the cursor forward one word.
    ⎇ Alt+l : Lowers the case of every character 
    ⎇ Alt+r : Cancels the changes and puts back the line as it was in the history.
    ⎇ Alt+u : Capitalizes every character 
    ⎇ Alt+. : Insert the last argument to the previous command 

------


The most commonly used shortcuts are listed below :

CTRL Key Bound
---
    Ctrl + a - Jump to the start of the line
    Ctrl + b - Move back a char
    Ctrl + c - Terminate the command
    Ctrl + d - Delete from under the cursor
    Ctrl + e - Jump to the end of the line
    Ctrl + f - Move forward a char
    Ctrl + k - Delete to EOL
    Ctrl + l - Clear the screen
    Ctrl + r - Search the history backwards
    Ctrl + R - Search the history backwards with multi occurrence
    Ctrl + u - Delete backward from cursor
    Ctrl + xx - Move between EOL and current cursor position
    Ctrl + x @ - Show possible hostname completions
    Ctrl + z - Suspend/ Stop the command

Alt Key Bound
---
    Alt + < - Move to the first line in the history
    Alt + > - Move to the last line in the history
    Alt + ? - Show current completion list
    Alt + * - Insert all possible completions
    Alt + / - Attempt to complete filename
    Alt + . - Yank last argument to previous command
    Alt + b - Move backward
    Alt + c - Capitalize the word
    Alt + d - Delete word
    Alt + f - Move forward
    Alt + l - Make word lowercase
    Alt + n - Search the history forwards non-incremental
    Alt + p - Search the history backwards non-incremental
    Alt + r - Recall command
    Alt + t - Move words around
    Alt + u - Make word uppercase
    Alt + back-space - Delete backward from cursor

More Special Keybindings
---
    Here "2T" means Press TAB twice
    $ 2T - All available commands(common)
    $ (string)2T - All available commands starting with (string)
    $ /2T - Entire directory structure including Hidden one
    $ 2T - Only Sub Dirs inside including Hidden one
    $ *2T - Only Sub Dirs inside without Hidden one
    $ ~2T - All Present Users on system from "/etc/passwd"
    $ $2T - All Sys variables
    $ @2T - Entries from "/etc/hosts"
    $ =2T - Output like ls or dir

