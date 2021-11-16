 <!-- markdownlint-disable MD013-->
 <!-- vim: set tw=100 : -->
# How to build a songbook from this repository

You'll need to immerse yourself in geekiness for this at present as there is no pretty clicky way to
achieve it, and no fancy-pants web interface for it, but it is pretty easy, actually.

## System Requirements

You'll need certain software on your computer to make this work - how you get it will depend on
your OS.

1. Python

You can install this from here: [Python Downloads](https://www.python.org/downloads/)
At the time of writing this was version 3.10. Just download this or any later version and run the
installer.

Mac users will probably use the "universal installer" package

1. Git

Git is our means of managing songbook content and changes to songbook content on
[github](https://github.com). You can get this from the [git downloads
page](https://git-scm.com/downloads)

When you install git on windows it will ask you which default editor you want to use - if in doubt
choose 'notepad', or install one of the other suggestions. You probably won't need this anyway - see
[EDITING.md](EDITING.md) for a more user-friendly approach to editing the songsheets.
.
For Mac users, install [homebrew](https://brew.sh/) if you don't already have it and then
    
    brew install git

in a terminal window should do the trick.


1. (Optional) A decent terminal emulator

This will make things easier to use, IMO, but the default built-in MacOS Terminal and the Windows
Command Prompt (or powershell) will also work just fine.

On Windows git also comes with a shell called "git bash" - this is probably the best choice here.
You will be asked about this by the git installer wizard.


1. (Optional) A decent text (or programmer's) editor

If you want to make any changes to the songsheets, you will need an editor that makes this easier.
There are loads. Here are some...

TextEdit (mac)  - I think this is preinstalled
Notepad++ (windows) - although the default "Notepad" can also work, it is ugly and fiddly.
Atom (cross-platform, from github)

There's a decent list of them here, too: https://www.techradar.com/uk/best/best-text-editors

## Setting up

Now we'll take a copy of this locally and treat it with wanton abandon, or something.

1. clone the repository so you have a local copy

in your terminal


I'm afraid the only way to properly manage this is using a terminal - on Mac, there is a `terminal`
application, or for a more user-friendly approach you could install `iterm2` from
[here](https://iterm2.com/)


On windows, once you have git installed you will also have  `git bash` avaiable, which is a decent
terminal app. Or just stick to powershell, which you should have anyway.


