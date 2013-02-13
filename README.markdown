# yubrew's dotfiles

## dotfiles

Dotfiles are meant to be forked / shareable / scalable. These dotfiles are forked from [Todd Werth](http://github.com/twerth) and inspired by [Zach Holman](http://github.com/holman)'s [post on sharing dotfiles](http://zachholman.com/2010/08/dotfiles-are-meant-to-be-forked/).

This repo represents a subset of all my command-line folders.

## install

Run this:

```sh
git clone https://github.com/holman/dotfiles.git ~/.dotfiles
cd ~/.dotfiles
script/bootstrap
```

This will symlink the appropriate files in `.dotfiles` to your home directory.
Everything is configured and tweaked within `~/.dotfiles`.

The main file you'll want to change right off the bat is `zsh/zshrc.symlink`,
which sets up a few paths that'll be different on your particular machine.

`dot` is a simple script that installs some dependencies, sets sane OS X
defaults, and so on. Tweak this script, and occasionally run `dot` from
time to time to keep your environment fresh and up-to-date. You can find
this script in `bin/`.

## topical

Everything's built around topic areas. If you're adding a new area to your
forked dotfiles - say, "Java" - you can simply add a `java` directory and put
files in there. Anything with an extension of `.zsh` will get automatically
included into your shell. Anything with an extension of `.symlink` will get
symlinked without extension into `$HOME` when you run `script/bootstrap`.

## what's inside

A lot of stuff. Seriously, a lot of stuff. Check them out in the file browser
above and see what components may mesh up with you. Fork it, remove what you
don't use, and build on what you do use.

## components

I store all my command-line files in a folder (cl), then under that folder there are 3 sub-folders (cl/bin cl/etc cl/doc), to keep them organized away from all my other files.  I link (etc/link) the dot files to the root of my home folder, so I prefer to store them without the . (gitignore rather than .gitignore), then I add the dot in the link.  So if you use one, make sure you put the dot back.

  * ~
  ** cl
  *** bin
  *** docs
  *** etc
  **** vim
          
## warning

I mod these all the time, and sometimes I break stuff.  Also, my main platforms are OS X and Linux (Debian based) in the console, not XWindows.  Most of my stuff works just fine in something like gnome-terminal, but I usually only check my main platforms when I make changes.

## more info

"Blog post":http://blog.toddwerth.com/entries/9
