# yubrew's dotfiles

## dotfiles

Dotfiles are meant to be forked / shareable / scalable. These dotfiles are forked from [Todd Werth](http://github.com/twerth) and inspired by [Zach Holman](http://github.com/holman)'s [post on sharing dotfiles](http://zachholman.com/2010/08/dotfiles-are-meant-to-be-forked/).

This repo represents a subset of all my command-line folders.

## requirements
You need:
`git`
`brew`
`rvm use system` (if you dont' have vim installed already)

`brew install mercurial`
`brew install vim`

## install

Run this:

```sh
git clone https://github.com/yubrew/dotfiles.git ~/cl
cd ~/cl
source ./etc/link
```
This will symlink the appropriate files in `.dotfiles` to your home directory.
Everything is configured and tweaked within `~/cl`.

First, you'll want to look in `~/cl/etc` for `bash_profile` `bashrc` `bashrc_help`. That sets up aliasing 
and path displays.

## what's inside

I store all my command-line files in a folder (cl), then under that folder there are 3 sub-folders (cl/bin cl/etc cl/doc), to keep them organized away from all my other files.  I link (etc/link) the dot files to the root of my home folder, so I prefer to store them without the . (gitignore rather than .gitignore), then I add the dot in the link.  So if you use one, make sure you put the dot back.

  * ~
    * cl
      * bin
      * docs
      * etc
          * vim
          
## warning

I mod these all the time, and sometimes I break stuff.  Also, my main platform is OS X in the console, doing Ruby / Rails dev.

## more info

"Blog post":http://blog.toddwerth.com/entries/9

## vim shortcuts

It's also in vimrc.
`V` visual mode
`,n` nerdtree
`,f` fuzzy file search
`,c` toggle commenting
`/` search within file
`u` undo
`$` end of line
`^` start line
`Ctrl + }` navigate paragraph down
`Ctrl + {` navigate paragraph up
