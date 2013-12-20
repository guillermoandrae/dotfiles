# Guillermo's dotfiles

[Mathias's readme](https://github.com/mathiasbynens/dotfiles/) is awesome. So is [Paul's](https://github.com/paulirish/dotfiles/).

I go between a Mac and an Ubuntu machine every day, so my project focuses more on Unix-y stuff and less on OS X stuff. I'm also not doing the same sort of work @paulirish and @mathiasbynens do; consequently, I have different needs.

Fork? Sure!

## private config

Toss it into a file called `.extra` which you do not commit to this repo and just keep in your `~/`. 

I do something nice with my `PATH` there:

```shell
# PATH like a bawss
PATH=/opt/local/bin
PATH=$PATH:/opt/local/sbin
PATH=$PATH:/bin
PATH=$PATH:~/.rvm/bin
PATH=$PATH:~/code/git-friendly
# ...

export PATH
```

## Syntax highlighting

…is really important. even for these files.

Install [Dotfiles Syntax Highlighting](https://github.com/mattbanks/dotfiles-syntax-highlighting-st2) via [Sublime Text 2 Package Control](http://wbond.net/sublime_packages/package_control)


### Sensible OS X defaults

When setting up a new Mac, you may want to set some sensible OS X defaults:

```bash
./.osx
```

## overview of files
####  Automatic config
* `.vimrc`, `.vim` - vim config, obv.

#### shell environment
* `.aliases`
* `.bash_profile`
* `.bash_prompt`
* `.bashrc`
* `.exports`
* `.functions`
* `.extra` - not included, explained above

#### manual run
* `.osx` - run on a fresh osx machine
* `.brew` - homebrew initialization

#### git, brah
* `.git`
* `.gitattributes`
* `.gitconfig`
* `.gitignore`

* `.inputrc` - config for bash readline


## Installation

```bash
git clone git@github.com:guillermoandrae/dotfiles.git && cd dotfiles && ./sync.sh
```
