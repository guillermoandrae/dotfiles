# Guillermo's dotfiles

[Mathias's readme](https://github.com/mathiasbynens/dotfiles/) is awesome. So is [Paul's](https://github.com/paulirish/dotfiles/).

I go between a Mac and an Ubuntu machine every day, so my project focuses more on Unix-y stuff and less on OS X stuff. I'm also not doing the same sort of work @paulirish and @mathiasbynens do; consequently, I have different needs.

Fork? If you really like my version, then sure. It might be better to fork [Mathias'](https://github.com/mathiasbynens/dotfiles/), though.

## Additional configuration

If there are more goodies you want to add that are highly personalized, add them to a file called `.extra` that should live in your home directory and keep that file out of version control. Mine's got some git configuration, a snippet from a poem, and a cheesy bit of inspiration for a quick smile when a new terminal is opened:

```bash
# Git credentials
# Not in the repository, to prevent people from accidentally committing under my name
GIT_AUTHOR_NAME="Guillermo A. Fisher"
GIT_COMMITTER_NAME="$GIT_AUTHOR_NAME"
git config --global user.name "$GIT_AUTHOR_NAME"
GIT_AUTHOR_EMAIL="guillermoandraefisher@gmail.com"
GIT_COMMITTER_EMAIL="$GIT_AUTHOR_EMAIL"
git config --global user.email "$GIT_AUTHOR_EMAIL"
 
# MOTD (Message Of The Day) 
# Breakthrough, by Carolyn M. Rodgers
cat << EOF

And my mouth has been open 
Most of the time but 
I ain't been saying nothin but 
Thinking about ev'rything 
And the partial pain has been 
How do I put my self on paper 
The way I want to be or am and be 
Not like any one else in this 
Black world but me

Break through, Mr. Fisher.

EOF
```

## Installation

You'll notice that the directory in this command is capitalized. That's because I'm strange, not because of a typo ;-). 

```bash
git clone git@github.com:guillermoandrae/dotfiles.git Dotfiles && cd Dotfiles && ./sync.sh
```
