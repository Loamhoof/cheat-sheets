Index
-----

* [Aliases](#aliases)
* [Commands](#commands)
* [New commands](#new-commands)
* [Miscellaneous](#miscellaneous)


Aliases
-------

* To create an alias:`git config --global alias.<alias> <command>`
* To create an alias to run from the root directory:`git config --global alias.<alias> "! git <command>"`

Commands
--------

* List all the untracked files: `git ls-files --others --exclude-standard`
* Get the root directory: `git rev-parse --show-toplevel`

New Commands
------------

To add a new git command, add a `git-<command>` binary. Git will automatically create the corresponding `git <command>`.


Miscellaneous
-------------

To add the current branch in the PS1:
```
function parse_git_branch () {
  git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}

RED="\[\033[0;31m\]"
YELLOW="\[\033[0;33m\]"
GREEN="\[\033[0;32m\]"
NO_COLOR="\[\033[0m\]"
PS1="$GREEN\u@\h$NO_COLOR:$RED\w$YELLOW\$(parse_git_branch)$NO_COLOR\$ "
```
