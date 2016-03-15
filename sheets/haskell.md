Index
-----

* [Install GHC & Cabal](#install-haskell)
* [New project](#new-project)
* [Shell](#shell)


Install Haskell
---------------

```bash
sudo apt-get update
sudo apt-get install -y software-properties-common
sudo add-apt-repository -y ppa:hvr/ghc
sudo apt-get update
sudo apt-get install -y cabal-install-1.22 ghc-7.10.3
cat >> ~/.bashrc <<EOF
export PATH="\$HOME/.cabal/bin:/opt/cabal/1.22/bin:/opt/ghc/7.10.3/bin:\$PATH"
EOF
export PATH=~/.cabal/bin:/opt/cabal/1.22/bin:/opt/ghc/7.10.3/bin:$PATH
```

New Project
-----------

```bash
cabal sandbox init
```

Shell
-----

* `:t` inspects the type.
* `:i` gets info about the type.
* `:k` inspects the kind.
* `:set -X<extension>` sets the extension `<extension>` (e.g. `UnicodeSyntax`)
* `:! <command>` executes the shell `<command>`.
