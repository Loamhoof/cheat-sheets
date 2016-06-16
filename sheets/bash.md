Index
-----

* [History](#history)
* [Shortcuts](#shortcuts)

History
-------

* Search the history: `Ctrl + R`
* Repeat the last command: `!!` (can be embedded in another command - e.g. `sudo !!`)
* Repeat the nth last command: `!-<num>`
* Repeat the nth command: `!<num>` (to display the command number in the PS1, add `\!`)
* Repeat the last command starting with `<str>`: `!<str>`
* Repeat the last command containing `<str>`: `!?<str>`
* Replace something in the last command: `^<str1>^<str2>^`
* Reuse the first argument of a command: `:^` (e.g. `!!:^`)
* Reuse the last argument of a command: `:$` (e.g. `!!:$`)
* Reuse the nth argument of a command: `:<num>` (e.g. `!!:<num>`)
* Reuse all the arguments of a command: `:*` (e.g. `!!:*`)
* Reuse a range of argument of a command: `:<num1>-<num2>`, `:<num1>-`, `:<num1>-$`, `:<num1>*`, `:^-<num2>`, `:-<num2>`
* Remove the file part of an argument: `:h` (e.g. `!!:^:h`)
* Remove the directory part of an argument: `:t` (e.g. `!!:^:t`)
* Remove the extension part of an argument: `:r` (e.g. `!!:^:r`)
* Print the command without executing it: `:p` (e.g. `!!:^:t:r:p`)

Shortcuts
---------

* Move (word): `Alt + B` (backward) ; `Alt + F` (forward)
* Move (line): `Ctrl + A` (backward) ; `Ctrl + E` (forward)
* Move (other): `Ctrl + XX` (between cursor and BOL)
* Clear (word): `Ctrl + W` (backward) ; `Alt + D` (forward)
* Clear (line): `Ctrl + U` (backward) ; `Ctrl + K` (forward)
* Paste: `Ctrl + Y` (what has been cut)
* Swap (letters): `Ctrl + T` (backward)
* Swap (words): `Alt + T` (backward)
